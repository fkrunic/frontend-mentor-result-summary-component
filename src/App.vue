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

        py-8
        px-12
        gap-6

        bg-gradient-to-b from-light-slate-blue to-light-royal-blue

        rounded-bl-3xl
        rounded-br-3xl
        ">

        <p class="font-bold text-light-lavender">Your Result</p>

        <!-- Score Callout -->
        <div class="
          flex 
          flex-col 
          items-center

          p-8
          rounded-full
          
          bg-gradient-to-b from-violet-blue to-persian-blue          
          ">
          <p class="text-5xl text-white font-black">76</p>
          <p class="text-light-lavender/50 text-sm font-bold">of 100</p>
        </div>

        <!-- Assessment Callout -->
        <div class="flex flex-col items-center gap-2">
          <p class="text-white font-bold text-xl text-center">Great</p>
          <p class="text-light-lavender text-sm text-center">
            You scored higher than 65% of the people who have taken these tests.
          </p>        
        </div>
      </div>

      <!-- Content -->
      <div class="flex flex-col p-6 gap-6">
        <p class="font-black text-dark-gray-blue">Summary</p>

        <!-- Scores -->
        <div class="flex flex-col gap-4">
          
          <!-- Reaction Score -->
          <div class="
            flex 
            flex-row 
            justify-between 

            p-4
            
            bg-light-red/10 

            rounded-lg
            ">
            <div class="flex flex-row items-center gap-2">
              <img src="./assets/img/icon-reaction.svg" alt="reaction">
              <p class="font-bold text-light-red text-sm">Reaction</p>
            </div>
            <div class="flex flex-row gap-1">
              <p class="font-black text-sm text-dark-gray-blue">80</p>
              <p class="font-black text-sm text-dark-gray-blue/50">/ 100</p>
            </div>
          </div>

          <!-- Memory Score -->
          <div class="
            flex 
            flex-row 
            justify-between 

            p-4
            
            bg-orangey-yellow/10 
            
            rounded-lg
            ">
            <div class="flex flex-row items-center gap-2">
              <img src="./assets/img/icon-memory.svg" alt="memory">
              <p class="font-bold text-orangey-yellow text-sm">Memory</p>
            </div>
            <div class="flex flex-row gap-1">
              <p class="font-black text-sm text-dark-gray-blue">92</p>
              <p class="font-black text-sm text-dark-gray-blue/50">/ 100</p>
            </div>
          </div>
          
          <!-- Verbal Score -->
          <div class="
            flex 
            flex-row 
            justify-between
            
            p-4
            
            bg-green-teal/10 
            
            rounded-lg
            ">
            <div class="flex flex-row items-center gap-2">
              <img src="./assets/img/icon-verbal.svg" alt="verbal">
              <p class="font-bold text-green-teal text-sm">Verbal</p>
            </div>
            <div class="flex flex-row gap-1">
              <p class="font-black text-sm text-dark-gray-blue">61</p>
              <p class="font-black text-sm text-dark-gray-blue/50">/ 100</p>
            </div>
          </div>
          
          <!-- Visual Score -->
          <div class="
            flex 
            flex-row 
            justify-between 

            p-4
            
            bg-cobalt-blue/10 
            
            rounded-lg
            ">
            <div class="flex flex-row items-center gap-2">
              <img src="./assets/img/icon-visual.svg" alt="visual">
              <p class="font-bold text-cobalt-blue text-sm">Visual</p>
            </div>
            <div class="flex flex-row gap-1">
              <p class="font-black text-sm text-dark-gray-blue">72</p>
              <p class="font-black text-sm text-dark-gray-blue/50">/ 100</p>
            </div>
          </div>        

        </div>

        <!-- Button -->
        <div class="
          flex 
          flex-row 
          justify-center 

          p-4

          rounded-full
          
          bg-dark-gray-blue

          hover:bg-gradient-to-b from-light-slate-blue to-light-royal-blue
          hover:cursor-pointer
          ">
          <p class="text-pale-blue font-bold">Continue</p>
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