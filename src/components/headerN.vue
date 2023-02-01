<template>
  <nav id="nav_header">
    <div>
      <h1>logo</h1>
    </div>
    <ul class="menu">
      <li v-on:click="gosection" data-target="Intro" class="gotosce">
        Intro
      </li>
      <li v-on:click="gosection" data-target="About" class="gotosce">
        About
      </li>
      <li v-on:click="gosection" data-target="Project01" class="gotosce">
        Project
      </li>
      <li v-on:click="gosection" data-target="Cloning" class="gotosce">
        Cloning
      </li>
      <li v-on:click="gosection" data-target="Contact" class="gotosce">
        Contact
      </li>
    </ul>
  </nav>
</template>
<script>
  import {onMounted}  from 'vue'
  export default {
    data() {
      return {
        scrollPosition: null,
      };
    },
    methods: {
      gosection(e) {
        if (!e.target.matches(".gotosce")) return;
        e.preventDefault();
        const sec = document.getElementById(e.target.dataset.target);
        if (sec) {
          sec.scrollIntoView({ behavior: "smooth" });
        }
      },
    },
    setup(){
        onMounted(() => {
          window.addEventListener("scroll",()=>{
            const menu = document.getElementById("nav_header");
            const Project01 = document.getElementById("Project01");
            const Cloning = document.getElementById("Cloning");
            const scrollY = window.pageYOffset;
            if( Project01.offsetTop <= scrollY ){
              menu.classList.add('change_color');
              if(Cloning.offsetTop <= scrollY){
              menu.classList.remove('change_color');
            }
            }else{
              menu.classList.remove('change_color');
            }
          })
        })
      }
  };
</script>
<style scoped>
  nav {
    width: 100%;
    height: auto;
    padding: 0 30px;
    box-sizing: border-box;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    left: 50%;
    transform: translate(-50%);
    transition: all 300ms ease;
  }
  .menu {
    padding: 10px 0;
    display: flex;
    justify-content: center;
  }
  .menu > li {
    position:relative;
    cursor: pointer;
    padding: 0 20px;
    padding-bottom: 10px;
    box-sizing: border-box;
  }
  .menu > li::after{
    content: '';
    display: block;
    position:absolute;
    left:0; bottom:0;
    width:0%;
    border-bottom: 2px solid #ffcc00;
    -webkit-transition:all .4s cubic-bezier(0.68, -0.55, 0.265, 1.55); -o-transition:all .4s cubic-bezier(0.68, -0.55, 0.265, 1.55); transition:all .4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }
  .menu > li:hover::after{
    width: 100%;
  }
  #nav_header{
    position: fixed;
    color: #fff;
    top: 0;
  }
  #nav_header.change_color {
    color: black;
  }
</style>