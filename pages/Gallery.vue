<template>
  <div class="member">
    <div class="bg-image-loop"></div>
    <v-container>
      <h1 class="headline-type1 my-12">Gallery</h1>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
.bg-image-loop {
	width: 100%;
	height: 600px; /* 画像の高さを指定 */
	position: relative;
	background: url("../static/img/slide-sample.jpg") repeat-x 0 0;
	background-size: auto 100%;
	animation: bgSlider 200s linear infinite;
	padding: 0;

  &:hover {
    animation-play-state: paused;
  }
}
@keyframes bgSlider {
	from { background-position: 0 0; }
    to { background-position: -13172px 0; }
}
</style>