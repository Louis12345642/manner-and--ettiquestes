
<script>
import layeout from '@/Layouts/layeout.vue'
import { Link } from '@inertiajs/inertia-vue3'
import { ref } from 'vue'
import moment from 'moment'
export default{
  components: { layeout ,Link},
props:{
    singlePost:Array
},
setup(props){
    const singlePost=props.singlePost
    const authorRoute=ref('/author/'+singlePost.author.username)
    const categoryRoute=ref('/categories/'+singlePost.category.slug)
    return{
        moment,
        authorRoute,
        categoryRoute
    }
}
}
</script>

<template>
 <layeout>

    <main class="max-w-6xl mx-auto mt-10 lg:mt-20 space-y-6 container">
    <article class="max-w-4xl mx-auto lg:grid lg:grid-cols-12 gap-x-10">
        <div class="col-span-4 lg:text-center lg:pt-14 mb-10">
            <img src="/atomic.jpg" alt="" class="rounded-xl">

            <p class="mt-4 block text-gray-400 text-xs">
                Published <time>{{moment(singlePost.created_at).startOf('hour').fromNow()}} </time>
            </p>

            <div class="flex items-center lg:justify-center text-sm mt-4">
                <img class="mt-7 w-16 h-16 rounded-full round-border" src="/logo.jpg" alt="">
                <div class="ml-5 text-left mt-5">
                 <Link :href="authorRoute">   <h5 class="font-bold">   {{singlePost.author.name}}</h5></Link>
                    <h6>Manners and Ettiquetes</h6>
                </div>
            </div>
        </div>

        <div class="col-span-8">
            <div class="hidden lg:flex justify-between mb-6">
                <Link href="/"
                    class="transition-colors duration-300 relative inline-flex items-center text-lg hover:text-blue-500">
                    <svg width="22" height="22" viewBox="0 0 22 22" class="mr-2">
                        <g fill="none" fill-rule="evenodd">
                            <path stroke="#000" stroke-opacity=".012" stroke-width=".5" d="M21 1v20.16H.84V1z">
                            </path>
                            <path class="fill-current"
                                d="M13.854 7.224l-3.847 3.856 3.847 3.856-1.184 1.184-5.04-5.04 5.04-5.04z">
                            </path>
                        </g>
                    </svg>

                    Back to Posts
                </Link>


                <div class="space-x-2">
                    <Link :href="categoryRoute"
                        class="px-3 py-1 border border-blue-300 rounded-full text-blue-300 text-xs uppercase font-semibold"
                        style="font-size: 10px">{{singlePost.category.title }}</Link>

                </div>
            </div>

            <h1 class="font-bold text-3xl lg:text-4xl mb-10">
                {{singlePost.title}}

            </h1>

            <div class="space-y-4 lg:text-lg leading-loose space-x-2">
               <p>   {{singlePost.body}}</p>

            </div>
        </div>
    </article>
</main>
 </layeout>
</template>
<style>
</style>
