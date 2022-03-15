<template>
  <div
    class="h-screen flex m-auto justify-center items-center overflow-y-hidden"
  >
    <div class="hidden lg:flex h-screen w-[50%]">
      <img src="/images/login.jpg" alt="" class="object-cover w-full" />
    </div>

    <section class="px-10 flex flex-col md:w-[70%] lg:w-[50%] lg:max-w-lg m-auto">
      <section>
        <h1 class="text-4xl font-medium">Welcome Back</h1>
        <p class="text-gray-400">let's continue with us</p>
      </section>

      <form action="" class="pt-10 flex flex-col">
        <Input placeHolder="email" type="text" class="mb-5"/>
        <Input placeHolder="password" type="password"/>

        <section
          class="flex justify-between items-center mt-10 text-gray-400 text-sm"
        >
          <section class="flex justify-center items-center">
            <input type="checkbox" name="" id="" class="mr-2" />
            <p>keep me logged in</p>
          </section>

          <p class="cursor-pointer hover:text-blue-500 hover:underline">Forgot Password?</p>
        </section>

        <button class="py-3 rounded-lg bg-blue-500 text-white mt-10">
          Login
        </button>

        <button class="py-3 rounded-lg  mt-4 flex justify-center items-center font-medium border border-gray-300 shadow-md" >
          <img src="/images/linkedin-logo.png" alt="linkedin logo" class="w-[25px] h-[25px] mr-3">
          Sign in with Linkedin 
        </button>

      </form>
      <p class="text-center text-gray-400 mt-10">doesn't have an account? <router-link to="/register" class="text-blue-500 underline">Register</router-link></p>
    </section>

  </div>
</template>

<script>

import Input from '../components/Input.vue'

export default {
  name: "Login-page",

  components: {
    Input
  }
};
</script>
