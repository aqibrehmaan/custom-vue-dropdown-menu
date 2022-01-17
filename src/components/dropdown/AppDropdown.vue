<template>
    <div class="relative">
          <a href="" class="text-sm inline-flex bg-gray-300 h-10 px-4 rounded text-center flex items-center justify-center leading-none text-gray-600">Button</a>
          <ul class="bg-white shadow-xl absolute rounded overflow-hidden z-50 w-40 mt-2">
            <li v-for="(item, index) in items" :key="index"><a href="" class="block p-2 text-sm text-gray-800 hover:bg-gray-100">{{ item.title }}</a></li>
          </ul>
      </div>
</template>

<script>
export default {
    props: {
        items: {
            required: true,
            type: Array
        }
    }
}
</script>