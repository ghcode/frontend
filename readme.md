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


## hash、chunkhash、contenthash

## devtool&source map

# LocalStorage
# sessionStorage
# Application Cache
# Cache Stonrage
# IndexedDB
# WebSql
# cookies

# dns-prefetch
# Preload
# Prefetch
# defer
# async


# Object

## 1. Object.assign()
## 2. Object.creat()
## 3. Object.assign()


<font color=#A52A2A size=4 >

# optimization

|Name|Description|
|:---|:----------|
|**minimize**|是否对打包后的代码进行压缩|

# optimization.splitChunks

|Name|Description|
|:---|:----------|
|**chunks**||
|**minSize**|如果有公用模块,此项用于设置公用模块源文件（src文件夹下的文件）的总大小的下限|
|**maxSize**|此项用于设置拆分合并后单个bundle文件（dist文件夹下的文件）的大小的上限，如果超过此数值，继续拆分|
|**automaticNameDelimiter**|此选项允许您指定用于生成名称的分隔符。假设我们生成了一个公用文件名字叫version，class-a,和class-b都依赖他，并且我们设置的连接符是"~"那么，最终生成的就是 version~class-a~class-b.js,当存在匹配的缓存组（后面会说到）时，命名使用缓存组中的name值，若不存在则为  [来源]~[入口的key值].js  的格式|
|**maxAsyncRequests**||
|**maxInitialRequests**|maxSize的优先级高于maxInitialRequest / maxAsyncRequests。 实际优先级为maxInitialRequest / maxAsyncRequests <maxSize <minSize|
|**minChunks**||
|**name**|公用模块合并后的文件名|
|**cacheGroups**||
# optimization.splitChunks.cacheGroups

|Name|Description|
|:---|:----------|
|**priority**||
|**reuseExistingChunk**||
|**test**||
|**chunks**||
|**minSize**||
|**minChunks**||
|**maxAsyncRequests**||
|**maxInitialRequests**||
|**name**||



</font>




[splitChunks]:https://blog.csdn.net/qq_26733915/article/details/79458533 
[splitChunks]:https://www.codercto.com/a/24308.html
[splitChunks]:http://www.likecs.com/show-17716.html
[splitChunks]:https://segmentfault.com/a/1190000015919928
[splitChunks]:https://github.com/liangklfangl/commonsChunkPlugin_Config
[splitChunks]:https://www.cnblogs.com/ufex/p/8758792.html


[tree-shakeing]:
https://vincentdchan.github.io/2018/05/better-tree-shaking-with-scope-analysis/



