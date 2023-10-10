<template>
    <main class="mx-auto font-[mulish] items-center">
        <div class="max-w-screen-2xl items-center mx-auto">
            <nav class="flex justify-between mt-4 mx-4">
                <div class="md:hidden gap-x-4 flex items-center">
                    <!-- <div className="dropdown dropdown-bottom">
                        <label tabIndex={0}><i class="fa fa-bars fa-lg"></i></label>
                        <ul tabIndex={0} className="dropdown-content z-[1] menu p-2 mt-8 shadow bg-base-100 rounded-box w-52">
                            <li><a>Item 1</a></li>
                            <li><a>Item 2</a></li>
                        </ul>
                    </div> -->
                    <dropdown />
                    <img class="w-auto h-6" :src="Logo" alt="">
                </div>

            <ul class="md:flex hidden xl:gap-x-12 gap-x-8 lg:gap-x-6 text-sm items-center font-bold">
                <li><img class="w-auto h-6" :src="Logo" alt=""></li>
                <li>Find Talent</li>
                <li>Find Work</li>
                <li>Why Upwork</li>
                <li>Enterprise</li>
            </ul>
            <div class="flex gap-x-4 items-center">
                <div class="lg:flex hidden border rounded-full items-center">
                    <div class="flex items-center ml-4 gap-x-3">
                        <i class="fa fa-search"></i>
                        <input class="focus:outline-none text-base" type="text" placeholder="search" name="search" id="search">
                    </div>
                    <select class="select select-ghost select-sm w-full max-w-xs text-base focus:outline-none">
                        <option disabled selected>Talent</option>
                        <option>Svelte</option>
                        <option>Vue</option>
                        <option>React</option>
                    </select>
                </div>
                <div class="flex items-center gap-x-6 md:flex-row flex-row-reverse">
                    <div className="lg:hidden dropdown dropdown-end">
                    <label tabIndex={0}><i class="fa fa-search"></i></label>
                    <ul tabIndex={0} className="dropdown-content z-[1] menu p-2 mt-8 shadow bg-base-100 rounded-box w-52">
                        <li><a>Item 1</a></li>
                        <li><a>Item 2</a></li>
                    </ul>
                    </div>
                    <div class="flex gap-x-4">
                        <button class="md:block hidden">login</button>
                        <button class="md:bg-primary bg-white h-12 rounded-full w-24 md:text-white text-black">Sign Up</button>
                    </div>
                </div>
            </div>
        </nav>
        <hr class="my-4 absolute left-0 right-0">
        <nav class="mx-4 lg:flex hidden">
            <ul class="flex gap-x-5 text-sm font-bold mt-8">
                <li>Development & IT</li>
                <li>AI Services</li>
                <li>Design & Creative</li>
                <li>Sales & Marketing</li>
                <li>Admin & Customer Support</li>
                <li>More</li>
            </ul>
        </nav>
        <section class="flex items-center justify-around mt-12 mx-8">
            <div class="flex flex-col gap-y-12">
                <h1 class="xl:text-[100px] lg:text-[80px] md:text-[60px] text-primary font-bold text-[50px] font-serif leading-tight">How work<br/>should work</h1>
                <h2 class="xl:text-2xl md:text-lg sm:text-sm font-semibold">Forget the old rules. You can have the best people.<br />Right now. Right here.</h2>
                <button class="bg-primary text-white py-2 px-4 w-fit rounded-full hover:bg-green-700 font-bold">Get Started</button>
                <div>
                    <h3 class="my-2">Trusted by</h3>
                    <div class="flex gap-x-12">
                        <img :src="Image3" alt="">
                        <img :src="Image4" alt="">
                        <img :src="Image5" alt="">
                    </div>
                </div>
            </div>
            <div>
                <img class="xl:w-[500px] lg:w-[400px] md:w-[400px] md:flex hidden h-auto" :src="Image2" alt="">
            </div>  
        </section>
        </div>
        <footer class=" bg-green-950 w-full mt-32 rounded-lg">
            <div class="flex text-white py-16 text-sm justify-evenly leading-7 md:flex-row flex-col mx-12 gap-y-8">
                <ul>
                    <li class="font-bold my-2">For Clients</li>
                    <li>How to Hire</li>
                    <li>Talent Marketplace</li> 
                    <li>Project Catalog</li>
                    <li>Hire an Agency</li>
                    <li>Enterprise</li> 
                    <li>Any Hire</li>
                    <li>Contract-to-Hire</li>
                    <li>Direct Contracts</li>
                    <li>Hire Worldwide</li>
                    <li>Hire in the USA</li>  
                </ul>
                <ul>
                    <li class="font-bold my-2">For Talent</li>
                    <li>How to Find Work</li>
                    <li>Direct Contracts</li>
                    <li>Find Freelance Jobs Worldwide</li>
                    <li>Find Freelance Jobs in the USA</li>
                </ul>
                <ul>
                    <li class="font-bold my-2">Resources</li>
                    <li>Help & Support</li>
                    <li>Success Stories</li>
                    <li>Upwork Reviews</li>
                    <li>Resources</li>
                    <li>Blog</li> 
                    <li>Community</li>
                    <li>Affiliate Program</li>
                    <li>Free Business tools</li>
                </ul>
                <ul>
                    <li class="font-bold my-2">Company</li>
                    <li>About Us</li>
                    <li>Leadership</li>
                    <li>Investor Relations</li>
                    <li>Careers</li>
                    <li>Our Impact</li> 
                    <li>Press</li>
                    <li>Contact Us</li>
                    <li>Trust, Safety & Security</li>
                    <li>Modern Slavery Statement</li>  
                </ul>
            </div>
        </footer>
    </main>
</template>

<script setup>
import Logo from "../assets/Upwork_Logo.svg";
import Image2 from "../assets/use.webp";
import Image3 from "../assets/airbnb.svg";
import Image4 from "../assets/microsoft.svg"
import Image5 from "../assets/bissell.svg"
import 'font-awesome/css/font-awesome.min.css';
import dropdown from '../components/dropdown.vue';
</script>
