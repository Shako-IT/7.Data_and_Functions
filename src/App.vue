<template>
  <h2>My Course Goal</h2>
  <!-- Task 1: Output your main course goal with help of the composition API -->
  <!-- Don't hardcode it into the template, instead hardcode it into the JS code -->
  <h3 v-if="visibility">{{ goal }}</h3>
  <!-- Task 2: Toggle (show/ hide) the goal with help of the button  -->
  <button @click="toggleVisibility">Toggle Goal</button>
  <!-- Task 3: Manage data in three ways -->
  <!-- => Separate refs -->
  <!-- => Ref Object -->
  <!-- => Reactive Object -->
  <!-- Task 4: Also solve the assignment with the Options API -->
</template>

<script>
// import { ref } from 'vue';
// import { reactive } from 'vue';

export default {
  data() {
    return {
      goal: 'Learn Vue',
      visibility: false,
    };
  },
  methods: {
    toggleVisibility() {
      this.visibility = !this.visibility;
    },
  },
  // setup() {
  //   // const coursGoal = ref('Learn Vue');
  //   // const visible = ref(false);
  //   // const coursData = ref({
  //   //   goal: 'Learn Vue',
  //   //   visibility: false,
  //   // });
  //   const coursData = reactive({
  //     goal: 'Learn Vue',
  //     visibility: false,
  //   });
  //   function toggleVisibility() {
  //     // visible.value = !visible.value;
  //     // coursData.value.visibility = !coursData.value.visibility;
  //     coursData.visibility = !coursData.visibility;
  //   }
  //   return {
  //     // goal: coursData.value.goal,
  //     goal: coursData.goal,
  //     // visible: visible,
  //     coursData: coursData,
  //     toggleVisibility: toggleVisibility,
  //   };
  // },
};
</script>

<style>
html {
  font-family: sans-serif;
}
body {
  margin: 3rem;
  text-align: center;
}
</style>
