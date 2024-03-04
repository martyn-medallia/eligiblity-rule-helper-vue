<template>
  <v-card class="mx-auto" max-width="80%">
    <v-card-text>
      <p class="text-h4 text--primary">
        Question 1
      </p>
      <div class="text--primary">
        Pick an answer
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn variant="text" color="teal-accent-4" @click="reveal = 'a1'">
        Answer 1
      </v-btn>
      <v-btn variant="text" color="teal-accent-4" @click="reveal = 'a2'">
        Answer 2
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card v-if="reveal === 'a1'" class="v-card--reveal" style="height: 100%;">
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Origin
          </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn variant="text" color="teal-accent-4" @click="reveal = false">
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
      <v-card v-if="reveal === 'a2'" class="v-card--reveal" style="height: 100%;">
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Origin
          </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn variant="text" color="teal-accent-4" @click="reveal = false">
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    reveal: false,
  }),
}
</script>