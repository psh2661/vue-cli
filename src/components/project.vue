<template>
  <section id="Project01" class="scroll_sec">
    <div class="project_seomoon">
      <div class="left_cont">
        <p class="project_tit">서문시장야시장</p>
        <p class="project_type">리뉴얼 페이지-개인프로젝트</p>
        <p class="project_cont">
          단순히 시장을 홍보만하는 사이트가아니라<br>
          <span>"푸른도깨비의 축제"</span>라는 스토리와<br>
          푸른도깨비<span>"푸루다"</span>라는 도깨비 캐릭터를 더해<br>
          서문야시장의 아이덴티티를 만들어<br>
          의미가 담긴 사이트로 리뉴얼을 해보았습니다.</p>
        <p class="project_skill">SKILL : HTML5, CSS3 , JAVAscript, node, MySQL</p>
        <p class="project_date">작업 기간: 2022년 09월 초 ~ 2022년 11월 말</p>
        <a class="show_more" href="#">Show More ▶</a>
      </div>
      <div class="right_cont">
        <div class="aos_img">
          <img src="../assets/seomoon_mok.png">
        </div>
      </div>
    </div>
  </section>


  <section id="Project02" class="scroll_sec">
    <div class="project_eyeNlip">
      <div class="left_cont">
        <p class="project_tit">EYENLIP</p>
        <p class="project_type">리뉴얼 페이지-개인프로젝트</p>
        <p class="project_cont">상품의 종류가 다양하고 3개의 브랜드가
          모여있어<br>상품의 컨셉을 파악하기 어렵다고 생각하였습니다.<br>
          때문에 요즘 추세에 맞춘 상품 리스트를 선정하였고, <br>
          그 중 <span>“비건(vegan)"</span>을 주제로<br>심플하고 차분한 분위기를 연출하여<br>리뉴얼 작업을 하였습니다.</p>
        <p class="project_skill">SKILL : HTML5, CSS3 , JAVAscript, node, MySQL</p>
        <p class="project_date">작업 기간: 2022년 09월 초 ~ 2022년 11월 말</p>
        <a class="show_more" href="#">Show More ▶</a>
      </div>
      <div class="right_cont">
        <div class="aos_img">
          <img src="../assets/eyenlip_mok.png">
        </div>
      </div>
    </div>
  </section>


  <section id="Project03" class="scroll_sec">
    <div class="project_wonjoo">
      <div class="left_cont">
        <p class="project_tit">원주곤충마을박물관</p>
        <p class="project_type">리뉴얼 페이지-팀프로젝트</p>
        <p class="project_cont">
          기존 사이트의 테이블로만 마크업작업이 되어있던 사이트를<br>
          팀원들과 분석하면서 전체적인 컨셉을 잡고 <br>
          오시는길 section과 join / login페이지를 담당하였습니다<br>
          join / login페이지를 만들때 javascript로 유효성 검사를하면서<br>
          많은 공부가 되었던 과정이 었습니다.
        </p>
        <p class="project_skill">SKILL : HTML5, CSS3 , JAVAscript, node, MySQL</p>
        <p class="project_date">작업 기간: 2022년 11월 초 ~ 2022년 12월 말</p>
        <a class="show_more" href="#">Show More ▶</a>
      </div>
      <div class="right_cont">
        <div class="aos_img">
          <img src="../assets/seomoon_mok.png">
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
section{
  width: 100%; height: 100vh;
  background-color: white;
}
/* common */
.project_tit{
  font-size: 60px;
  font-weight: bold;
}
.project_type{
  padding-top: 10px;
  font-weight: bold;
  color: #888888;
}
.project_cont{
  padding-top: 50px;
  font-size: 20px;
  line-height: 30px;
}
.project_cont>span{
  /* font-size: 20px; */
  font-weight: bold;
}
.project_date{
  padding: 50px 0 20px 0;
  font-weight: bold;
}
.project_skill{
  padding-top: 10px;
  font-weight: bold;
  color: #ffcc00;
}
/* btn */
.show_more{
  padding: 5px 15px;
  color: #ffcc00;
  font-weight: bold;
  border: 1px solid #ffcc00;
  box-sizing: border-box;
}
.aos_img>img{
  width: 700px; height: auto;
}
/* project_seomoon */
.project_seomoon{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 70px;
  display: flex;
  justify-content: space-between;
}

/* project_eyeNlip */
.project_eyeNlip{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 70px;
  display: flex;
  justify-content: space-between;
}
/* project_wonjoo */
.project_wonjoo{
  width: 100%; height: auto;
  max-width: 1280px;
  margin: 0 auto;
  padding-top: 70px;
  display: flex;
  justify-content: space-between;
}
</style>