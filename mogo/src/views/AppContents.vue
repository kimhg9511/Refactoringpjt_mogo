<template>
  <div>
    <story-about-us></story-about-us>
    <sec-statistics></sec-statistics>
    <amazing-services></amazing-services>
    <unique-design></unique-design>
    <what-we-do></what-we-do>
  </div>
</template>

<script>
import StoryAboutUs from '../components/SecStoryAboutUs';
import SecStatistics from '../components/SecStatistics';
import AmazingServices from '../components/SecAmazingServices';
import UniqueDesign from '../components/SecUniqueDesign';
import WhatWeDo from '../components/SecWhatWeDo';
export default {
  components: {
    StoryAboutUs,
    SecStatistics,
    AmazingServices,
    UniqueDesign,
    WhatWeDo,
  }
}
</script>

<style>

</style>