## 搜索帮助公用

### open 

* input 配置 2个参数 url，id 

        id 是点击input id 属性，也是fragment名， 这样adddepdent  这个fragment。
        
        url 配置在input上自定义属性，是将来要请求的数据地址 [demo](http://jsbin.com/openui5-customdata-xmlview/1/edit?html,output)
            url 是 app 命名空间的自定义属性(app:url)
        
* 把当前id存入自定义model中， 为了在在关闭时候获取。 
* 执行search方法。  
* [x] 参见 base.controller.js  文件中   onShowCommonHelp 方法中  

### search

* Util.onSearchCommonHelp(oEvent, this, url);
* [x] 参见 base.controller.js 文件 onSearchCommonHelp 方法  
* [x] 以下参见 util.js
* onSearchCommonHelp方法中，通过对获取页面中的参数，对url进行处理，统一请求数据。

### rowSelect

    业务代码，每一个都不同，无法公用。
    
### close

*  取出弹出框id，并关闭 

        取出在open方法存储id
        为了每次弹出都清除之前DOM,清除bug可能点击新的会出现上次搜索帮助。
        执行当前id搜索帮助的close
        
* [x] 参见 base.controller.js  文件中   onCloseCommonHelp 方法中  
