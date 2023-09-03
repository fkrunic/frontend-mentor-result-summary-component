<script setup lang="ts">
</script>

<template>
  <div class="
    flex 
    flex-col 
    justify-start 
    items-center 
    min-h-screen

    desktop:justify-center
    ">

    <!-- Card -->
    <div class="
      flex 
      flex-col
      
      desktop:flex-row
      desktop:rounded-3xl
      
      desktop:bg-white

      desktop:shadow-xl 
      desktop:shadow-cobalt-blue/10
      ">

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

        desktop:w-96
        desktop:p-16
        desktop:pt-10

        desktop:rounded-3xl
        ">

        <p class="font-bold text-light-lavender desktop:text-2xl">Your Result</p>

        <!-- Score Callout -->
        <div class="
          flex 
          flex-col 
          items-center

          p-8
          rounded-full
          
          bg-gradient-to-b from-violet-blue to-persian-blue       
          
          desktop:p-14
          ">
          <p class="text-5xl text-white font-black desktop:text-6xl">76</p>
          <p class="text-light-lavender/50 text-sm font-bold desktop:text-base">of 100</p>
        </div>

        <!-- Assessment Callout -->
        <div class="flex flex-col items-center gap-2 desktop:gap-4">
          <p class="text-white font-bold text-xl text-center desktop:text-3xl">Great</p>
          <p class="text-light-lavender text-sm text-center desktop:text-base">
            You scored higher than 65% of the people who have taken these tests.
          </p>        
        </div>
      </div>

      <!-- Content -->
      <div class="
        flex 
        flex-col 
        gap-6
        p-6 

        desktop:w-96
        desktop:gap-8
        desktop:p-10
        
        ">
        <p class="font-black text-dark-gray-blue desktop:text-2xl">Summary</p>

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
              <p class="font-bold text-light-red text-sm desktop:text-base">Reaction</p>
            </div>
            <div class="flex flex-row gap-1 desktop:gap-2">
              <p class="font-black text-sm text-dark-gray-blue desktop:text-base desktop:font-bold">80</p>
              <p class="font-black text-sm text-dark-gray-blue/50 desktop:text-base desktop:font-bold">/ 100</p>
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
              <p class="font-bold text-orangey-yellow text-sm desktop:text-base">Memory</p>
            </div>
            <div class="flex flex-row gap-1 desktop:gap-2">
              <p class="font-black text-sm text-dark-gray-blue desktop:text-base desktop:font-bold">92</p>
              <p class="font-black text-sm text-dark-gray-blue/50 desktop:text-base desktop:font-bold">/ 100</p>
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
              <p class="font-bold text-green-teal text-sm desktop:text-base">Verbal</p>
            </div>
            <div class="flex flex-row gap-1 desktop:gap-2">
              <p class="font-black text-sm text-dark-gray-blue desktop:text-base desktop:font-bold">61</p>
              <p class="font-black text-sm text-dark-gray-blue/50 desktop:text-base desktop:font-bold">/ 100</p>
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
              <p class="font-bold text-cobalt-blue text-sm desktop:text-base">Visual</p>
            </div>
            <div class="flex flex-row gap-1 desktop:gap-2">
              <p class="font-black text-sm text-dark-gray-blue desktop:text-base desktop:font-bold">72</p>
              <p class="font-black text-sm text-dark-gray-blue/50 desktop:text-base desktop:font-bold">/ 100</p>
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
      bodyClass: 'font-hanken-grotesk desktop:bg-pale-blue'
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