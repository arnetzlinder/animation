<!-- ********************************** HTML ********************************************* -->
<template>
	<div class="img-container">
		<SVGAurelia />
	</div>
</template>

<!-- ********************************** script ********************************************* -->
<script lang="ts">
	import { gsap } from "gsap";
	import SVGAurelia from "./SVGAurelia.vue";
	export default {
		name: "AureliaAnimation",
		components: {
			SVGAurelia,
		},
		data() {
			return {};
		},
		mounted() {
					gsap.to('#a1', { rotate: 720, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#r', { scale: 1.8, y:200, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#l', { scale: 1.8, y:-100, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#a2', { rotate: -360, duration: 4, scale: 0.5, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#u', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#e', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#i', { scale: 0.5, duration: 2, ease: 'none', repeat: -1, yoyo: true});
                    gsap.to('#Hjärta', { scale: 0.5, x: 250, y: 120, duration: 3});
                    gsap.to('#Hjärta', { scale: 1, x: 500, y: 0, delay: 3, duration: 3});
                    gsap.to('#Hjärta', { scale: 1.2, delay: 6, duration: 0.4, yoyo: true, repeat: -1});
                    gsap.to('#Aurelia',{opacity: 0, duration: 5, yoyo :true, repeat: -1});
				}
			};
</script>