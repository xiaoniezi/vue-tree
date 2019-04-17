<template>
    <div id="app">
        <div class="check-router">
            <el-radio-group v-model="type" @change="changeRouter">
                <el-radio-button label="RenderTree">render-content</el-radio-button>
                <el-radio-button label="SlotTree">scoped slot</el-radio-button>
            </el-radio-group>
        </div>
        <router-view />
    </div>
</template>

<script>
export default {
    name: 'app',
    data(){
        return {
            type: 'SlotTree'
        }
    },
    methods: {
        changeRouter(name) {
            this.$router.push({ name: this.type })
        }
    }
}
</script>

<style lang="scss">
* {
    // padding: 0;
    // margin: 0;
    box-sizing: border-box;
}

html,
body {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
}

#app {
    width: 100%;
    height: 100%;
    position: relative;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    /*text-align: center;*/
    color: #2c3e50;
}

.check-router{
    padding: 1em 2em;
}
</style>