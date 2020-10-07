<template>
  <div class="text-center">
    <v-dialog v-model="dialog" width="500">
      <template v-slot:activator="{ on, attrs }">
        <a color="red lighten-2" dark v-bind="attrs" v-on="on">
          Privacy Policy
        </a>
      </template>

      <v-card>
        <v-card-title class="headline grey darken-1 mb-6">
          プライバシーポリシー
        </v-card-title>

        <v-card-text>
          当サイトでは、Googleの提供するアクセス解析サービス「GoogleAnalytics」を使用しています。これにはこれにはデータ収集のためにCookieを使用しておりますが、このデータは匿名で収集されており、個人を特定するものではありません。Googleアナリティクスのデータ収集、処理の仕組みについては、「ユーザーがGoogleパートナーのサイトやアプリを使用する際のGoogleによるデータ使用」のページを参照下さい。また、ユーザーがCookieの無効を希望する場合、こちらへアクセスすることで、それが可能となります。
        </v-card-text>

        <v-divider></v-divider>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="primary" text @click="dialog = false"> 了解 </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data: () => {
    return {
      dialog: false,
    }
  },
})
</script>
