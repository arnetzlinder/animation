<template>
    <button id="animationBtn" class="animationBtn" @click="changeAnimation">Byt animation</button>
</template>

<script lang="ts">
export default {
  data() {
    return {
      showsRafael: false,
    };
  },
  methods: {
    changeAnimation() {
      // this.showsRafael = !this.showsRafael;
      // this.$emit('click', this.showsRafael);
      console.log('något hände');
    },
  },
};
</script>

<style lang="scss" scoped>
button {
  background-color: #ec9929;
  color: #22282c;
  font-family: 'Rowdies', cursive;;
  font-size: 1rem;
  width: 130px;
  height: 50px;
  padding: 0.5rem;
  border: 2px solid black;
  border-radius: 10px;
  position: relative;
  left: 0;
  display: flex;
  align-items: center;
  text-align: center;
  display: inline;
  z-index: 40;

  &:hover {
    background-color: #946220;
  }

  &:active {
    background-color: #fb8f02;
  }

  &:disabled {
    background-color: lightgrey;
  }
}
</style>