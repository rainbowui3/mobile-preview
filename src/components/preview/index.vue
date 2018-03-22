<template>
 <div>
        <form-preview :header-label="title" :header-value="value" :body-items="data" :footer-buttons="buttons" :name="param"></form-preview>
  </div>
</template>

<script>
const FormPreview =  require("vux/src/components/form-preview/index.vue");
export default {
  props: {
    title: String,
    value: String,
    data:Array,
    buttons:Array,
    param:Object
  },
  components: {
    FormPreview
  }
}
</script>
<style>
.weui-form-preview__btn_primary {
   color: #4D93E4!important;
}
</style>

