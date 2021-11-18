<template>
  <div class="chestnut">{{ name }}
    </div>
</template>

<script>
export default {
  data() {
    return {
      name: "chestnut-知识点",
      date: '2021-10-11'
    };
  },
  methods(){
   return{
     changedate() {
      let now =  new date();
      a.getFullYear();
    }
    } 
  }
};
</script>

<style lang="scss" scoped>
.chestnut {
  background: #587fff;
  color: #fff;
  text-align: center;
  padding: 12px 24px;
}
</style>