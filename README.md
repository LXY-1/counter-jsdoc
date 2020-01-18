### jsdoc生成的一个js插件说明文档

1. jsdoc配置文件

   ```javascript
   {
       "tags": {
           "allowUnknownTags": false
       },
       "source": {
           "include": ["./src/api","./src/lib"],
           "exclude": [],
           "includePattern": ".+\\.js(doc)?$",
           "excludePattern": "(^|\\/|\\\\)_"
       },
       "plugins": [
          "plugins/markdown"
       ],
       "markdown":{
         "excludeTags":["author"],
         "hardwarp":true,
         "idInHeadings":true
       },
       "templates": {
           "cleverLinks": false,
           "monospaceLinks": false,
           "default":{
               "outputSourceFiles":false,
               "useLongnameInNav":true
           }
       },
       "opts":{
           "template":"docstrap-master/template",
           "encoding":"utf8",
           "destination":"./project-jsdoc/",
           "recurse":true,
           "package":"./package.json",
           "readme":"./read.md"
       }
   }
   ```

2. 使用模板：docstrap，[github项目地址](https://link.jianshu.com/?t=https://github.com/docstrap/docstrap)

3. 关联小项目预览地址:[link](<https://lxy-1.github.io/oop-counter/>)

