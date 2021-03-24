<template>
  <v-stepper
    v-model="e6"
    vertical
  >
    <v-stepper-step
      :complete="e6 > 1"
      color=#C42061
      step="1"
    >
      Step 1
      <small>Full name</small>
    </v-stepper-step>

    <v-stepper-content step="1">
      <v-card
      
        
      ><Step1/></v-card>
      <v-btn
        color=#C42061
        @click="e6 = 2"
      >
        Continue
      </v-btn>
      
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 2"
      color=#C42061
      step="2"
    >
     Step 2
     <small>Email</small>
    </v-stepper-step>

    <v-stepper-content step="2">
      <v-card
        
      ><Step2/></v-card>
      <v-btn
        color=#C42061
        @click="e6 = 3"
      >
        Continue
      </v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 3"
      color=#C42061
      step="3"
    >
      Step 3
    <small>About myself</small>
    </v-stepper-step>

    <v-stepper-content step="3">
      <v-card
      ><Step3/></v-card>
      <v-btn
        color=#C42061
        @click="e6 = 4"
      >
        Continue
      </v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 4"
      color=#C42061
      step="4"
    >
      Step 4
      <small>For you</small>
    </v-stepper-step>
    <v-stepper-content step="4">
      <v-card
      ><Step4/></v-card>
      <v-btn
        color=#C42061
        @click="e6 = 1"
      >
       Start over
      </v-btn>
    </v-stepper-content>
  </v-stepper>
</template>

<script>
import Step1 from './Step1.vue'
import Step2 from './Step2.vue'
import Step3 from './Step3.vue'
import Step4 from './Step4.vue'
  export default {
      components: {
    Step1,
    Step2,
    Step3,
    Step4,
  },
    data () {
      return {
        e6: 1,
      }
    },
  }
</script>
<style scoped>
.card{
    margin: 10% 10%;
    padding: 5% ;
    
}
</style>