<template>
    <div class="container">
        <ColumnList :list="list"/>
    </div>

</template>

<script lang="ts">
import { defineComponent } from 'vue'
import ColumnList, { ColumnProps } from './components/ColumnList.vue'
import 'bootstrap/dist/css/bootstrap.min.css'
const testdata: ColumnProps[] = [
    {
        id:1,
        title:"111111",
        description:"1111111",
        avatar:"http://bpic.588ku.com/element_origin_min_pic/18/08/24/05dbcc82c8d3bd356e57436be0922357.jpg"
    },
    {
        id:1,
        title:"111111",
        description:"1111111",
        avatar:"http://bpic.588ku.com/element_origin_min_pic/18/08/24/05dbcc82c8d3bd356e57436be0922357.jpg"
    }
]
export default defineComponent({
    name: 'App',
    setup(){
        return{
            list:testdata
        }
    },
    components: {
        ColumnList
    }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
