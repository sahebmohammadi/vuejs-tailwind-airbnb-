<template>
  <div id="app" class="min-h-screen bg-gray-200 antialiased">
    <SiteHeader />
    <SearchFilters />
    <main class="px-4 py-6">
      <h3 class="text-xl tex-gray-900">Los Angeles</h3>
      <p class="text-gray-600">Live like the stars in these luxurious Southern California estates.</p>
      <div class="mt-6 sm:flex sm:overflow-x-auto sm:space-x-2 sm:pb-8">
        <article :class="{ 'mt-10': i > 1 }" class="sm:mt-0 sm:max-w-xs sm:w-full sm:flex-shrink-0" v-for="i in 4">
          <div>
            <img class="rounded-lg h-64 object-cover w-full" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80" alt="" />
          </div>
          <div class="relative -mt-16 px-4">
            <div class="shadow-xl rounded-lg p-4 bg-white">
              <span class="rounded-full bg-green-200 text-green-800 px-2 py-1 leading-none font-medium text-xs uppercase tracking-wide">Plus</span>
              <span class="text-gray-400 font-semibold uppercase ml-3">3 beds &bull; 2 baths</span>
              <h4 class="text-gray-900 mt-2 font-semibold text-base">Modern home in city center</h4>
              <div class="mt-1">
                <span class="text-gray-900">$1,400</span>
                <span class="text-gray-600 ml-1 text-sm">/wk</span>
              </div>
              <div class="mt-2 text-sm text-gray-600 flex items-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 fill-current text-green-500" viewBox="0 0 20 20" fill="currentColor">
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  />
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 fill-current text-green-500" viewBox="0 0 20 20" fill="currentColor">
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  />
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 fill-current text-green-500" viewBox="0 0 20 20" fill="currentColor">
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  />
                </svg>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 fill-current text-green-500" viewBox="0 0 20 20" fill="currentColor">
                  <path
                    d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"
                  />
                </svg>
                <span class="ml-2">40 reviews</span>
              </div>
            </div>
          </div>
        </article>
      </div>
    </main>
  </div>
</template>

<script>
import SiteHeader from "./components/SiteHeader.vue";
import SearchFilters from "./components/SearchFilters.vue";

export default {
  name: "app",
  components: {
    SiteHeader,
    SearchFilters,
  },
};
</script>
