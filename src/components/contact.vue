<template>
  <section id="Contact" class="scroll_sec">
    <div class="contact_wrap">
      <div class="contact_me">
        <h1>CONTACT ME!</h1>
        <h2>포트폴리오를 끝까지 봐주셔서 감사합니다.</h2>
        <!-- <ul>
          <li><a href="mailto:psh2661@gmail.com">Email psh2661@gmail.com</a></li>
          <li><a href="tel:010-3850-2668">Phone 010-3850-2668</a></li>
          <li><a href="https://github.com/psh2661/2023.01.05_eyeNlip.git" target="_blank">Github https://github.com/psh2661</a></li>
        </ul> -->
    </div>

    <div class="back color-9">
      <div class="row columns">
        <h3>Effect 39</h3>
        <ul class="menu align-center expanded text-center SMN_effect-39">
          <li><a href="mailto:psh2661@gmail.com">Email psh2661@gmail.com</a></li>
          <li><a href="tel:010-3850-2668">Phone 010-3850-2668</a></li>
          <li><a href="https://github.com/psh2661/2023.01.05_eyeNlip.git" target="_blank">Github https://github.com/psh2661</a></li>
        </ul>
      </div>
	  </div>

    <div class="contact_bot_txt">
      <p>본 페이지는 상업적 목적이 아닌 개인 포트폴리오용으로 제작되었습니다.<br>© 2023 PARK SEOHEE. All Rights Reserved.</p>
    </div>
    </div>
  </section>
</template>
<script>
// export default {
//   data(){
//     return{
//       contactS:[
//         { name: "Email", cons: "psh2661@gmail.com" },
//         { name: "Call", cons: "010-3850-2668" },
//         { name: "Github", cons: "https://github.com/psh2661/2023.01.05_eyeNlip.git" },
//       ],
//     };
//   },
// }
</script>
<style scoped>
section{
  width: 100%; height: 100vh;
  background-color: black;
}
.contact_wrap{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 70px;
}
.contact_me>h1{
  font-size: 60px;
  color: #ffcc00;
}
.contact_me>h2{
  font-size: 20px;
  color: white;
  padding-bottom: 20px;
}
/* .contact_me>ul{
  padding: 50px 0 200px 0;
} */
.contact_me>ul>li{
  padding-bottom: 30px;
}
/* contact_bot_txt */
.contact_bot_txt>p{
  color: white;
  font-size: 10px;
  font-weight: 300;
  text-align: center;
}



/*  */
.menu{
  padding: 20px 0 100px 0;
}
.menu>li{
  padding-bottom: 30px;
}
.SMN_effect-39 a:before, .SMN_effect-39 a:after {
	content: '';
	position: absolute;
	width: 5px;
	border-radius: 50%;
	background: #ffcc00;
	top: 35px;
	transition: height 0.3s 0.3s ease, border-radius 0.3s 0.3s ease, top 0.3s 0.3s ease, width 0.3s ease;
}

.SMN_effect-39 a:before {
	height: 5px;
	left: 0;
}

.SMN_effect-39 a:after {
	height: 0;
	right: 0;
}

.SMN_effect-39 a:hover:before, .SMN_effect-39 a:hover:after {
	top: 10%;
	width: 55%;
	height: 80%;
	z-index: -1;
	border-radius: 5px;
	transition: height 0.3s ease, border-radius 0.3s ease, top 0.3s ease, width 0.3s 0.3s ease;
}

.SMN_effect-39 a {
  width: 600px; height: auto;
	z-index: 1;
	display: inline-block;
	padding: 10px 20px;
	position: relative;
	transition: all 0.3s ease;
  /* 추가 */
  font-size: 30px;
  font-weight: bold;
  text-align: left;
  display: block;
  color: white;
}

.SMN_effect-39 a:hover {
	transition: all 0.3s 0.3s ease;
	text-decoration: none;
	color: black;
}
</style>