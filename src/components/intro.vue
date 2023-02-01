<template>
  <section id="Intro" class="scroll_sec">
    <div class="intro_txt" 
      data-aos="fade-right"
      data-aos-delay="50"
      data-aos-duration="1000"
      data-aos-easing="ease-in-out"
      data-aos-mirror="true"
      data-aos-once="false"
      data-aos-anchor-placement="top-center"
      >
      <h1>안녕하세요!</h1>
      <h2>프론트엔드 개발자</h2>
      <h2>박서희입니다.</h2>
    </div>
    <img src="../assets/mas.png">
  </section>
</template>
<script>
AOS.init();
</script>
<style scoped>
section{
  /* position: relative; */
  width: 100%; height: 100vh;
  background-color: black;
}
.intro_txt{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 50px;
}
.intro_txt>h1{
  text-align: left;
  font-size: 200px;
  font-weight: bold;
  color: white;
}
.intro_txt>h2{
  line-height: 170px;
  text-align: left;
  font-size: 150px;
  font-weight: bold;
  color: #ffcc00;
}
img{
  position: absolute;
  bottom: 100px; right: 30px;
  width: 400px;
  height: 400px;
  object-fit: cover;
  animation:ani 1s infinite alternate;  
}
@keyframes ani{
  0%{transform:translate(0,0);}
  100%{transform:translate(0,80px);}
}  
</style>