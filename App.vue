<template>
  <a-config-provider :locale="locale">
<div>test</tets>
  <div id="app">
    <keep-alive>
    <router-view />

    </keep-alive>
  </div>
  </a-config-provider>
</template>

<script>
import zhCN from 'ant-design-vue/lib/locale-provider/zh_CN';
export default {
  name: 'App',
  data() {
    return {
      locale: zhCN,
    };
  },
}
</script>

<style>
@font-face
{
  font-family: dwnu;
  src: url('assets/dwnu.ttf')
}
.LayerImage {

  z-index: 99;
}

.ant-input-sm{
  height:100%
}
.ant-input-affix-wrapper {
  height: 1.9rem;
}
   .ant-table-placeholder{
    background: #081219;
    border: none;
  }
  .ant-table-header  {
     overflow: auto !important;
   }
   .ant-table-fixed-header > .ant-table-content > .ant-table-scroll > .ant-table-body{margin-top: 1rem}
body,html{height:100%;width:100%}

body,
html {
  width: 100%;
  height: 100%;
  font-family:"microsoft yahei";
  font-size: 1vw;
  overflow-x: hidden;
  overflow: auto;
}
html, body, ul, li, ol, dl, dd, dt, p, h1, h2, h3, h4, h5, h6, form, fieldset, legend, img {
  margin: 0 ;
  padding: 0;
}

ul, ol {
  list-style: none; /*去掉原样式中的小黑点*/
}
#app{ width: 100%; height: 100%; color: #fff; background-color: #0a0b11;
  overflow: hidden;
}
   /*定义滚动条高宽及背景 高宽分别对应横竖滚动条的尺寸*/
   ::-webkit-scrollbar {
     width: 0.3rem;
     height: 0.5rem;
     background-color: transparent;
   }

   /*定义滚动条轨道 内阴影+圆角*/
   ::-webkit-scrollbar-track {
     -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
     border-radius: 10px;
     background-color: #555;
   }

   /*定义滑块 内阴影+圆角*/
   ::-webkit-scrollbar-thumb {
     border-radius: 10px;
     -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
     background-color: #21c9d9;
   }


</style>
