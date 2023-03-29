<template>
  <div class="h-auto md:p-5 w-full">
    <!-- side bar call button -->
    <div
      @click="dashboard()"
      class="md:hidden fixed right-[20px] bottom-[40px] w-10 h-10 bg-black flex justify-center items-center"
    >
      <icon class="text-[30px]" name="uil:create-dashboard" />
    </div>

    <div class="flex w-full h-full">
      <!-- side bar -->
      <div
        id="side-bar"
        class="fixed left-[-1000px] md:sticky w-full md:w-auto"
      >
        <NuxtLink to="/">
          <navigation />
        </NuxtLink>
        <side-bar @close-sidebar="closedashboard()" />
      </div>
      <!-- dashboard content -->
      <div class="flex flex-col w-full">
        <div class="flex flex-col lg:flex-row items-start">
          <db-personal-info />
          <amount />
        </div>
        <div>
          <db-cards />
        </div>
        <div>
          <transactions />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    methods: {
      dashboard(){
        document.getElementById('side-bar').style.left = '0px'
      },
      closedashboard(){
        document.getElementById('side-bar').style.left = '-1000px'
      }
    }
}
</script>