<template>
    <footer class="relative pt-8 pb-6 bg-blueGray-200">
        <div
            class="absolute top-0 left-0 right-0 bottom-auto w-full h-20 -mt-20 overflow-hidden pointer-events-none"
            style="transform: translateZ(0);"
        >
            <svg
                class="absolute bottom-0 overflow-hidden"
                xmlns="http://www.w3.org/2000/svg"
                preserveAspectRatio="none"
                version="1.1"
                viewBox="0 0 2560 100" 
                x="0"
                y="0"
            >
                <polygon
                    class="fill-current text-blueGray-200"
                    points="2560 0 2560 100 0 100"
                ></polygon>
            </svg>
        </div>
        <div class="container px-4 mx-auto">
            <div class="flex flex-wrap text-center lg:text-left">
                <div class="w-full px-4 lg:w-6/12">
                    <h4 class="text-3xl font-semibold">Let's keep in touch!</h4>
                    <h5 class="mt-0 mb-2 text-lg text-blueGray-600">
                        Find me on any of these platforms, I respond 1-2 business days.
                    </h5>
                    <div class="mt-6 mb-6 lg:mb-0">
<!--                        <button-->
<!--                            class="items-center justify-center w-10 h-10 mr-2 font-normal bg-white rounded-full shadow-lg outline-none text-lightBlue-400 align-center focus:outline-none"-->
<!--                            type="button"-->
<!--                        >-->
<!--                            <i class="fab fa-twitter"></i>-->
<!--                        </button>-->
<!--                        <button-->
<!--                            class="items-center justify-center w-10 h-10 mr-2 font-normal bg-white rounded-full shadow-lg outline-none text-lightBlue-600 align-center focus:outline-none"-->
<!--                            type="button"-->
<!--                        >-->
<!--                            <i class="fab fa-facebook-square"></i>-->
<!--                        </button>-->
                        <button
                            class="items-center justify-center w-10 h-10 mr-2 font-normal text-blue-500 bg-white rounded-full shadow-lg outline-none align-center focus:outline-none"
                            type="button"
                            onclick="window.open('https://https://www.linkedin.com/in/ten-sokheng-255014369/', '_blank')"
                        >
                            <i class="fab fa-linkedin"></i>
                        </button>
                        <button
                            class="items-center justify-center w-10 h-10 mr-2 font-normal bg-white rounded-full shadow-lg outline-none text-blueGray-800 align-center focus:outline-none"
                            type="button"
                               onclick="window.open('https://github.com/HengJr10', '_blank')"
                        >
                            <i class="fab fa-github"></i>
                        </button>
                    </div>
                </div>
                <div class="w-full px-4 lg:w-6/12">
                    <div class="flex flex-wrap mb-6 items-top">
                        <div class="w-full px-4 ml-auto lg:w-4/12">
              <span
                  class="block mb-2 text-sm font-semibold uppercase text-blueGray-500"
              >
                Useful Links
              </span>
                            <ul class="list-unstyled">
                                <li>
                                    <a
                                        class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800"
                                        href="#"
                                    >
                                        About Us
                                    </a>
                                </li>
                                <li>
                                    <a
                                        class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800"
                                        href="#"
                                    >
                                        Blog
                                    </a>
                                </li>
                                <li>
                                    <a
                                        class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800"
                                        href="#"
                                    >
                                        Github
                                    </a>
                                </li>
                                <li>
                                    <a
                                        class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800"
                                        href="#"
                                    >
                                        Free Products
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="w-full px-4 lg:w-4/12">
              <span
                  class="block mb-2 text-sm font-semibold uppercase text-blueGray-500"
              >
                Other Resources
              </span>
                            <ul class="list-unstyled">
                                <li>
                                    <Link :href="route('login')"
                                          class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800">
                                        Login
                                    </Link>
                                </li>
                                <li>
                                    <Link :href="route('register')"
                                          class="block pb-2 text-sm font-semibold text-blueGray-600 hover:text-blueGray-800">
                                        Create new account
                                    </Link>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <hr class="my-6 border-blueGray-300"/>
            <div
                class="flex flex-wrap items-center justify-center md:justify-between"
            >
                <div class="w-full px-4 mx-auto text-center md:w-4/12">
                    <div class="py-1 text-sm font-semibold text-blueGray-500">
                        Copyright © {{ date }}
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<script>
import {Link} from "@inertiajs/vue3";

export default {
    components: {Link},
    data() {
        return {
            date: new Date().getFullYear(),
        };
    },
};
</script>
