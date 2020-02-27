<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <h1 class="display-2 text-center mb-8">基礎から始める株式投資</h1>
      <v-card>
        <v-card-title class="headline">
          株式投資を始めるにはどうしたらいいの？
        </v-card-title>
        <v-card-text class="subtitle-1">
          <p>株式投資にはまず証券口座を開く必要があります。</p>
          <p>証券口座は大手の会社であればどこで開いても大差はありませんが、多くの方々は<a href="">SBI証券</a>、<a href="">楽天証券</a>、<a href="">マネックス証券</a>あたりで口座を開いているかと思います。</p>
          <p>なのでまずはご自身でそれぞれの証券会社のページに行き、証券口座の申し込み手続きをしましょう。</p>
          <hr class="my-3">
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/howtopurchase"
          >
            次へ
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>

export default {
  components: {
  }
}
</script>
