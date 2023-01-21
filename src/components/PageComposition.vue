<template>
    <div>
        <HeaderAnimation @click="toggleRafael" />
        <div class="animationDiv">
            <div class="Aurelia">
             <SVGcontainerAurelia />
            </div>
        <div>
            <SVGcontainerRafael :class="{ Rafael: true, show: showsRafael }"/>
        </div>
    </div>
</div>
</template>

<script lang="ts">
import HeaderAnimation from './HeaderAnimation.vue';
import SVGcontainerAurelia from './SVGcontainer-Aurelia.vue';
import SVGcontainerRafael from './SVGcontainer-Rafael.vue';

export default {
  components: {
    HeaderAnimation,
   SVGcontainerAurelia,
   SVGcontainerRafael,
  },
  data() {
    return {
      showsRafael: false,
    };
  },
  methods: {
    toggleRafael() {
      console.log('click');
      this.showsRafael = !this.showsRafael;
    },
  },
};
</script>

<style lang="scss" scoped>
.animationDiv {
    width: 70%;
    height: auto;
    margin-left: 10rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    top: 200px;
}

.Rafael {
    display: none;
}
div.show {
    display: block;
    position: fixed;
    z-index: 60;
    width: 100%;
    min-height: 100vh;
    top: 200px;
    bottom: 0;
    left: 0;
    overflow-y: scroll;
    position: fixed;
    background-color: white;

}

</style>