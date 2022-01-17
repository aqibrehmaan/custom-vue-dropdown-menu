<template>
    <div class="container mx-auto p-6"> 
        <AppDropdown :items="items" />
    </div>
</template>

<script>

import AppDropdown from '@/components/dropdown/AppDropdown'

export default {
    components: {
      AppDropdown
    },
    data() {
      return {
        items: [
          { title: 'Price: High to low', slug: 'price-desc'},
          { title: 'Price: Low to high', slug: 'price-asc'}
        ]
      }
    }
}
</script>

<style src="@/assets/app.css">

</style>
