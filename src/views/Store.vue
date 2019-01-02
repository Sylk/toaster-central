<template>
  <div class="home">
    <StoreItem
    :v-for="item in store"/>
  </div>
</template>

<script>
import StoreItem from '@/components/StoreItem.vue'

export default {
  name: 'store',
  components: {
    StoreItem
  },
  data() {
    return {
        store: [
            {item: 'Sock', description: 'Just a sock you know?'},
            {item: 'Yam', description: 'Just a yam you know?'}
        ]
    }
  }
}
</script>