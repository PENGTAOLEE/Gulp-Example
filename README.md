# Gulp
> 这是一个个人的把玩项目，还有很多坑需要踩 不建议直接clone
## 依赖环境
* node
* npm 

## 创建项目
```bash
mkdir gulp
cd gulp
```
## 构建项目目录结构
```
├── dist                                       #发布环境 
│   ├── css                                    #编译后的CSS文件
|   |   └── etc..
│   ├── images                                 #压缩后的图片文件
|   |   └── etc..
│   ├── js                                     #编译后的JS文件
|   |   └── etc..
│   ├── index.html
├── src                                        #开发环境
│   ├── scss                                   # CSS文件
|   |   └── etc..
│   ├── images                                 # 图片资源
|   |   └── etc..
│   |── js                                     # JS文件
|   |   └── etc..
|   |── index.html                             # HTML
├── package.json                               # 依赖管理
|── gulpfile.js                                #任务文件
├── README.md                                  #md文件
```
   
## 安装gulp

### 全局安装
```bash
npm install -g gulp
```
> Gulp在每构建一个项目时，都需要全局安装一次 
> gulp -v 查看版本号

### 本地安装
> npm init 

```bash
npm install gulp --save-dev
```

## Gulp安装插件
* gulp-webserver         # 静态服务器
* gulp-livereload        # 网页自动刷新

```bash
npm install gulp-livereload gulp-webserver --save-dev
```

## Gulp 任务配置

在项目根目录中，创建gulpfile.js文件，用来配置和定义任务
```bash
touch gulpfile.js
```

## 插件介绍及使用方法

```javascript
// 这里会放一套最后成型的gulpfile.js文件
// ... 然而还没配置完成
```

### gulp执行命令

执行多条命令
```javascript
gulp.task('build', ['scripts', 'assets','html',...]);
```

> gulp build   

gulp : 执行默认配置
```javascript
gulp.task('default',['webserver','watch']);
```

> gulp 

## 提交Gitbub

不提交依赖包 && 打包文件 && log文件
```bash
#不提交依赖模块
node_modules

#不提交打包后文件
dist

#不提交npm debug
npm-debug.log
```





































