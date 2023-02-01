<template>
  <section id="About" class="scroll_sec">
    <div class="about_me">
      <div class="about_me_txt">
        <h1>통.통.튀는<br>아이디어를 갖고 있는</h1>
        <p>탄력있는 아이디어로 새로움을 보여주는 개발자!
          <br>사용자에게 늘 재미있고 즐기기 좋은 사이트를 디자인합니다.
        </p>
        <p class="skill">
          HTML5, CSS3, JAVAscript, jQuery, node.js, vue.js<br>
          VScode, MySQL, Heroku, Git, Github, AWS<br>
          Figma, Illustrator, Photoshop, Blender, Maya
        </p>
        <img src="../assets/mas.png">
      </div>
      <div class="about_me_cont">
        <div class="shc">
          <img src="../assets/notebook-front-front.png">
          <ul>
            <li>
              <p>(2023.02 이수)</p>
              <h1>노원 그린컴퓨터 아카데미 학원</h1>
              <h2>[디지털컨버전스] 뷰(Vue) 활용 프론트엔드 웹개발자 양성과정</h2>
            </li>
            <li>
              <p>(2020.03 졸업)</p>
              <h1>오사카 종합디자인 전문학교</h1>
              <h2>코믹아트학과</h2>
            </li>
            <li>
              <p>(2017.03 졸업)</p>
              <h1>오사카 휴먼 아카데미 일본어학교</h1>
              <h2>일본어</h2>
            </li>
            <li>
              <p>(2015.02 졸업)</p>
              <h1>한국 문화 콘텐츠 고등학교</h1>
              <h2>영상・애니메이션과</h2>
            </li>
          </ul>
        </div>
        <div class="comp">
          <img src="../assets/file-front-clay.png">
          <ul>
            <li>
              <p>(2021.06 ~ 2022.04)</p>
              <h1>합동회사 Ami - 번역,편집디자이너</h1>
            </li>
            <li>
              <p>(2020.09 ~ 2021.04)</p>
              <h1>합동회사 Ami - 번역,편집디자이너</h1>
            </li>
          </ul>
        </div>
        <div class="mdal">
          <img src="../assets/medal-front-clay.png">
          <ul>
            <li>
              <p>(2022.07 취득)</p>
              <h1>운전면허 보통 2종</h1>
            </li>
            <li>
              <p>(2019.12 취득)</p>
              <h1>일본어 능력 시험 - N2</h1>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
section{
  width: 100%; height: 100vh;
  background-color: black;
}
.about_me{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 70px;
  display: flex;
  justify-content: space-between;
}
.about_me_txt{
  position: relative;
}
.about_me_txt>h1{
  text-align: left;
  font-size: 60px;
  font-weight: bold;
  color: white;
}
.about_me_txt>p{
  text-align: left;
  font-size: 20px;
  color: white;
  padding: 20px 0;
}
.about_me_txt>.skill{
  font-size: 16px;
  color: #ffcc00;
}
.about_me_txt>img{
  position: absolute;
  left: 350px; bottom: 20px;
  width: 350px;
  height: auto;
  object-fit: cover;
}
.about_me_cont>div{
  padding-bottom: 15px;
}
/*  */
.shc{
  display: flex;
}
.shc>img{
  width: 100px;
  height: 100px;
  object-fit: cover;
  padding-right: 20px;
}
.shc>ul>li{
  padding-bottom: 10px;
}
.shc>ul>li>p{
  font-size: 16px;
  font-weight: 300;
  color: white;
}
.shc>ul>li>h1{
  font-size: 20px;
  font-weight: bold;
  color: #ffcc00;
}
.shc>ul>li>h2{
  font-size: 16px;
  color: white;
}
/*  */
.comp{
  display: flex;
}
.comp>img{
  width: 100px;
  height: 100px;
  object-fit: cover;
  padding-right: 20px;
}
.comp>ul>li{
  padding-bottom: 10px;
}
.comp>ul>li>p{
  font-size: 16px;
  font-weight: 300;
  color: white;
}
.comp>ul>li>h1{
  font-size: 20px;
  font-weight: bold;
  color: #ffcc00;
}
/*  */
.mdal{
  display: flex;
}
.mdal>img{
  width: 100px;
  height: 100px;
  object-fit: cover;
  padding-right: 20px;
}
.mdal>ul>li{
  padding-bottom: 10px;
}
.mdal>ul>li>p{
  font-size: 16px;
  font-weight: 300;
  color: white;
}
.mdal>ul>li>h1{
  font-size: 20px;
  font-weight: bold;
  color: #ffcc00;
}
</style>