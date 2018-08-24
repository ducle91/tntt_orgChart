<template>
  <div>
    <vo-basic :data="chartData"></vo-basic>
  </div>
</template>

<script>
import { VoBasic } from 'vue-orgchart'
export default {
  components: { VoBasic },
  created () {
    this.chartData = {
      name: 'Cha Tuyen Uy - Fr.Tri',
        children: [
          { name: 'Doan Truong - Thinh Tran',
            children:
            [
              {name: 'PQT - Jade Phan'},
              {name: 'PNH - Duc Le'},
              {name: 'Thu Ky - Amy Dang'},
              {name: 'Thu Quy - Tru Nguyen'}
            ] 
          }
        ]
    }
}
}
</script>

