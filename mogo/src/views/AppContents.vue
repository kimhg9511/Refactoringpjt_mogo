<template>
  <div>
    <story-about-us></story-about-us>
    <sec-statistics></sec-statistics>
    <amazing-services></amazing-services>
    <unique-design></unique-design>
    <what-we-do></what-we-do>
    <sec-comment></sec-comment>
    <meet-our-team></meet-our-team>
    <some-of-our-works></some-of-our-works>
    <sec-comment></sec-comment>
    <what-people-say></what-people-say>
    <latest-blog></latest-blog>
    <open-map></open-map>
    <sec-community></sec-community>
  </div>
</template>

<script>
import StoryAboutUs from '../components/SecStoryAboutUs';
import SecStatistics from '../components/SecStatistics';
import AmazingServices from '../components/SecAmazingServices';
import UniqueDesign from '../components/SecUniqueDesign';
import WhatWeDo from '../components/SecWhatWeDo';
import SecComment from '../components/SecComment';
import MeetOurTeam from '../components/SecMeetOurTeam';
import SomeOfOurWorks from '../components/SecSomeofOurWorks';
import WhatPeopleSay from '../components/SecWhatPeopleSay';
import LatestBlog from '../components/SecLatestBlog';
import OpenMap from '../components/SecOpenMap';
import SecCommunity from '../components/SecCommunity';
export default {
  components: {
    StoryAboutUs,
    SecStatistics,
    AmazingServices,
    UniqueDesign,
    WhatWeDo,
    SecComment,
    MeetOurTeam,
    SomeOfOurWorks,
    WhatPeopleSay,
    LatestBlog,
    OpenMap,
    SecCommunity,
  }
}
</script>

<style>

</style>