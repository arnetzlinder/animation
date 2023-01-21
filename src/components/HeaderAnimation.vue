<template>
    <header>
        <img src="../../hearts.jpg" />
        <div class="button-holder">
            <AnimationButton />
        </div>
    </header>
</template>

<script lang="ts">
import AnimationButton from './AnimationButton.vue';

	export default {
        components: {
            AnimationButton
        },
    };
</script>

<style lang="scss" scoped>
    .button-holder {
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        top: -25px;
        position: relative;
    }
    header {
        margin-inline: auto;
        width: 100vw;
        height: 150px;
        background-color: #111e26;
        position: absolute;
        display: flex;
        flex-direction: column;
        justify-content: center;
        img {
        width: 25rem;
        height: 150px;
        position: relative;
        background-size: cover ;
        background-position: center;
        }
    }
</style>