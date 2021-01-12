<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
<!-- <ve-line :data="chartData"></ve-line> -->
 <ve-line :data="chartData"></ve-line>


  </div>
</template>

<script>
// @ is an alias to /src
import VeLine from 'v-charts/lib/line'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data(){
    return{
      chartData: {
            columns: ['日期', '销售额'],
            rows: [
              { '日期': '1月1日', '销售额': 123 },
              { '日期': '1月2日', '销售额': 1223 },
              { '日期': '1月3日', '销售额': 2123 },
              { '日期': '1月4日', '销售额': 4123 },
              { '日期': '1月5日', '销售额': 3123 },
              { '日期': '1月6日', '销售额': 7123 }
            ]
          }
      
   
    }
    }
   
 
}
</script>
