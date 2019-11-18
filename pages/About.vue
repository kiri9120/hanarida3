<template>
  <div class="about">
    <v-container>
      <h1 class="headline-type1 my-12">About</h1>
      <div class="slash-wrapper my-12">
        <div class="slash-text">
          <div title="Vision" class="top"></div>
          <div title="Vision" class="bottom"></div>
        </div>
      </div>
      <p>
        <vue-typer text='テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。' :repeat='0'></vue-typer>
      </p>
      <div class="slash-wrapper my-12">
        <div class="slash-text">
          <div title="Mission" class="top"></div>
          <div title="Mission" class="bottom"></div>
        </div>
      </div>
      <p>
        <vue-typer text='テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。' :repeat='0'></vue-typer>
      </p>
      <div class="slash-wrapper my-12">
        <div class="slash-text">
          <div title="Value" class="top"></div>
          <div title="Value" class="bottom"></div>
        </div>
      </div>
      <p>
        <vue-typer text='テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。テキストが入ります。' :repeat='0'></vue-typer>
      </p>
    </v-container>
  </div>
</template>
<script>
import { VueTyper } from 'vue-typer'
export default {
  components: {
    VueTyper
  }
}
</script>

<style scoped lang="scss">
.slash-wrapper {
  height: 100px;
  position: relative;
  overflow: hidden;
  -webkit-transform: rotate(-5deg);
  -moz-transform: rotate(-5deg);
  -o-transform: rotate(-5deg);
  -ms-transform: rotate(-5deg);
  transform: rotate(-5deg);

  .slash-text {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    text-shadow: 3px 3px 3px rgba(0,0,0,0.5);

    .top, .bottom {
      text-align: left;
      font: 62px/100px arial;
      text-transform: uppercase;
      text-align: center;
      overflow: hidden;

      &::before {
        content: attr(title);
        -webkit-transform: rotate(5deg);
        -moz-transform: rotate(5deg);
        -o-transform: rotate(5deg);
        -ms-transform: rotate(5deg);
        transform: rotate(5deg);
      }
    }

    .top {
      position: absolute;
      top: 0;
      left: 5px;
      right: 0;
      bottom: 50%;

      &::before {
        position: absolute;
        bottom: -50px;
        left: 0;
        right: 0;
      }
    }

    .bottom {
      position: absolute;
      top: 50%;
      left: 0;
      right: 5px;
      bottom: 0;

      &::before {
        position: absolute;
        top: -50px;
        left: 0;
        right: 0;
      }
    }
  }
}


</style>