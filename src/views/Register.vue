<template>
  <div
    class="h-screen flex m-auto justify-center items-center overflow-y-hidden max-w-7xl"
  >
    <section class="px-10 flex flex-col md:w-[70%] lg:w-[50%] lg:max-w-lg m-auto">
      <section>
        <p class="text-gray-400">Start for free</p>
        <h1 class="text-4xl font-medium">Create new account</h1>
      </section>

      <form action="" class="pt-10 flex flex-col">

        <section class="flex justify-between mb-5">
          <Input placeHolder="first name" type="text" class="w-[48%]" />
          <Input placeHolder="last name" type="text" class="w-[48%]"/>
        </section>
        
        <Input placeHolder="email" type="text" class="mb-5"/>
        <Input placeHolder="password" type="password"/>

        <section
          class="flex justify-center items-center mt-10 text-gray-400 text-sm"
        >
          <input type="checkbox" name="" id="" class="mr-3" />
          <p>I accept terms & condition</p>
        </section>

        <button class="py-3 rounded-lg bg-blue-500 text-white mt-10">
          Login
        </button>
      </form>
    
      <p class="text-center mt-10 text-gray-400">already have an account? <router-link to="/" class="text-blue-500 underline">Login</router-link></p>
    </section>

    <div class="hidden lg:flex h-screen w-[50%]">
      <img src="/images/register.jpg" alt="" class="object-cover w-full" />
    </div>

  </div>
</template>

<script>

import Input from '../components/Input.vue'

export default {
  name: "Register-page",

  components: {
      Input
  }
};
</script>
