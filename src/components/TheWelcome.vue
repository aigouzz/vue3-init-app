<script setup lang="ts">
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import SupportIcon from "./icons/IconSupport.vue";
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>毕业学校</template>

    <a href="https://www.bupt.edu.cn/" target="_blank" rel="noopener">北京邮电大学</a>
    2009-2013
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>专业</template>

    信息管理与信息系统
    <a
      href="https://baike.baidu.com/item/%E4%BF%A1%E6%81%AF%E7%AE%A1%E7%90%86%E4%B8%8E%E4%BF%A1%E6%81%AF%E7%B3%BB%E7%BB%9F/890173?fr=aladdin"
      target="_blank"
      rel="noopener"
      >专业</a
    >
    <br />
    <a href="https://code.visualstudio.com/" target="_blank" rel="noopener"
      >VSCode</a
    >
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>职业</template>

    前端开发工程师
    <br />
    <a href="https://baike.baidu.com/item/%E5%89%8D%E7%AB%AF%E5%BC%80%E5%8F%91?fromModule=lemma_search-box" target="_blank" rel="noopener">链接</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>特长</template>

    <a href="https://www.vuejs.org" target="_blank" rel="noopener">Vue</a> + 
    <a href="https://vuex.vuejs.org/zh/" target="_blank" rel="noopener">vuex</a> + 
    <a href="https://router.vuejs.org/zh/" target="_blank" rel="noopener">vue-router</a> + 
    <a href="https://webpack.docschina.org/" target="_blank" rel="noopener">webpack</a>
    <br />
    <a href="https://react.docschina.org/" target="_blank" rel="noopener">React</a> + 
    <a href="https://cn.redux.js.org/" target="_blank" rel="noopener">redux</a> + 
    <a href="http://react-guide.github.io/" target="_blank" rel="noopener">react-router</a> + 
    <a href="https://webpack.docschina.org/" target="_blank" rel="noopener">webpack</a>
    <br />
    <a href="https://www.w3school.com.cn/html/html5_intro.asp" target="_blank" rel="noopener">HTML5</a> + 
    <a href="https://www.runoob.com/css3/css3-tutorial.html" target="_blank" rel="noopener">css3</a> 
    <br />
    <a href="http://nodejs.org/" target="_blank" rel="noopener">Nodejs</a>
    <br />
    <a href="https://developers.weixin.qq.com/miniprogram/dev/framework/" target="_blank" rel="noopener">小程序开发</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>爱好</template>

    <a href="https://baike.baidu.com/item/%E8%B7%91%E6%AD%A5/4510250" target="_blank" rel="noopener">跑步</a>
    + 
    <a href="https://baike.baidu.com/item/%E9%9F%B3%E4%B9%90/61907" target="_blank" rel="noopener">音乐</a>
    + 
    <a href="https://baike.baidu.com/item/%E8%A7%86%E9%A2%91/321962" target="_blank" rel="noopener">视频</a>
  </WelcomeItem>
</template>
