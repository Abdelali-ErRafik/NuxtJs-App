<template>
<div>
  <div class="container">
    <LargeCardDisplay
      v-for= "cardInfo in largeCardInfo.slice(0,1)"
      :key= "cardInfo.id"
      :cardSection="cardInfo"
      />
      <SmallCardDisplay
        v-for= "cardInfo in smallCardInfo"
        :key= "cardInfo.id"
        :cardsSection="cardInfo"
        />
  </div>
</div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data'
export default {
  name: 'ProductsView',
  data () {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }
}
</script>
