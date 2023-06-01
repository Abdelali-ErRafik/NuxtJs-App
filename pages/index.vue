<template>
<div>
  <div class="container">
    <Hero />
    <LargeCardDisplay
      v-for= "cardInfo in largeCardInfo"
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
  name: 'HomeView',
  data () {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections
    }
  }
}
</script>
