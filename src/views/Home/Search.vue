<template>
  <div>
    <search :isvideo="true"
            :issoftware="true"
            :ismicroservice="true"></search>
  </div>
</template>

<script>
import search from '@/components/Search/search'

export default {
  components: {
    search,
  },
  data () {
    return {
      value: ''
    };
  },
  methods: {
    onClickLeft () {
      this.$router.go(-1)
    },
  },
  created () {
    this.value = this.$route.query.value
  }
}
</script>

<style>
</style>