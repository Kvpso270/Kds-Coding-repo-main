<template>
  <div style="position: relative">
    <svg
      :width="width"
      :height="height"
      viewBox="0 0 1900 786"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect width="1900" height="786" :fill="rectColor" />
      <path
        d="M680 0H1900V772.512C1900 772.512 1432.94 839.74 1405.59 590.385C1378.25 341.03 1214.92 378.922 1162.11 473.041C1109.3 567.161 943.951 474.264 967.15 314.139C1014.79 -14.668 808.652 6.11164 680 0Z"
        :fill="pathColor"
      />
    </svg>
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    iconName: {
      type: String,
      default: "box",
    },
    width: {
      type: [Number, String],
      default: 1900.232143,
    },
    height: {
      type: [Number, String],
      default: 786.232143,
    },

    rectColor: {
      type: String,
      default: "currentColor",
    },
    pathColor: {
      type: String,
      default: "currentColor",
    },
  },
};
</script>

<style>
#headerTextBox {
  display: flex;
  flex-direction: column;
  width: 100%;
  z-index: 3;
  position: absolute;
  top: 60%;

  transform: translateY(-55%);
  justify-content: center;
  align-content: center;
  align-items: center;
}
.courseTitle {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 5em;
  line-height: 1em;
}
#HeaderSubTitle {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 2.5em;
  line-height: 2em;
  text-align: center;

  color: #ffffff;
}
.HeaderTitleText {
  width: 40%;
  font-family: Alatsi;
  font-style: normal;
  font-weight: normal;
  font-size: 2em;
  line-height: 1.2em;
  text-align: center;
  color: #000000;
}
</style>
<!--
    <Banner rectColor="#46BB6E" pathColor="#178C3F"></Banner>
-->