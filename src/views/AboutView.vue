<template>
  <div>
  <a href="https://soundcloud.com/jonny_boi_ist_haesslich"><img src="https://img.icons8.com/ios-filled/1000/000000/soundcloud.png" class="hv orange"/></a>
  <a href="https://github.com/Jomyy">
  <img src="https://img.icons8.com/ios-glyphs/200/000000/github.png" class="hv pink"/>
  </a>
  <a href="https://open.spotify.com/artist/6sP4WzEXeQ8vifuUgr3tZu?si=4c15izOlQq6K3ECywx94UA">
  <img src="https://img.icons8.com/ios-glyphs/200/000000/spotify.png" class="hv green"/>
  </a>
  <a href="https://www.youtube.com/c/jonny_ist_haesslich">
  <img src="https://img.icons8.com/ios-filled/200/000000/youtube-music.png" class="hv red"/>
  </a>
  <a href="https://www.youtube.com/c/jonny_ist_haesslich">
  <img src="https://img.icons8.com/ios-filled/200/000000/youtube-play.png" class="hv red"/>
  </a>
  </div>
</template>
<script>
import { reactive } from "@vue/reactivity";

export default {
  setup() {
    
  },
};
</script>
<style scoped>
.hv{
  transition-property: -moz-filter, -ms-filter, -o-filter, -webkit-filter, filter;
  transition-duration: 200ms;
}
.orange:hover{
  filter: invert(55%) sepia(72%) saturate(2929%) hue-rotate(337deg) brightness(103%) contrast(104%);
  -moz-filter: invert(55%) sepia(72%) saturate(2929%) hue-rotate(337deg) brightness(103%) contrast(104%);
  -webkit-filter: invert(55%) sepia(72%) saturate(2929%) hue-rotate(337deg) brightness(103%) contrast(104%);
  -o-filter: invert(55%) sepia(72%) saturate(2929%) hue-rotate(337deg) brightness(103%) contrast(104%);
  -ms-filter: invert(55%) sepia(72%) saturate(2929%) hue-rotate(337deg) brightness(103%) contrast(104%);

}
.green:hover{
  filter: invert(68%) sepia(29%) saturate(5682%) hue-rotate(93deg) brightness(92%) contrast(77%);
  -moz-filter: invert(68%) sepia(29%) saturate(5682%) hue-rotate(93deg) brightness(92%) contrast(77%);
  -webkit-filter: invert(68%) sepia(29%) saturate(5682%) hue-rotate(93deg) brightness(92%) contrast(77%);
  -ms-filter: invert(68%) sepia(29%) saturate(5682%) hue-rotate(93deg) brightness(92%) contrast(77%);
  -o-filter: invert(68%) sepia(29%) saturate(5682%) hue-rotate(93deg) brightness(92%) contrast(77%);
}
.pink:hover{
  filter: invert(49%) sepia(25%) saturate(7258%) hue-rotate(236deg) brightness(62%) contrast(69%);
  -moz-filter: invert(49%) sepia(25%) saturate(7258%) hue-rotate(236deg) brightness(62%) contrast(69%);
  -webkit-filter: invert(49%) sepia(25%) saturate(7258%) hue-rotate(236deg) brightness(62%) contrast(69%);
  -ms-filter: invert(49%) sepia(25%) saturate(7258%) hue-rotate(236deg) brightness(62%) contrast(69%);
  -o-filter: invert(49%) sepia(25%) saturate(7258%) hue-rotate(236deg) brightness(62%) contrast(69%);
}
.red:hover{
  filter: invert(13%) sepia(97%) saturate(6860%) hue-rotate(1deg) brightness(103%) contrast(108%);
  -moz-filter: invert(13%) sepia(97%) saturate(6860%) hue-rotate(1deg) brightness(103%) contrast(108%);
  -webkit-filter: invert(13%) sepia(97%) saturate(6860%) hue-rotate(1deg) brightness(103%) contrast(108%);
  -ms-filter: invert(13%) sepia(97%) saturate(6860%) hue-rotate(1deg) brightness(103%) contrast(108%);
  -o-filter: invert(13%) sepia(97%) saturate(6860%) hue-rotate(1deg) brightness(103%) contrast(108%);
}
div{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  padding: 0px;
  margin: 0px;
  height:100vh;
}
img{
  width:6vw;
}
svg{
  width:vw;
}
</style>