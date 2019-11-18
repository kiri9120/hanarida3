<template>
  <div class="member">
    <v-container>
      <h1 class="headline-type1 my-12">Member</h1>
      <v-row no-gutters>
        <v-col v-for="(member, index) in members" :key="index" cols="6" sm="4" lg="3" class="pa-2">
          <v-card shaped tile raised>
            <v-img :src="member.image" aspect-ratio="1"></v-img>
            <v-card-title class="pb-0">{{ member.name }}</v-card-title>
            <v-card-text class="pb-0">{{ member.job }}</v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn icon :href="member.instagram" target="_blank">
                <v-icon>mdi-instagram</v-icon>
              </v-btn>
              <v-btn icon :href="member.twitter" target="_blank">
                <v-icon>mdi-twitter</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      members: [
        {
          name: '今瀧 健登',
          job: 'モデル',
          image: require('../static/img/member02.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        },
        {
          name: '山田 太郎',
          job: 'モデル',
          image: require('../static/img/member01.jpg'),
          instagram: 'https://www.instagram.com/watanabenaomi703',
          twitter: 'https://www.twitter.com/watanabe_naomi'
        }
      ]
    }
  }
};
</script>

