<template>
  <div>
    <vo-basic :data="chartData"></vo-basic>
  </div>
</template>

<script>
import { VoBasic } from 'vue-orgchart'
export default {
  name:'btv',
  components: { VoBasic },
  created () {
    this.chartData = {
        name: 'BCH',
        children: [
            //-------------------HSTT-----------------------
            {
            name: 'Hiep Si Truong Thanh',
            children: 
            [
                {   
                    name: 'NT - Duc Le',
                    children: [{name: 'NP - Vien'}] 
                }
            ]
            },
            //--------------------HS------------------------
            {
            name: 'Hiep Si',
            children: 
            [
                {
                    name: 'NT - Quang Dong',
                    children: [{name: 'NP - Thuong Hunyh'}]
                }
            ]
            },
            //---------------------NS-----------------------
            {
            name: 'Nghia Si',
            children:
            [
                {
                    name: 'NT - Huy Vu',
                    children: [{name: 'NP - Khoa Nguyen'}]
                }
            ]
            },
            //---------------------TN------------------------
            {
            name: 'Thieu Nhi',
            children:
            [
                {
                    name: 'NT - David Tran',
                    children: [{name: 'NP - Jade Phan'}]
                }
            ]
            },
            //---------------------AN------------------------
            {
            name: 'Au Nhi',
            children:
            [
                {
                    name: 'NT - Ngoc Nguyen',
                    children: [{name: 'NP - Anne Le'}]
                }
            ]
            },
        ]
    }
}
}
</script>

