# gulp构建工具
前端自动化构建工具:
打包工具，可以生成相应目录和代码，同时对项目进行编译。一次安装，到处运行

##功能一览

###编译预览

- [x] Sass/less 编译
- [x] CSS兼容、检查、合并、压缩
- [x] 文件内联
- [x] 页面html编译、压缩、清除注释
- [x] JS检查、合并、压缩
- [x] 自动生成雪碧图
- [x] 自定义图片转base64
- [x] 图片压缩
- [x] CDN
- [x] 文件MD5戳
- [x] 本地监听预览

##安装

项目结构

一个项目对应多个目录<br>
    ├── branches             - 分支目录<br/>
    ├── dist                 - 打包目录<br>
    ├── path                 - 开发目录<br>
    ├── config               - 项目的配置信息<br>
    └── remark.txt           - 打包备注<br>
    
开发中模块将由以下结构组成<br>
    ├── css                     - 通过编译生成的css目录<br/>
    │<br/>
    ├── html                    - 通过编译生成的html目录<br/>
    │<br/>
    ├── images                  - 静态页面使用的image，不打包<br>
    │<br> 
    ├── img                     - 需打包文件，具体根据项目自配<br>
    │   ├── icon                - css里的image<br>
    │   ├── dialog              - 弹出框模块<br>
    │   ├── user                - 会员模块image<br>
    │   ... <br>
    │<br>   
    ├── js                       - js目录，具体根据项目自配<br>
    │   ├── plugins              - 第三方框架/库<br>
    │   ├── common               - 全局方法<br>
    │   ├── index                - 首页模块js文件<br>
    │   ├── user                 - 会员模块js文件<br>
    │   ...<br>
    │   ├── config.js            -js配置信息<br>
    │<br>
    ├── sass/less<br>
    │   ├── base                  - css底层<br>
    │   ├── common                - 通用css<br>
    │   ├── ui                    -模块css<br>
    │   ├── all.scss<br>
    │<br>
    ├── template<br>
    │   ├── inc                   - 公用<br>
    │   ...<br>
    │<br>
    └── index.html                - 中转页<br>
