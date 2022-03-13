<template>
  <div
    class="h-screen flex m-auto justify-center items-center overflow-y-hidden"
  >
    <div class="hidden lg:flex w-[50%] h-screen">
      <img src="/images/register.jpg" alt="" class="object-cover" />
    </div>

    <section class="px-10 flex flex-col md:w-[70%] lg:w-[50%] lg:max-w-lg m-auto">
      <section>
        <h1 class="text-4xl font-medium">Welcome Back</h1>
        <p class="text-gray-400">let's continue with us</p>
      </section>

      <form action="" class="pt-10 flex flex-col">
        <input
          type="text"
          class="px-6 py-3 bg-blue-50 rounded-lg mb-5 outline-none"
          placeholder="email"
        />
        <input
          type="password"
          class="px-6 py-3 bg-blue-50 rounded-lg outline-none"
          placeholder="password"
        />

        <section
          class="flex justify-center items-center mt-10 text-gray-400 text-sm"
        >
          <input type="checkbox" name="" id="" class="mr-3" />
          <p>Remember me</p>
        </section>

        <button class="py-3 rounded-lg bg-blue-500 text-white mt-10">
          Login
        </button>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  name: "Login-page",
};
</script>
