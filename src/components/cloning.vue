<template>
  <section id="Cloning" class="scroll_sec">
    <div class="cloning_text">
      <h1>Cloning</h1>
      <h2></h2>
      <p id="dynamic"></p>
      <div class="cloning_box">
        <ul :class="Fstyle">
          <li v-for="wcl of cloningS">
            <a :href="wcl.href">{{ wcl.name }}</a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "App",
  data(){
    return{
      cloningS:[
        { name : "도시락통(웹 클로닝)", href : "https://github.com/psh2661/2023.01.05_dosirak.git" },
        { name : "싱그러운집(웹 클로닝)", href : "https://github.com/psh2661/2023.01.05_singu.git" },
        { name : "평창리치먼드(웹 클로닝)", href : "https://github.com/psh2661/2023.01.05_richmond.git" },
      ],
    };
  },
  mounted() {
      //타이핑 효과
      const target = document.querySelector('#dynamic');
      const string = "저의 기초의 시작, 웹 클로닝입니다." //원하는 텍스트
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
.cloning_text{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding: 70px 0;
}
/*css 작성하기*/
.cloning_text>h1 {
  font-size: 60px;
  font-weight: bold;
  color: white;
}
.cloning_text>h2 {
  font-size: 20px;
  color: white;
}
.cloning_text #dynamic {
  position: relative;
  display: inline-block;
  font-size: 35px;
  color: white;
}
/*커서모양 만들기*/
.cloning_text #dynamic::after {
    content: "";
    display: block;
    position: absolute;
    top: 0;
    right: -10px;
    width: 4px;
    color: white;
}
/*css active클래스에 속성추가*/
.cloning_text #dynamic.active::after{
    /* display: none; */
    color: yellow;
}

/* cloning_box */
.cloning_box{
  margin: 0 auto;
}
.cloning_box>ul{
  padding-top: 50px;
  display: flex;
  justify-content: space-between;}
.cloning_box>ul>li{
  width: 30%; height: auto;
  box-sizing: border-box;
  background-color: #ffcc00;
  border-radius: 30px;
  text-align: center;
}
.cloning_box>ul>li>a{
  align-items: center;
  font-size: 30px;
  font-weight: bold;
  color: black;
}
</style>