<template>
  <devObjHeader id="devOHeader">
    <h2 id="HeaderSubTitle">Cours et exercices</h2>
    <Discover></Discover>
  </devObjHeader>
  <div id="DevOConteneur" class="CourseContainer">
    <br />
    <div class="container CoursePage">
      <div class="col-lg-12 subTitle">
        <div class="icon"><Avatar1></Avatar1></div>
        <h1>Cours</h1>
      </div>
      <article class="col-lg-10 course">
        <div class="medal">
          <GoldMedal width="275.232143" height="275.232143"></GoldMedal>
        </div>
        <div class="content">
          Niveau : Facile
          <h1>cours 1</h1>
          <p>
            Ce cours va te permettre de savoir à quoi ça sert et en quoi est-ce
            utile l'algorithmie dans la programmation et d'entrer doucement dans
            la logique d'un programme.
          </p>
        </div>
        <div class="play">
          <Play
            circleColor="#BB4646"
            @click="() => $router.push('/devO/devO')"
          ></Play>
        </div>
      </article>
      <article class="col-lg-10 course">
        <div class="medal">
          <GoldMedal width="275.232143" height="275.232143"></GoldMedal>
        </div>
        <div class="content">
          Niveau : Facile
          <h1>cours 2</h1>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore.
          </p>
        </div>
        <div class="play">
          <Play
            circleColor="#BB4646"
            @click="() => $router.push('/algo/course1')"
          ></Play>
        </div>
      </article>
      <article class="col-lg-10 course">
        <div class="medal">
          <SilverMedal width="275.232143" height="275.232143"></SilverMedal>
        </div>
        <div class="content">
          Niveau : Facile
          <h1>cours 3</h1>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore.
          </p>
        </div>
        <div class="play"><Play circleColor="#BB4646"></Play></div>
      </article>
      <div class="container-fluid text-center" style="margin: 20px">
        <Arrow arrowTransform="rotate(270)" target="AlgoHeader"></Arrow>
        <Arrow arrowTransform="rotate(90)" target="ExerciceConteneur"></Arrow>
      </div>
    </div>

    <div class="container CoursePage" id="ExerciceConteneur">
      <div class="col-lg-12 subTitle">
        <div class="icon"><Avatar1></Avatar1></div>
        <h1>Exercices</h1>
      </div>
      <article class="col-lg-10 excercise">
        <div class="medal">
          <GoldMedal width="125.232143" height="125.232143"></GoldMedal>
        </div>
        <div class="content">
          Niveau : Facile
          <h1>Exercice 1 :Lorem ipsum dolor sit amet</h1>
        </div>
        <div class="play"><Play circleColor="#BB4646"></Play></div>
      </article>
      <article class="col-lg-10 excercise">
        <div class="medal">
          <GoldMedal width="125.232143" height="125.232143"></GoldMedal>
        </div>
        <div class="content">
          Niveau : Facile
          <h1>Exercice 2 :Lorem ipsum dolor sit amet</h1>
        </div>
        <div class="play"><Play circleColor="#BB4646"></Play></div>
      </article>
    </div>
    <div class="container-fluid text-center" style="margin: 20px">
      <Arrow arrowTransform="rotate(270)" target="AlgoConteneur"></Arrow>
    </div>
  </div>

  <Footer>
    <Banner
      rectColor="#46BB6E"
      pathColor="#178C3F"
      height="100%"
      width="100%"
      class="col-lg-6"
    >
      <div class="centerLink">
        <h1 class="footerLink">DEVELOPPEMENT ORIENTE</h1>
        <Arrow arrowTransform="rotate(180)"></Arrow>
      </div>
    </Banner>

    <Banner
      rectColor="#4691BD"
      pathColor="#1E6995"
      height="100%"
      width="100%"
      class="col-lg-6"
    >
      <div class="centerLink">
        <h1 class="footerLink">DEVELOPPEMENT WEB</h1>
        <Arrow
          arrowTransform="rotate(0)"
          @click="() => $router.push('/web')"
        ></Arrow>
      </div>
    </Banner>
  </Footer>
</template>

<script>
//import AlgoHeader from "@/components/common/AlgoHeader.vue";
import devObjHeader from "@/components/common/devObjHeader.vue"
import Discover from "@/components/common/Discover.vue";
import Footer from "@/components/common/Footer.vue";
import GoldMedal from "@/assets/svg/icons/medal/gold-medal";
import SilverMedal from "@/assets/svg/icons/medal/silver-medal";
import Avatar1 from "@/assets/svg/icons/Avatar/Avatar1";
import Banner from "@/assets/svg/Headers/bannerObj.vue";
import Arrow from "@/assets/svg/icons/buttons/arrow.vue";
import Play from "@/assets/svg/icons/buttons/play_circle_filled.vue";

export default {
  components: {
    devObjHeader,
    Discover,
    GoldMedal,
    SilverMedal,
    Avatar1,
    Banner,
    Footer,
    Arrow,
    Play,
  },
};
</script>

<style lang="scss">
#DevOConteneur .medal,
#DevOConteneur .subTitle {
  background-color: #46BB6E;
}
</style>