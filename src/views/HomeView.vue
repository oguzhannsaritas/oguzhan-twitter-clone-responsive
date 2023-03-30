<template>
  <div class=" w-full min-h-screen  flex fixed  justify-between overflow-hidden  ">

    <Menu />
    <Feed />
    <Makelogin />
  </div>
</template>
  
<script>

import Menu from '@/components/Menu.vue';
import Feed from '@/components/Feed.vue';
import Makelogin from '@/components/Makelogin.vue';
export default {
  name: 'home',
  components: { Menu, Feed, Makelogin, }
}
</script>
  