<template>
  <div class="inner-doc">
    <FileMenu />
    <div id="doc-bg">
      <iframe id="fr"></iframe>
    </div>
  </div>
</template>
<script setup lang="ts">
import FileMenu from '@/components/FileMenu.vue'

//https://developer.mozilla.org/zh-CN/docs/Web/API/HTMLIFrameElement/contentWindow
</script>

<style lang="scss" scoped>
.inner-doc {
  width: 100%;
  height: calc(100vh - 56px);
}

#doc-bg {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #ccc;

  > #fr {
    border: none;
    background-color: #fff;
    box-shadow: #00000023 0 0 3px 3px;
  }
}
</style>
