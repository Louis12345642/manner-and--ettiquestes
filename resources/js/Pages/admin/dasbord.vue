<script setup>
import layeoutVue from '@/Layouts/layeout.vue';
import { Link } from '@inertiajs/inertia-vue3'
import allPostsHeaderVue from '@/Components/hero-section/all-posts-header.vue';




</script>
<template>
<layeoutVue>
<allPostsHeaderVue title="Admin section"/>
<section class="grid grid-cols-1 lg:grid lg:grid-cols-3 gap-10 m-10 ">


<section>
    <div class="text-center h-20 card-bg title-width  mt-5 card-border rounded-t-md">
            <h1 class="font-bold font-mono text-center mt-6 text-3xl ">
     All articles
          </h1>
          </div>
    <section
          class="lg:card-bg card-border rounded-b-md card-bg lg:col-span-2 lg:row-span-2 shadow-md md:col-span-2 overflow-scroll max-heigth"
        >


          <section
            class="wrapper grid grid-cols-2 gap-5 mt-20 hover:bg-gray-200 cursor-pointer card-border m-4 rounded-bottom-lg"
          >
            <!-- image container -->

            <div class="m-2">
              <img
                class="rounded-lg card-border"
                src="side2.jpg"
                alt=""
              />
            </div>


            <Link href="/">
            <article class="mt-5">
              <p class="font-semibold leading-6 mb-4 text-sm">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, debitis.
              </p>

              <div class="flex gap-5 justify-left font-bold text-lg">
             <h1><i class='fa fa-edit    text-emerald-500'></i></h1>
             <h1><i class='fa fa-plus-circle' style='color:#3d25b1'></i></h1>
             <h1>
<i class='fa fa-trash' style='color: red'></i></h1>

            </div>
            </article>
            </Link>

          </section>

          <hr class="m-8" />
          <section
            class="wrapper grid grid-cols-2 gap-5 mt-20 hover:bg-gray-200 cursor-pointer card-border m-4 rounded-lg"
          >
            <!-- image container -->

            <div class="m-2">
              <img
                class="rounded-lg card-border"
                src="atomic.jpg"
                alt=""
              />
            </div>
            <Link href="/">
            <article class="mt-5">
              <p class="font-semibold leading-6 mb-4 text-sm">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, debitis.
              </p>
              <p class="mt-2 block text-gray-400 text-xs">

              </p>
              <div class="flex gap-5 justify-left font-bold text-lg">
             <h1><i class='fa fa-edit    text-emerald-500'></i></h1>
             <h1><i class='fa fa-plus-circle' style='color:#3d25b1'></i></h1>
             <h1>
<i class='fa fa-trash' style='color: red'></i></h1>

            </div>
            </article>
            </Link>
          </section>
          <hr class="m-8" />
          <section
            class="wrapper grid grid-cols-2 gap-5 mt-20 hover:bg-gray-200 cursor-pointer card-border m-4 rounded-lg"
          >
            <!-- image container -->

            <div class="m-2">
              <img
                class="rounded-lg card-border"
                src="logo.jpg"
                alt=""
              />
            </div>

            <Link href="/">
            <article class="mt-5">
              <p class="font-semibold leading-6 mb-4 text-sm">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, debitis.
              </p>

              <div class="flex gap-5 justify-left font-bold text-lg">
             <h1><i class='fa fa-edit    text-emerald-500'></i></h1>
             <h1><i class='fa fa-plus-circle' style='color:#3d25b1'></i></h1>
             <h1>
<i class='fa fa-trash' style='color: red'></i></h1>

            </div>
            </article>
            </Link>
          </section>
          <hr class="m-8" />
          <section
            class="wrapper grid grid-cols-2 gap-5 mt-20 hover:bg-gray-200 cursor-pointer card-border m-4 rounded-lg"
          >
            <!-- image container -->

            <div class="m-2">
              <img
                class="rounded-lg card-border"
                src="atomic-2.jpg"
                alt=""
              />
            </div>
            <Link href="/">
            <article class="mt-5">
              <p class="font-semibold leading-6 mb-4 text-sm">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, debitis.
              </p>
             <div class="flex gap-5 justify-left font-bold text-lg">
             <h1><i class='fa fa-edit    text-emerald-500'></i></h1>
             <h1><i class='fa fa-plus-circle' style='color:#3d25b1'></i></h1>
             <h1>
<i class='fa fa-trash' style='color: red'></i></h1>

            </div>

            </article>
            </Link>
          </section>
        </section>
</section>
<section class="lg:col-span-2">
    <div class=" p-5 my-4  card-bg card-border rounded-lg shadow-md h-70 hover:bg-gray-200 block">
            <!-- <img class="mx-auto mb-2"
                  src="/assets/icons/mailbox-icon.svg"
                  alt="mailbox letter"
                /> -->
                <h1 class="text-lg font-sans font-bold mt-3 text-center uppercase mb-3">create a new post</h1>
               <!-- <form @submit.prevent="submitData" class="p-5 py-3"> -->
                <label class="block my-3 font-mono font-bold" for="">Title</label>

                <input name="name" class="block my-3 input-width card-border rounded-md bg-slate-100 h-8 " type="text">
                <label for="countries" class="block mb-2  text-black font-bold">Select a category</label>
<select id="countries" class="bg-gray-100 border border-gray-300 text-black font-semibold text-md rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 ">
  <option selected>Choose a category</option>
  <option value="US">United States</option>
  <option value="CA">Canada</option>
  <option value="FR">France</option>
  <option value="DE">Germany</option>
  <option selected>Choose a category</option>
  <option value="US">United States</option>
  <option value="CA">Canada</option>
  <option value="FR">France</option>
  <option value="DE">Germany</option>
</select>

<label class="block my-3 font-mono font-bold" for="">Excerpt</label>
                <textarea  name="email" class="block my-3 input-width card-border rounded-md bg-slate-100 h-8" type="text"></textarea>
                <!--
                <label class="font-sans font-bold" for="">Body</label>
                <textarea name="message" class="block my-3 input-width bg-gray-100 card-border rounded-md active:border-purple-500"  ></textarea>

                <button type="submit" class="mt-4 px-4 py-1 text-sm text-purple-600 font-semibold rounded-full border border-purple-500 hover:text-white hover:bg-purple-600 hover:border-transparent focus:outline-none focus:ring-2 focus:ring-purple-600 focus:ring-offset-2 w-36">summit</button> -->
               <!-- </form> -->
        </div>
        <form>
   <div class="mb-4 w-full card-bg rounded-lg border border-gray-200 ">
       <div class="flex justify-between items-center py-2 px-3 border-b ">
           <div class="flex flex-wrap items-center divide-gray-200 sm:divide-x ">
               <div class="flex items-center space-x-1 sm:pr-4">
                   <button type="button" class="p-2 text-gray-900 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M8 4a3 3 0 00-3 3v4a5 5 0 0010 0V7a1 1 0 112 0v4a7 7 0 11-14 0V7a5 5 0 0110 0v4a3 3 0 11-6 0V7a1 1 0 012 0v4a1 1 0 102 0V7a3 3 0 00-3-3z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Attach file</span>
                   </button>
                   <button type="button" class="p-2 text-gray-00 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Embed map</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Upload image</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.316 3.051a1 1 0 01.633 1.265l-4 12a1 1 0 11-1.898-.632l4-12a1 1 0 011.265-.633zM5.707 6.293a1 1 0 010 1.414L3.414 10l2.293 2.293a1 1 0 11-1.414 1.414l-3-3a1 1 0 010-1.414l3-3a1 1 0 011.414 0zm8.586 0a1 1 0 011.414 0l3 3a1 1 0 010 1.414l-3 3a1 1 0 11-1.414-1.414L16.586 10l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                        <span class="sr-only">Format code</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM7 9a1 1 0 100-2 1 1 0 000 2zm7-1a1 1 0 11-2 0 1 1 0 012 0zm-.464 5.535a1 1 0 10-1.415-1.414 3 3 0 01-4.242 0 1 1 0 00-1.415 1.414 5 5 0 007.072 0z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Add emoji</span>
                   </button>
               </div>
               <div class="flex flex-wrap items-center space-x-1 sm:pl-4">
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 4a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zm0 4a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zm0 4a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zm0 4a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Add list</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M11.49 3.17c-.38-1.56-2.6-1.56-2.98 0a1.532 1.532 0 01-2.286.948c-1.372-.836-2.942.734-2.106 2.106.54.886.061 2.042-.947 2.287-1.561.379-1.561 2.6 0 2.978a1.532 1.532 0 01.947 2.287c-.836 1.372.734 2.942 2.106 2.106a1.532 1.532 0 012.287.947c.379 1.561 2.6 1.561 2.978 0a1.533 1.533 0 012.287-.947c1.372.836 2.942-.734 2.106-2.106a1.533 1.533 0 01.947-2.287c1.561-.379 1.561-2.6 0-2.978a1.532 1.532 0 01-.947-2.287c.836-1.372-.734-2.942-2.106-2.106a1.532 1.532 0 01-2.287-.947zM10 13a3 3 0 100-6 3 3 0 000 6z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Settings</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Timeline</span>
                   </button>
                   <button type="button" class="p-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
                       <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 17a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zm3.293-7.707a1 1 0 011.414 0L9 10.586V3a1 1 0 112 0v7.586l1.293-1.293a1 1 0 111.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                       <span class="sr-only">Download</span>
                   </button>
               </div>
           </div>
           <button type="button" data-tooltip-target="tooltip-fullscreen" class="p-2 text-gray-500 rounded cursor-pointer sm:ml-auto hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600">
               <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 4a1 1 0 011-1h4a1 1 0 010 2H6.414l2.293 2.293a1 1 0 11-1.414 1.414L5 6.414V8a1 1 0 01-2 0V4zm9 1a1 1 0 010-2h4a1 1 0 011 1v4a1 1 0 01-2 0V6.414l-2.293 2.293a1 1 0 11-1.414-1.414L13.586 5H12zm-9 7a1 1 0 012 0v1.586l2.293-2.293a1 1 0 111.414 1.414L6.414 15H8a1 1 0 010 2H4a1 1 0 01-1-1v-4zm13-1a1 1 0 011 1v4a1 1 0 01-1 1h-4a1 1 0 010-2h1.586l-2.293-2.293a1 1 0 111.414-1.414L15 13.586V12a1 1 0 011-1z" clip-rule="evenodd"></path></svg>
               <span class="sr-only">Full screen</span>
           </button>
           <div id="tooltip-fullscreen" role="tooltip" class="inline-block absolute invisible z-10 py-2 px-3 text-sm font-medium text-white bg-gray-900 rounded-lg shadow-sm opacity-0 transition-opacity duration-300 tooltip dark:bg-gray-700">
               Show full screen
               <div class="tooltip-arrow" data-popper-arrow></div>
           </div>
       </div>
       <div class="py-2 px-4 bg-gray-100 rounded-b-lg ">
           <label for="editor" class="sr-only">Publish post</label>
           <textarea id="editor" rows="8" class="block px-0 w-full text-sm text-gray-800 bg-gray-100 border-0  focus:ring-0 " placeholder="Write an article..." required></textarea>
       </div>
   </div>
   <button type="submit" class="inline-flex items-center px-5 py-2.5 text-sm font-medium text-center text-white bg-blue-700 rounded-lg focus:ring-4 focus:ring-blue-200 dark:focus:ring-blue-900 hover:bg-blue-800">
       Publish post
   </button>
</form>


  </section>
</section>
</layeoutVue>
</template>
<style>
</style>
