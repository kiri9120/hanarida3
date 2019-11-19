<template>
  <div class="home">
    <img class="logo" src="../static/img/logo-main.png" alt="ロゴ" />
    <v-row no-gutters v-if="$vuetify.breakpoint.xsOnly">
      <v-col
        v-for="(item, index) in topItems"
        :key="`first-${index}`"
        cols="4"
        style="height: calc(calc(100vh - 56px) / 3)"
      >
        <v-hover v-slot:default="{ hover }">
          <v-card
            outlined
            tile
            :style="{ backgroundColor: item.color }"
            :to="item.link"
            style="height: 100%; position: relative; border: none;"
          >
            <p class="top-text">
              {{ item.name }}
            </p>
          </v-card>
        </v-hover>
      </v-col>
    </v-row>
    <v-row no-gutters v-else>
      <v-col
        v-for="(item, index) in topItems"
        :key="`second-${index}`"
        cols="4"
        style="height: calc((100vh - 56px) / 3)"
      >
        <v-hover v-slot:default="{ hover }">
          <v-card
            outlined
            tile
            :style="{ backgroundColor: item.color }"
            :to="item.link"
            style="height: 100%; border: none; background-size: cover;"
          >
            <v-expand-transition>
              <div
                v-if="hover"
                class="d-flex transition-fast-in-fast-out grey darken-2 v-card--reveal display-2 white--text"
                style="height: 100%;"
              >
                {{ item.name }}
              </div>
            </v-expand-transition>
          </v-card>
        </v-hover>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    Logo,
    VuetifyLogo
  },
  data() {
    return {
      topItems: [
        {
          name: "TOP",
          color: "#dcb6c6",
          link: "/"
        },
        {
          name: "ABOUT",
          color: "#a5c1c2",
          link: "/about"
        },
        {
          name: "MEMBER",
          color: "#f4b684",
          link: "/member"
        },
        {
          name: "CONTACT",
          color: "#82b783",
          link: "/contact"
        },
        {
          name: "NEWS",
          color: "#a1994c",
          link: "/news"
        },
        {
          name: "WORKS",
          color: "#ad9089",
          link: "/works"
        },
        {
          name: "GALLERY",
          color: "#e68888",
          link: "/gallery"
        },
        {
          name: "NEWS",
          color: "#8392b4",
          link: "/news"
        },
        {
          name: "NEWS",
          color: "#f2ddb2",
          link: "/news"
        }
      ]
    };
  }
};
</script>
<style scoped lang="scss">
.home {
  position: relative;
}
.logo {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateY(-50%) translateX(-50%);
  z-index: 2;
  width: 50%;
  min-width: 200px;
  max-width: 400px;
  pointer-events: none;
}
.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: .5;
  position: absolute;
  width: 100%;
}
</style>
