<template>
  <div>
    <story-about-us></story-about-us>
    <sec-statistics></sec-statistics>
    <amazing-services></amazing-services>
  </div>
</template>

<script>
import StoryAboutUs from '../components/SecStoryAboutUs'
import SecStatistics from '../components/SecStatistics'
import AmazingServices from '../components/SecAmazingServices'
export default {
  components: {
    StoryAboutUs,
    SecStatistics,
    AmazingServices,
  }
}
</script>

<style>

</style>