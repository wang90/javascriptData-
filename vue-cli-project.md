# vue 创建项目相关内容
## vue-cli创建
##### 下载vue-cli
``````
npm install vue-cli
``````
##### vue-cli3创建项目
``````
vue create app
cd app 
npm install 
npm run dev
npm run-script build 
``````

## 项目中加入less
##### 下载less
``````
npm i style-resources-loader vue-cli-plugin-style-resources-loader -D
npm install --save -dev less-loader
``````
##### vue.config.js添加内容
``````
pluginOptions: {
      'style-resources-loader': {
        preProcessor: 'less',
        patterns: [path.resolve(__dirname, "src/common/less/variable.less")] // 引入全局样式变量
      }
}
``````
