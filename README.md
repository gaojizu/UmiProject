# UmiProject
### Umi项目，结合了Proantd开发的项目，展示了基本使用
## 安装Umi 项目步骤
[官网](https://umijs.org/zh-CN/docs/getting-started)
#### 安装国内源（如果你有代理的话可以忽略）
> npm i yarn tyarn -g
#### 查看安装版本
> tyarn -v
#### 安装Umi
> tyarn create @umijs/umi-app
#### 安装依赖
> tyarn install
#### 启动
> tyarn start
#### 安装antdpro
> tyarn add @ant-design/pro-layout
#### 安装成功截图
![image](https://user-images.githubusercontent.com/37791775/116212227-3362ec80-a777-11eb-8343-70fb2c153e36.png)
#### 更新配置文件（测试是否成功） 文件名：.umirc.ts
  ```js
  import { defineConfig } from 'umi';

export default defineConfig({
  nodeModulesTransform: {
    type: 'none',
  },
  layout: {},
  routes: [
    { path: '/', component: '@/pages/index' },
  ],
  fastRefresh: {},
});
  ```
  #### 部署
  > tyarn build
  #### 测试，安装serve
  > tyarn global add serve
  #### 运行测试
  > serve ./dist
  #### 运行效果
  ![image](https://user-images.githubusercontent.com/37791775/116213855-b6d10d80-a778-11eb-8f71-8dba01031b99.png)



