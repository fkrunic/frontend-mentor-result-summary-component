<script setup lang="ts">
</script>

<template>
  <div class="flex flex-col justify-start items-center min-h-screen">

    <!-- Card -->
    <div class="flex flex-col">

      <!-- Banner -->
      <div class="
        flex 
        flex-col 
        items-center

        bg-gradient-to-b from-light-slate-blue to-light-royal-blue
        ">


        <p class="font-bold text-light-lavender">Your Result</p>

        <!-- Score Callout -->
        <div class="
          flex 
          flex-col 
          items-center
          
          bg-gradient-to-b from-violet-blue to-persian-blue
          
          ">
          <p>76</p>
          <p>of 100</p>
        </div>

        <div class="flex flex-col items-center">
          <p>Great</p>
          <p>
            You scored higher than 65% of the people who have taken these tests.
          </p>        
        </div>
      </div>

      <!-- Content -->
      <div class="flex flex-col">
        <p>Summary</p>

        <!-- Scores -->
        <div>
          
          <!-- Reaction Score -->
          <div class="flex flex-row">
            <div class="flex flex-row">
              <img src="./assets/img/icon-reaction.svg" alt="reaction">
              <p>Reaction</p>
            </div>
            <div class="flex flex-row">
              <p>80</p>
              <p>/ 100</p>
            </div>
          </div>

          <!-- Memory Score -->
          <div class="flex flex-row">
            <div class="flex flex-row">
              <img src="./assets/img/icon-memory.svg" alt="memory">
              <p>Memory</p>
            </div>
            <div class="flex flex-row">
              <p>92</p>
              <p>/ 100</p>
            </div>
          </div>
          
          <!-- Verbal Score -->
          <div class="flex flex-row">
            <div class="flex flex-row">
              <img src="./assets/img/icon-verbal.svg" alt="verbal">
              <p>Verbal</p>
            </div>
            <div class="flex flex-row">
              <p>61</p>
              <p>/ 100</p>
            </div>
          </div>
          
          <!-- Visual Score -->
          <div class="flex flex-row">
            <div class="flex flex-row">
              <img src="./assets/img/icon-visual.svg" alt="visual">
              <p>Visual</p>
            </div>
            <div class="flex flex-row">
              <p>72</p>
              <p>/ 100</p>
            </div>
          </div>        

        </div>

        <!-- Button -->
        <div class="bg-dark-gray-blue">
          <p class="text-pale-blue">Continue</p>
        </div>

      </div>

    </div>
  </div>

</template>

<style scoped>
* {
  box-sizing: border-box;
}
</style>

<script lang="ts">
export default {
  data() {
    return {
      bodyClass: 'font-hanken-grotesk'
    };
  },
  mounted() {
    document.body.className = this.bodyClass;
  },
  beforeDestroy() {
    // Reset the class when the component is destroyed
    document.body.className = '';
  }
};
</script>