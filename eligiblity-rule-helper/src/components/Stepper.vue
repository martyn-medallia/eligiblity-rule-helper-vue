<template>
<v-stepper v-model="question" vertical>

    <v-stepper-step :complete="question > 1" step="1">What do you want to do</v-stepper-step>
    <v-stepper-content step="1">
      <v-btn color="primary" @click="question = 2; answer1 = 'eligibility'">Create an Eligibility Rule</v-btn>
      <v-btn color="primary" @click="question = 2; answer1 = 'usecase'">Create a Usecse</v-btn>
    </v-stepper-content>


    <v-stepper-step :complete="question > 2" v-if="answer1 = 'eligibility'" step="2">Configure analytics for this app</v-stepper-step>
    <v-stepper-content step="2">
      <v-btn color="primary" @click="question = 3">Continue</v-btn>
      <v-btn color="primary" @click="question = 3">Continue</v-btn>
    </v-stepper-content>


    
  </v-stepper>
</template>

<script>
export default {
  data: () => ({
    question: 1,
    answer1: null,
  }),
}
</script>