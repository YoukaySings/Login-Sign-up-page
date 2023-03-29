<template>
  <div
    class="h-screen w-full md:grid md:grid-cols-3 flex flex-col justify-center items-center"
  >
    <div
      class="hidden md:block relative md:col-span-2 bg-[url('/firstpage-img.jpg')] bg-cover"
    >
      <div class="bg-[#002864d2] w-full h-screen p-20">
        <!-- company logo -->
        <div class="z-40 bg-white inline-block p-3 text-[#333]">
          <img src="" alt="company-logo" />
        </div>

        <!-- text -->
        <div class="z-40">
          <h2 class="large-header leading-[60px] mt-4">Company name</h2>
          <h4 class="medium-header mt-5">Information title</h4>
          <br />
          <p class="w-8/12">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos in
            dolore, fugiat voluptate ipsam neque, consequuntur ullam voluptas
            soluta, non cumque. Libero, ab porro. Amet debitis architecto
            dolorum beatae aperiam!
            <br />
            <br />
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius eos
            temporibus deleniti natus, at libero illo quisquam atque placeat
            voluptatum vel ratione modi debitis quam obcaecati. Sapiente labore
            quis expedita?
            <br />
            <br />
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore a
            sunt corrupti quis minus placeat ut, provident recusandae expedita
            deleniti nam rerum dolorum fuga, quo magnam, excepturi quaerat
            blanditiis error!
          </p>
          <br />
          <br />
          <br />
          <div class="flex items-center justify-between">
            <icon class="text-[40px]" name="uil:credit-card" />
            <icon class="w-10/12" name="uil:arrows-h" />
            <icon class="text-[40px]" name="uil:padlock" />
          </div>
        </div>
      </div>
    </div>

    <div class="flex flex-col justify-center items-center gap-4">
      <div
        class="z-40 rounded-md mb-20 bg-white text-[#333] inline-block p-3 md:hidden"
      >
        <img src="" alt="company-logo" />
      </div>
      <NuxtLink to="/signUpPage">
        <button class="login-btn">Sign up</button>
      </NuxtLink>
      <NuxtLink to="/signInPage">
        <button class="login-btn">Sign in</button>
      </NuxtLink>
    </div>
  </div>
</template>