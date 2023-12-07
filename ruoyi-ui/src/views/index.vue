<template>
  <div>
    <!--块类统计-->
    <el-row :gutter="20">
      <el-col :span="6">
        <el-card class="box-card">
          <h3>知识分享文章数</h3>
          <div>
            <i class="el-icon-s-shop" style="color: rgb(128, 36, 0)9, 128, 0)"></i>
            <span>30</span>
          </div>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card class="box-card">
          <h3>累计用户数</h3>
          <div>
            <i class="el-icon-user-solid" style="color: rgb(102, 0, 128)"></i>
            <span>30</span>
          </div>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card class="box-card">
          <h3>兑换次数</h3>
          <div>
            <i class="el-icon-s-flag" style="color: rgb(71, 173, 142)"></i>
            <span>20</span>
          </div>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card class="box-card">
          <h3>入驻作者数</h3>
          <div>
            <i class="el-icon-star-on" style="color: rgb(43, 43, 115)"></i>
            <span>29</span>
          </div>
        </el-card>
      </el-col>
    </el-row>
    <!--acharts统计图-->
    <el-row :gutter="20">
      <el-col :span="16">
        <el-card class="box-card">
          <echarts4 />
        </el-card>
      </el-col>
      <el-col :span="8">
        <el-card class="box-card">
          <echarts6 />
        </el-card>
      </el-col>
      <el-col :span="16">
        <el-card class="box-card">
          <echarts5 />
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import echarts6 from './ECharts/echarts6'
import echarts5 from './ECharts/echarts5'
import echarts4 from './ECharts/echarts4'

export default {
  name: 'home',
  components: {
    echarts6,
    echarts5,
    echarts4
  }
}
</script>

<style scoped>
.el-card {
  margin-bottom: 20px;
  text-align: center;
}
</style>
