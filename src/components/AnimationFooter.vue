<template>
        <footer>
      <ul class="contact">
        <li class="contact-images"> <span class="location"> <i class="fa-solid fa-location-dot"></i></span> Stockholm</li>
        <li> <a href="https://github.com/arnetzlinder" class="contact-images"><span class="github"> <i class="fa-brands fa-github"></i></span> </a></li>
        <li> <a href="https://www.linkedin.com/in/susanne-arnetz-linder-999a2481/" class="contact-images"><span class="linkedIn"> <i class="fa-brands fa-linkedin"></i></span> </a></li>
    </ul>
    </footer>
</template>

<script lang="ts">
	export default {};
</script>

<style lang="scss" scoped>
.contact {
  display: flex;
  position: absolute;
  list-style: none;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  background-color: #111e26;
  width: 100%;
  margin: 0;
  padding: 10px 0;
  .contact-images{
    color: #cbf7ff;
  }
}
</style>