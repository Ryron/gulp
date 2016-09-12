# gulp项目中的使用

# 目录
[TOC]

使用gulp也有一段时间了，总结下在前端开发中使用。

### 1.文件目录

```
gulp/
│   ├── dist            "输出文件"
│   │   ├── css              
│   │   ├── html  
│   │   ├── images
│   │   └── javascript    
│   │
│   ├── gulp            
│   │   ├── tasks       "gulp 任务"
│   │   │   ├── default       "默认任务文件夹"
│   │   │   ├── deploy        "部署任务文件夹"
│   │   │   ├── default.js    "默认任务启动js"
│   │   │   ├── deploy.js     "部署任务启动js"
│   │   │   └── sprite.js     "雪碧图js"
│   │   └── config.js   "gulp任务配置"
│   │
│   ├── node_modules    "模块"
│   │
│   ├── src             "需编译的文件"
│   │   ├── html
│   │   ├── images
│   │   ├── javascript
│   │   └── less
│   ├── .gitignore
│   ├── gulpfile.js
│   ├── package.json
│   ├── README.md

```
### 2.gulp主要任务简介
- watch     监听需要编译文件
- default   默认任务，与watch一起用
- deploy    部署前调用，主要是压缩文件
- sprite    雪碧图

### 3.使用插件
| 插件          |    作用          | 备注            |
| :--------     | --------:        | :--:            |
|  browser-sync | 浏览器自动刷新   |                 |
|  gulp-less    | less编译成css    |                 |
|  gulp-cssmin  | css压缩          |                 |
|  gulp-htmlmin | html压缩         |                 |
|  gulp-imagemin| image压缩        |                 |
|  gulp-uglify  | js压缩           |                 |
|  gulp-rename  | 重命名           |                 |
|  gulp-watch   | 监听             |                 |
| gulp.spritesmith| 雪碧图         |                 |
| gulp-fileversion| 版本号         |                 |

### 4.代码
 [链接](https://github.com/Ryron/gulp)
