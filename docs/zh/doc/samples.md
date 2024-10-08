---
layout: doc
title: 文档插件示例

authors:
  - M1hono
  - skyraah
tags:
  - sample
---

# 文档插件示例

## Mermaid示例

:::demo


```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```


:::

## 时间线插件示例



:::: demo 示例
::: timeline 2023-05-24
- **do some thing1**
- do some thing2
:::

::: timeline 2023-05-23
do some thing3
do some thing4
:::
::::

## B站视频示例

:::demo
<BilibiliVideo bvid="BV1rC4y1C7z2" />
:::

## 伤害静态图示例

:::demo

<DamageChart
  mode="static"
  :incomingDamage="20"
  :armorToughness="5"
  :minDamage="4"
  :maxDamage="20"
  :maxArmorPoints="20"
  :isJavaEdition="true"
/>

:::

## PDF Viewer

:::demo
<PdfViewer pdfSource="/pdf/modding/java/test.pdf"/>
:::

## 文件树

<!-- :::demo -->
<LiteTree>
#error=color:red;border: 1px solid red;background:#ffd2d2;padding:2px;
#blue=color:red;border: 1px solid blue;background:#e6e6ff;padding:2px;
airplane=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjgiIGhlaWdodD0iMTI4IiB2aWV3Qm94PSIwIDAgMjQgMjQiPjxwYXRoIGZpbGw9IiNmZmZmZmYiIGQ9Ik0yMC41NiAzLjkxYy41OS41OS41OSAxLjU0IDAgMi4xMmwtMy44OSAzLjg5bDIuMTIgOS4xOWwtMS40MSAxLjQybC0zLjg4LTcuNDNMOS42IDE3bC4zNiAyLjQ3bC0xLjA3IDEuMDZsLTEuNzYtMy4xOGwtMy4xOS0xLjc3TDUgMTQuNWwyLjUuMzdMMTEuMzcgMTFMMy45NCA3LjA5bDEuNDItMS40MWw5LjE5IDIuMTJsMy44OS0zLjg5Yy41Ni0uNTggMS41Ni0uNTggMi4xMiAwIi8+PC9zdmc+
ts=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxZW0iIGhlaWdodD0iMWVtIiB2aWV3Qm94PSIwIDAgMTUgMTUiPjxwYXRoIGZpbGw9Im5vbmUiIHN0cm9rZT0iY3VycmVudENvbG9yIiBkPSJNMTIuNSA4di0uMTY3YzAtLjczNi0uNTk3LTEuMzMzLTEuMzMzLTEuMzMzSDEwYTEuNSAxLjUgMCAxIDAgMCAzaDFhMS41IDEuNSAwIDAgMSAwIDNoLTFBMS41IDEuNSAwIDAgMSA4LjUgMTFNOCA2LjVIM20yLjUgMFYxM00uNS41aDE0djE0SC41eiIvPjwvc3ZnPg==
---
- [airplane]A公司({color:red;}重点,{#blue}紧急)          //   企业名称
    行政中心
        {color:red;font-weight:bold;background:#ffeaea}总裁办
        [checked]人力资源部
        [unchecked]{.blue}财务部
        行政部        //+  负责行政管理
        法务部        //+  打官司等
        [airplane]审计部        //+  审计财务[保存:tag](sss) [连接](sss)
        信息中心      // 重点[保存](www.baidu.com)[tag][连接:tag](https://www.baidu.com)
        [star]安[star]全[star]保[star]卫[star]部[star]    //{color:red}   保密工作
    + 市场中心    
        市场部({#error}出错,"{#warning}警告")
        销售部            //-
        客服部            //-
        {#blue}品牌部            //   this is cool
        市场策划部    //!  重点
        市场营销部        // {.blue}this is cool
    研发中心
        移动研发部      //!
        平台研发部({success}Java,{error}Go)
        {.success}测试部
        运维部
        产品部            //*
        设计部            //*
        项目管理部        //*
        
</LiteTree>
<!-- ::: -->