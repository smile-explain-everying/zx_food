<template>
    <div class="wrapper">
    <v-head></v-head>
    <v-sidebar></v-sidebar>
    <div class="content">
        <transition name="move" mode="out-in"><router-view></router-view></transition>
    </div>
    </div>
</template>

<script>
import vHead from './Header.vue'
import vSidebar from './Sidebar.vue'
export default {
    components:{
      vHead,vSidebar
    }
}
</script>
<style type="text/css">
    .content{
        background: none repeat scroll 0 0 #fff;
        position: absolute;
        left: 250px;
        right: 0;
        top: 70px;
        bottom: 0;
        width: auto;
        padding: 40px;
        box-sizing: border-box;
        overflow-y: auto;
        }
</style>