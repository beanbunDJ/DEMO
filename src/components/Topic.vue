<template>
  <div></div>
    <div v-for="(item,i) in tdata" key="item.id">
      <div class="title">{{item.title}}</div>
      <div class="anser"><textarea :value="item.anser"></textarea></div>
    </div>
  </div>
</template>

<script>
let data=[
  {
    id:1,
    title:'MVC 和 MVVM 区别',
    anser:`MVC
MVC全名是 Model View Controller,时模型 - 视图 - 控制器的缩写，一种软件设计典范。

Model(模型)：是用于处理应用程序数据逻辑部分。通常模型对象负责在数据库中存取数据。
View(视图)：是应用程序中处理数据显示的本分。通常视图是依据模型数据创建的。
Controller(控制器)：是应用程序处理用户交互的部分。通常控制器负责从视图读取数据，控制用户输入，并向模型发送数据。`
  },
  { id:2,
    title:'第2题',
    anser:'解答思路如下：xxx'
  }
]
  export default {
    data() {
      return {
        tdata: data,
      }
    },
  }
</script>

<style lang="scss" scoped>
.title{
  padding:10px 24px;
  background:#ccc;
  font-weight: bold;
  font-size: 16px;
}
.anser{
  padding:10px 24px;
  textarea{
    width:100%;
    height: 300px;
  }
}
</style>