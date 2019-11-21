# webpack打包项目
 ## 操作步骤
  ### 1.  创建前端项目架构包含src目录，用来存放源文件,src下创建index.html，main.js，创建dist目录用来存放打包后的文件
  ### 2.  到项目内部使用终端执行npm init -y初始化项目信息
  ### 3.  在项目内部安装webpack，使用终端执行npm i webpack webpack-cli -D (不指定版本安装最新的webpack)
  ### 4.  执行webpack src/main.js -o dist/bundle.js将本次编辑的main.js打包为bundle.js
  ### 5.  项目根目录新增webpack.config.js配置webpack相关参数，之后到终端执行webpack打包
  ### 6.  终端执行npm i webpack-dev-server -D安装webpack-dev-server插件到本地项目中
  ### 7.  修改项目的package.json文件script对象，新增"dev": "webpack-dev-server --open --port 3001 --contentBase src --hot"
  ### 8.  终端执行npm run dev开启自动编译JS
  ### 9.  终端执行npm i html-webpack-plugin -D安装html-webpack-plugin插件到项目中
  ### 10. 到项目的webpack.config.js中新增html-webpack-plugin
  ### 11. 对项目的CSS文件进行编译，到main.js引入本次新增的index.css样式文件
  ### 12. 安装CSS所需的loader: npm i style-loader css-loader -D
  ### 13. 到webpack.config.js中新增CSS相关配置，添加module属性配置正则匹配规则
  ### 14. 终端执行npm i less-loader less -D 安装less所需loader到本地
  ### 15. 终端执行npm i sass-loader node-sass -D 安装sass所需loader到本地项目
  ### 16. 需要打包生产时将webpack.config.js的mode改为production，再到终端执行webpack即可在项目的dist目录下生成压缩后的页面以及对应的JS文件
  ### 17. 打包项目中图片信息需要安装url-loader，终端执行npm i url-loader file-loader -D
  ### 18. 到webpack.config.js中新增module的匹配规则
  ### 19. 安装bootstrap终端执行 npm i bootstrap@3.3.7 -s

