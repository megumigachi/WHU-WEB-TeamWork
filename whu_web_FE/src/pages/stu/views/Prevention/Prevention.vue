<template>
  <div>
    <el-row>
      <el-col :span="4" v-for="(o, index) in DiseaseList" :key="o.title" :offset="index > 0 ? 2 : 0">
        <PreventDetail :DiseaseInfo = "o"></PreventDetail>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import PreventDetail from '@/pages/stu/components/Prevention/Prevention'
export default {
  name: 'Prevention',
  components: {
    PreventDetail
  },
  data () {
    return {
      DiseaseList: [
        {
          ImgSrc: 'https://s1.ax1x.com/2020/04/24/JrB9f0.jpg',
          Title: '腰肌劳损',
          Name: 'LumbarMuscleDegeneration',
          Description: '因腰部肌肉、韧带等软组织损伤导致疼痛 \n 好发于30～50岁的中青年人 \n 可表现出腰部疼痛及活动受限 \n 积极治疗后大多数可得到完全缓解'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
