<template>
  <div>
    <div formGroup="orderForm">
    <div class="form-row">
        <div class="form-group col-md-6">
            <div class="e-float-input e-control-wrapper">
                <input id="OrderID" name="OrderID" v-model='data.OrderID' type="text" :disabled="!data.isAdd">
                <span class="e-float-line"></span>
                <label class="e-float-text e-label-top" for="OrderID"> Order ID</label>
            </div>
        </div>
    </div>
    <div class="form-row">
        <!-- DatePicker Should be rendered below -->
        <div class="form-group col-md-6">
            <HelloWorld msg="check"></HelloWorld>
            
        </div>
    </div> 
</div>
  </div>
</template>

<script>

import { HelloWorld } from "./components/HelloWorld";

// import { createApp } from "vue";
// 
// const app = createApp();

// app.mixin();

export default {
  name: "App",
  components: {
    "HelloWorld": HelloWorld,
  },
  data() {
    return {
      data: {},
    };
  },
};
</script>

<style>
</style>
