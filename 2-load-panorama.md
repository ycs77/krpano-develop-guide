## 载入全景

**引入脚本（html5渲染器）**

```html
<script src="./tour.js"></script>
```

**创建嵌入容器**

```html
<div id="pano" style="width:100%;height:100%;"></div>
```

**创建对象及配置参数**

```js
embedpano({
  swf:"krpano.swf", // flash渲染器
  xml:"krpano.xml", // 主配置文件   缺省的时候会调用krpano.xml和krpano.swf  不加载设置0即可
  target:"pano", // 嵌入容器id
  id:"krpanoSWFObject", // 当前全景id，javascript接口调用会使用此id
  bgcolor:"#000000",// 背景颜色
  html5:"auto", // html5模式（auto：自动；prefer：优先使用html5；fallback：优先flash；only：只使用html5；always：始终使用html5-仅用于测试；never：始终使用flash；可加上webgl或css3d渲染技术，如auto+css3d）
  flash："auto",// flash模式（auto,prefer,fallback,only,never和html设置类似）
  wmode:"window",// flash模式设置（window：窗口；opaque：不透明；opaque-flash：不透明，仅限flash；transparent：透明的；transparent-flash：透明的，仅限flash；direct：最佳性能，但可能不兼容旧系统和浏览器）
  localfallback:"http://localhost:8090",
  vars:{},// 在xml加载解析后设置启动变量
  initvars：{},// 在xml加载解析前设置启动变量，可以在地址进行查询（our.html?initvars.variable=value）
  basepath:...// 基本路径 （相对于krpano.swf）
  consolelog:false,// 是否在浏览器控制台打印日志信息
  mwheel:true,// 是否启用鼠标滚轮
  focus:true,// 获得焦点
  webglsettings:{preserveDrawingBuffer:false, depth:false, stencil:false},//webgl设置
  mobilescale:0.5, // 移动设备缩放
  fakedevice:"",// "mobile", "tablet", "desktop"；模拟设备 （仅限测试）
  onready:function(){},// 准备就绪回调函数，一般当javascript调用krpano接口的时候，需要在此方法内
  onerror:function(){},// 错误回调函数
  passQueryParameters:true, // 启用url查询参数（ html5, flash, wmode, mobilescale, fakedevice, initvars）作为变量传递，如tour.html?html5=only&startscene=scene2&initvars.design=flat
});
```

**移除全景**

```js
removepano(id);
```

官网文档：https://krpano.com/docu/embedpano/
