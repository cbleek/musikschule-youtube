<template>
  <q-page class="flex flex-center">
    <div class="musikschule">
    <img src="/musikschule.jpg" usemap="#youtube" ismap="ismap" border="0">
    <map name="youtube">
      <area alt="Streicher" title="Streicher" href="https://youtu.be/MaTpHKRBWds" coords="338,697,530,870" shape="rect">
      <area alt="Klavier" title="Klavier" href="https://youtu.be/GNjgwm0KEDc" coords="614,694,787,861" shape="rect">
      <area alt="Trompete" title="Trompete" href="https://youtu.be/qfE5OJ8zlqM" coords="872,694,1055,876" shape="rect">
      <area alt="Tanz" title="Tanz" href="https://youtu.be/JKB2VOGt0MU" coords="346,935,525,1112" shape="rect">
      <area alt="Querflöte" title="Querflöte" href="https://youtu.be/N_5jM19F5gE" coords="610,933,794,1118" shape="rect">
      <area alt="Gitarre" title="Gitarre" href="https://youtu.be/y_N-IDAzCdA" coords="872,929,1043,1108" shape="rect">
      <area alt="Flöte" title="" href="https://youtu.be/8EqvyyCLW_E" coords="348,1175,532,1361" shape="rect">
      <area alt="KiKo Männchen" title="KiKo Männchen" href="https://youtu.be/gfzixOp2-7g" coords="610,1178,783,1519" shape="rect">
      <area alt="Schlagzeug" title="Schlagzeug" href="https://youtu.be/IqIhRXxKdtM" coords="880,1182,1053,1355" shape="rect">
    </map>

    <div class="intro">
      <iframe width="180" height="300"
        src="https://www.youtube.com/embed/gfzixOp2-7g"
        title="Intro"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

<!--    <div class="streicher">
      <iframe width="180" height="315"
        src="https://www.youtube.com/embed/MaTpHKRBWds"
        title="Streicher"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

    <div class="klavier">
      <iframe width="180" height="315"
        src="https://www.youtube.com/embed/GNjgwm0KEDc"
        title="Klavier"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

    <div class="trompete">
      <iframe width="180" height="315"
        src="https://www.youtube.com/embed/qfE5OJ8zlqM"
        title="Trompete"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>-->

    <div class="tanz effect effect-3">
      <iframe frameborder="0"
      title="Tanz"
      scrolling="no"
      marginheight="0"
      marginwidth="0"
      width="180"
      height="179"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      type="text/html"
      src="https://www.youtube.com/embed/JKB2VOGt0MU?autoplay=0&fs=1&iv_load_policy=3&showinfo=0&rel=0&cc_load_policy=0&start=0&end=0&vq=medium">
      </iframe>
    </div>
<!--


    <div class="q-video">
      <iframe width="560" height="315"
        src="https://www.youtube.com/embed/N_5jM19F5gE"
        title="Querflöte"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

    <div class="q-video">
      <iframe width="560" height="315"
        src="https://www.youtube.com/embed/y_N-IDAzCdA"
        title="Gitarre"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

    <div class="q-video">
      <iframe width="560" height="315"
        src="https://www.youtube.com/embed/8EqvyyCLW_E"
        title="Flöte"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>

    <div class="q-video">
      <iframe width="560" height="315"
        src="https://www.youtube.com/embed/gfzixOp2-7g"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </div>-->
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex'
})
</script>

<style lang="scss">

$bg-color: #F1E9DA;
$link-text-color: #fff;
$button-bg-1: #541388;
$button-bg-2: #D90368;
$button-bg-3: #104547;
$button-bg-4: #4F000B;
$button-bg-5: #F28123;
$border-radius: 6px;
$overlay-color: #fff;

.musikschule {
  position: relative;
}
.intro {
  position: absolute;
  top: 1180px;
  left: 610px;
  border: 1px solid red;
}
.tanz {
  position: absolute;
  top: 930px;
  left: 344px;
  border: 1px solid blue;
}

.tanz:hover {
  border: 1px solid yellow;
}
.effect {
  text-align: center;
  //display: inline-block;
  //position: relative;
  text-decoration: none;
  color: $link-text-color;
  text-transform: capitalize;
  /* background-color: - add your own background-color */
  font: {
    family: 'Roboto', sans-serif; /* put your font-family */
    size: 18px;
  }
  padding: 20px 0px;
  width: 150px;
  border-radius: $border-radius;
  //overflow: hidden;
}

.effect.effect-3 {
  transition: all 0.2s linear 0s;

  &:before {
    content: "\f178";
    font-family: FontAwesome;
    position: absolute;
    display: flex;
    align-items: center;
    justify-content: center;
    position: absolute;
    top: 100%;
    left: 0px;
    width: 100%;
    height: 100%;
    text-align: center;
    font-size: 30px;
    transition: all 0.2s linear 0s;
  }

  &:hover {
    text-indent: -9999px;

    &:before {
      top: 0;
      text-indent: 0;
    }
  }
}

</style>
