<template>
    <div id="app">
        <div class="btn-list">
            <el-button type="primary" size="small" @click="ChangeTree('RenderTree')">render-content</el-button>
            <el-button type="primary" size="small" @click="ChangeTree('SlotTree')">scoped slot</el-button>
        </div>
        <router-view/>
    </div>
</template>

<script>
export default {
    name: 'app',
    methods: {
        ChangeTree(name){
            this.$router.push({name})
        }
    }
}
</script>

<style>
    *{
      padding:0;
      margin:0;
      box-sizing:border-box;
    }
    html,body{
      width:100%;
      height:100%;
    }
    #app {
      width:100%;
      height:100%;
      position:relative;
      font-family: 'Avenir', Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      /*text-align: center;*/
      color: #2c3e50;
    }
    .btn-list{
        padding: 1em 0;
        text-align: center;
    }
</style>
