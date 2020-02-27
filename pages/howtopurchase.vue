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
          株の買い方（用語編）
        </v-card-title>
        <v-card-text class="subtitle-1">
          <p>証券口座を開いてお金を入金したら、いつでも株を購入することができます。</p>
          <p>株には主に買い方は3つあり、一つは成行、もう一つは指値、もう一つは逆指値というものがあります。</p>
          <p>いきなり難しい用語が出てきましたが、成行は<span class="font-weight-bold">「すぐに買える」</span>、指値は<span class="font-weight-bold">「自分で値段を決めて買える（売れる）」</span>、逆指値は<span class="font-weight-bold">「自分で値段を決めて買える（売れる）」のですが、指値と全く逆の動作になる</span>、くらいに覚えておけばいいでしょう。</p>
          <p>もう少し具体的な例を見てみましょう。株が1000円で売買できるようになった時に、成行注文を出したとします。そうすると1000円で株価を買うことができます。</p>
          <p>指値注文は、「いやいや、もう少し安くなったら買いたいな。990円になったら買おう」という時に990円の指値をして、その金額に下がるまで待ち、購入します。</p>
          <p>逆指値の場合は「995円まで上昇（回復）してきたタイミングで買いたいな」と思った時に値段を設定して待ちます。</p>
          <p>指値と逆指値が少しわかりにくいのですが、指値で買う場合は「指定の金額を下回った場合は購入」逆指値の場合は「指定の金額を上回った場合は購入」ということになります。売る場合はその逆です。</p>
          <hr class="my-3">
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
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
