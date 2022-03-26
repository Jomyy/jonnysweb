<template>
  <div id="HomeView">
    <div class="home" id="title">
      <h1 id="header">Jonny</h1>
     
    </div>
    <section id="fact1" class="stick">
      <div>
        <h1>Music</h1>
      </div>

      <div>
        <p>I'm a musician in my freetime, I produce every genre of music, be it synthwave, trap, hip-hop or, 80s pop. You can find my music on <a href="https://open.spotify.com/artist/6sP4WzEXeQ8vifuUgr3tZu?si=Xh63Y6nqTz2fMzjQAmboQQ">Spotify</a>,<a href="https://www.youtube.com/c/jonny_ist_haesslich">Youtube</a>, and many more platforms!</p>
      </div>
    </section>
    <section id="fact2" class="stick">
      <div>
        <h1>Video</h1>
      </div>

      <div>
        <p>I also do video editing, I edited all the videos on my <a href="https://www.youtube.com/c/jonny_ist_haesslich">Youtube</a> channel and many more!</p>
      </div>
    </section>
    <section id="fact3" class="stick">
      <div>
        <h1>Coding</h1>
      </div>

      <div>
        <p>And last but not least: I programm... in fact I programmed this website. You can find my source code on <a href="https://github.com/Jomyy">Github</a></p>
      </div>
    </section>
  </div>
</template>
<script>
import { reactive } from "@vue/reactivity";

export default {
  setup() {
    
  },
  mounted(){
    document.getElementById("header").style.opacity = ((window.innerHeight + document.getElementById("HomeView").getBoundingClientRect().top * 2) / +window.innerHeight).toString();
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
    

  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  },

  methods: {
    handleScroll(event) {
      document.getElementById("header").style.opacity = ((window.innerHeight + document.getElementById("HomeView").getBoundingClientRect().top * 2) / +window.innerHeight).toString();
      
    },
  },
};
</script>

<style scoped>

#fact2 {
  background-color: fuchsia;
}
#fact3 {
  background-color: mediumslateblue;
}
h1 {
  font-size: max(10vw, 30px);
}

.home {
  scroll-snap-align: start;
  display: flex;
  padding: 0px;
  margin: 0px;
}
.home h1 {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0px;
  padding: 10px;
}

.stick h1 {
  margin: 0px;
  text-align: center;
  align-content: center;
  padding: 0px;
  word-break: break-all;
}
.stick a {
  color: blue;
}
.stick div {
  display: flex;
  width: 50vw;
  padding: 0px;
  margin: 0px;
  padding-top: 0px;
  align-items: center;
  justify-content: center;
  justify-items: center;
}

.stick div p {
  text-align: center;
  width: 30vw;
}
.stick {
  display: flex;
  flex-direction: row;
  justify-content: center;
  height: 100vh;
  width: 100vw;
  scroll-snap-align: start;
  background-color: aqua;
}

.home {
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  height: 100vh;
  width: 100vw;
}
html {
  height: 100vh;
  height: 100vw;
}
@media (max-width: 400px) {
  .stick {
    display: flex;
    justify-content: center;
    flex-direction: column;
  }
  .stick div {
    text-align: center;
    width: 100vw;
  }
}
</style>
