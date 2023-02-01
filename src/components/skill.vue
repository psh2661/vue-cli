<template>
  <section id="Skill" class="scroll_sec">
    <div class="skill_text">
      <h1>Cloning</h1>
      <h2></h2>
      <p id="dynamic"></p>
    </div>
  </section>
</template>
<script>
export default {
  name: "App",
  mounted() {
      //타이핑 효과
      const target = document.querySelector('#dynamic');
      const string = "기초의 시작, 웹 클로닝입니다." //원하는 텍스트
      const split = string.split(""); 
      //string의 텍스트를 여러개의 문자열로 나눠줌

      console.log(target)
      //문자열을 한개씩 나타내주는 함수 만들기
      function dynamic(arr){
          if(arr.length > 0){
              target.textContent += arr.shift();
              setTimeout(function(){
                  dynamic(arr)}, 150) //0.08초 후에 dynamic 함수를 실행
          }
      }
      // dynamic(split); //dynamic 함수에 split 인자 넣어서 실행
      function reset(){
          target.textContent = ""; //textContent의 내용 없애주기
          const resplit = string.split("");
          //string의 텍스트를 여러개의 문자열로 나눠주고 resplit 변수에 할당
          dynamic(resplit);
          //dynamic 함수에 resplit인자를 넣어서 실행
      }
      function dynamic(split){
          if(split.length > 0){
              target.textContent += split.shift();
              setTimeout(function(){
                  dynamic(split)}, 150)
          }else{
              setTimeout(reset, 3000); 
              //3초 후에 reset 함수 실행
          }
      }
      dynamic(split);
      function blink(){
          target.classList.toggle('active');
      }
      setInterval(blink, 500) //blink 함수를 0.5초마다 실행
      },
}
</script>
<style scoped>
section{
  width: 100%; height: 100vh;
  background-color: black;
}
.skill_text{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 50px;
}
.skill_container{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
}

.flow-text {
  display: flex;
  flex: 0 0 auto;
  white-space: nowrap;
  overflow: hidden;
  transition: 0.3s;
  font-size: 2.5rem;
  font-weight:bold;
  color: #9D9993;
}
.flow-text:hover {
  color: #000;
}
.flow-text:hover .skill_wrap {
  animation-play-state: paused;
  cursor: pointer;
}
.skill_wrap {
  animation: textLoop 30s linear infinite;
  padding-right: 1.4881vw;
}

@keyframes textLoop {
  0% {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
  100% {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }
}

/*css 작성하기*/
.skill_text>h1 {
  font-size: 60px;
  font-weight: bold;
  color: white;
}
.skill_text>h2 {
  font-size: 20px;
  color: white;
}
.skill_text #dynamic {
  position: relative;
  display: inline-block;
  font-size: 35px;
  color: white;
}
/*커서모양 만들기*/
.skill_text #dynamic::after {
    content: "";
    display: block;
    position: absolute;
    top: 0;
    right: -10px;
    width: 4px;
    color: white;
}
/*css active클래스에 속성추가*/
.skill_text #dynamic.active::after{
    /* display: none; */
    color: yellow;
}
</style>