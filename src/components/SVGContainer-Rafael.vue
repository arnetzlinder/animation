<template>
	<div class="img-container-r">
		<SVGRafael />
	</div>
</template>

<!-- ********************************** script ********************************************* -->
<script lang="ts">
	import { gsap } from "gsap";
	import SVGRafael from "./SVGRafael.vue";
	export default {
		name: "RafaelAnimation",
		components: {
			SVGRafael,
		},
		data() {
			return {};
		},
		mounted() {
                gsap.to('#r', { rotate: 720, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#a1', { scale: 1.8, y:200, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#a2', { scale: 1.8, y:-100, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#l', { rotate: -360, duration: 4, scale: 0.5, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#f', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#e', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#i', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                gsap.to('#Rafael', {x: 500, duration: 5, yoyo: true, repeat: -1})
                gsap.to('#Spöke', { scale: 0.5, y: 220, duration: 3});
                gsap.to('#Spöke', { scale: 1, x: 500, y: 300, delay: 3, duration: 3});
                gsap.to('#Spöke', { scale: 0.3, rotate:-1080, delay: 6, duration: 1.5, yoyo: true, repeat: -1, ease: 'slow'});
				}
			};
</script>