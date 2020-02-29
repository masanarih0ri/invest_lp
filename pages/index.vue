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
      <!-- <h1 class="display-2 text-center mb-8">配当金ツール</h1> -->
      <v-card class="mb-6 pa-8">
        <v-card-title class="headline">
          データを入力してください
        </v-card-title>
        <v-form
          ref="form"
          v-model="valid"
          :lazy-validation="lazy"
        >
          <v-text-field
            v-model="name"
            :counter="20"
            :rules="nameRules"
            label="Name"
            required
          ></v-text-field>
          <v-text-field
          v-model.number="nowStockPrice"
          label="現在株価"
        ></v-text-field>
        <v-text-field
          v-model.number="yield1"
          label="配当金1"
        ></v-text-field>
        <v-text-field
          v-model.number="yield2"
          label="配当金2"
        ></v-text-field>
        <v-text-field
          v-model.number="yield3"
          label="配当金3"
        ></v-text-field>
        <v-text-field
          v-model.number="yield4"
          label="配当金4"
        ></v-text-field>
        </v-form>
      </v-card>
      <v-card>
        <v-card-title class="headline">
          計算結果
        </v-card-title>
        <v-card-text>
          {{ calcYield }}%
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>

export default {
  components: {
  },
  data: function() {
    return {
      name: '',
      nowStockPrice: 0,
      yield1: 0,
      yield2: 0,
      yield3: 0,
      yield4: 0,
      valid: true,
      nameRules: [
        v => !!v || 'Name is required',
        v => (v && v.length <= 20) || 'Name must be less than 10 characters',
      ],
      lazy: false
    }
  },
  computed: {
    calcYield() {
      return (this.yield1 + this.yield2 + this.yield3 + this.yield4) / this.nowStockPrice * 100 || 0;
    },

    plus() {
      return this.yield1 + this.yield2 + this.yield3 + this.yield4;
    }
  }
}
</script>
