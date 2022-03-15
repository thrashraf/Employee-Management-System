
<template>
    <div class="flex flex-no-wrap bg-gray-200 h-screen">
        <div class="w-64 absolute sm:relative bg-gray-800 shadow md:h-full flex-col justify-between hidden sm:flex">
            <div class="px-8">
                <div class="h-16 w-full flex items-center">
                    <!-- logo -->
                </div>
                <ul class="mt-12">
                    <li class="flex w-full justify-between text-gray-300 hover:text-gray-500 cursor-pointer items-center mb-6">
                        <div class="flex items-center">
                            <img src="/images/dashboard.svg" alt="dashboard" class="fill-gray-300">
                            <span class="text-sm ml-2">Dashboard</span>
                        </div>
                        <div class="py-1 px-3 bg-gray-700 rounded text-gray-500 flex items-center justify-center text-xs">5</div>
                    </li>
                    <li class="flex w-full justify-between text-gray-600 hover:text-gray-500 cursor-pointer items-center mb-6">
                        <div class="flex items-center">
                            <img src="/images/product.svg" alt="">
                            <span class="text-sm ml-2">Products</span>
                        </div>
                        <div class="py-1 px-3 bg-gray-700 rounded text-gray-500 flex items-center justify-center text-xs">8</div>
                    </li>
                    <li class="flex w-full justify-between text-gray-600 hover:text-gray-500 cursor-pointer items-center mb-6">
                        <div class="flex items-center">
                            <img src="/images/performance.svg" alt="performance">
                            <span class="text-sm ml-2">Performance</span>
                        </div>
                    </li>

                </ul>
                <div class="flex justify-center mt-48 mb-4 w-full">
                    <div class="relative">
                        <div class="text-gray-500 absolute ml-4 inset-0 m-auto w-4 h-4">
                            <img src="/images/search.svg" alt="">
                        </div>
                        <input class="bg-gray-700 focus:outline-none rounded w-full text-sm text-gray-500  pl-10 py-2" type="text" placeholder="Search" />
                    </div>
                </div>
            </div>
            <div class="px-8 border-t border-gray-700">
                <ul class="w-full flex items-center justify-between bg-gray-800">
                    <li class="cursor-pointer text-white pt-5 pb-3">
                        <img src="/images/notification.svg" alt="">
                    </li>
                    <li class="cursor-pointer text-white pt-5 pb-3">
                        <img src="/images/setting.svg" alt="">
                    </li>
                    <li class="cursor-pointer text-white pt-5 pb-3">
                        <img src="/images/archive.svg" alt="">
                    </li>
                    <li class="cursor-pointer text-white pt-5 pb-3">
                        <img src="/images/logout.svg" alt="" class="w-[20px]">
                    </li>
                </ul>
            </div>
        </div>
        <!-- Sidebar ends -->
        <!-- Remove class [ h-64 ] when adding a card block -->
        <div class="container mx-auto py-10 h-64 md:w-4/5 w-11/12 px-6">
            <!-- Remove class [ border-dashed border-2 border-gray-300 ] to remove dotted border -->
            <div class="w-full h-full rounded border-dashed border-2 border-gray-300">
                <!-- Place your content here -->
            </div>
        </div>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Home",
    data() {
        return {
            moved: true,
        };
    },
    methods: {
        sidebarHandler() {
            var sideBar = document.getElementById("mobile-nav");
            sideBar.style.transform = "translateX(-260px)";
            if (this.$data.moved) {
                sideBar.style.transform = "translateX(0px)";
                this.$data.moved = false;
            } else {
                sideBar.style.transform = "translateX(-260px)";
                this.$data.moved = true;
            }
        },
    },
};
</script>