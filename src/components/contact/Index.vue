<template>
  <div class="contact">
    <router-link to="/contact">
      <el-button>Email</el-button>
    </router-link>
    <router-link to="/contact/phone">
      <el-button>Phone</el-button>
    </router-link>
    <router-link to="/contact/gmap">
      <el-button>Map</el-button>
    </router-link>
    <hr>
    <router-view></router-view>
  </div>
</template>

<script>
  import Email from './Email';
  import Phone from './Phone';
  import Gmap from './Gmap';

  export default {
    name: 'contact',
    components: {
      Email,
      Phone,
      Gmap,
    },
  };
</script>
