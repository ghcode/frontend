# webpack.cmd
    1. %~dp0 获取webpack.cmd所在目录
    2. "%~dp0\node_modules\webpack\bin\webpack.js" %* 拼接webpack.js 得完整路径
    3. node  "%~dp0\node_modules\webpack\bin\webpack.js" %*

# webpack.js
    1. 判断webpack-cli或webpack-command是否安装
    2. 如果没有,首选安装webpack-cli
    3. 加载webpack-cli包下的package.json,获取bin字段的值(此版本为./bin/cli.js)
    4. 加载cli.js

# webpack-cli.js
    1.  options = require("./convert-argv")(argv);
        加载wepack.config.js,分析webpack命令行参数
    2.  加载/lib/webpack.js




# 知识点
 * process.argv\: 返回一个数组，这个数组包含了启动Node.js进程时的命令行参数。第一个元素为process.execPath。如果需要获取argv[0]的值请参见node文档的 process.argv0。第二个元素为当前执行的JavaScript文件路径。剩余的元素为其他命令行参数。
 * __filename 
 * reduce()
 * Object.creat
 * process.argv


# webpack

## [webpack4.0](http://blog.51cto.com/13869008/category6.html 'webpack')

## [tapable](https://www.codercto.com/a/21587.html 'tapable')




# Object

## 1. Object.assign()
## 2. Object.creat()
## 3. Object.assign()