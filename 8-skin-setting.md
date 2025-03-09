## skin_setting

```xml
<!-- skin_setting 自定义元素，默认皮肤的参数设置-->
maps="false"  <!-- 是否使用必应地图或谷歌地图 -->
maps_type="bing"  <!-- 选择使用谷歌地图或必应地图 -->
maps_bing_api_key=""   <!-- 必应地图所需的API密钥，需申请 -->
maps_google_api_key=""   <!-- 谷歌地图所需的API密钥，需申请 -->
maps_zoombuttons="false"   <!-- 是否在地图上显示缩放按钮 -->
gyro="true"   <!-- 是否使用陀螺仪 -->
webvr="true"    <!-- 是否启用VR -->
webvr_gyro_keeplookingdirection="false" <!-- 进入陀螺仪或VR时是否保持观看方向 -->
webvr_prev_next_hotspots="true"  <!-- 在VR下是否启用导航到前后场景的链接热点-->
littleplanetintro="false"    <!-- 是否使用小行星开场 -->
title="true"  <!-- 是否左下角显示title -->
thumbs="true"  <!-- 是否使用缩略图，如不使用，则没有缩略图一栏 -->
thumbs_width="120" thumbs_height="80" thumbs_padding="10" thumbs_crop="0|40|240|160"  <!-- 缩略图宽度、高度、间距以及缩略图裁切范围 -->
thumbs_opened="false"   <!-- 是否在启动时弹出缩略图一栏 -->
thumbs_text="false"  <!-- 是否在缩略图上显示名字 -->
thumbs_dragging="true"   <!-- 是否允许鼠标拖拽缩略图区域 -->
thumbs_onhoverscrolling="false"  <!-- 是否允许鼠标悬停缩略图自动滚动 -->
thumbs_scrollbuttons="false"   <!-- 是否显示缩略图滚动按钮 -->
thumbs_scrollindicator="false"   <!-- 是否显示缩略图滚动条 -->
thumbs_loop="false"  <!-- 滚动按钮是否使用缩略图循环 -->
tooltips_buttons="false" <!-- 鼠标在按钮悬停时是否弹出文字提示 -->
tooltips_thumbs="false"  <!-- 鼠标在缩略图悬停时是否弹出文字提示 -->
tooltips_hotspots="false"   <!-- 鼠标在热点上悬停时是否弹出文字提示 -->
tooltips_mapspots="false"   <!-- 鼠标在地图热点悬停时是否弹出文字提示 -->
deeplinking="false"       <!-- 是否使用深度链接获取功能，可使得当前页面路径获取场景及视角信息 -->
loadscene_flags="MERGE"  <!-- 缩略图切换场景时的变量 -->
loadscene_blend="OPENBLEND(0.5, 0.0, 0.75, 0.05, linear)"  <!-- 缩略图切换场景时的融合 -->
loadscene_blend_prev="SLIDEBLEND(0.5, 180, 0.75, linear)"  <!-- 缩略图切换到上一个场景时的融合 -->
loadscene_blend_next="SLIDEBLEND(0.5, 0, 0.75, linear)"  <!-- 缩略图切换到下一个场景时的融合 -->
loadingtext="载入中..." <!-- 在全景图载入中时显示的文字 -->
layout_width="100%"  <!--导航条容器相对屏幕宽度的百分比 -->
layout_maxwidth="814"  <!--导航条容器的最大宽度像素 -->
controlbar_width="-24" <!--导航条背景的宽度像素 -->
controlbar_height="40"  <!--导航条背景的高度像素 -->
controlbar_offset.normal="20"  <!--导航条背景与屏幕底部的距离-->
controlbar_offset_closed="-40"  <!--导航条隐藏状态时与屏幕底部的距离-->
controlbar_overlap.no-fractionalscaling="10"  <!--在不支持分级缩放页面和设置像素比的设备的导航条重叠的像素-->
controlbar_overlap.fractionalscaling="0" <!--支持分级缩放页面和设置像素比的设备的导航条重叠的像素-->
design_skin_images="vtourskin.png" <!--皮肤所用的源图片-->
design_bgcolor="0x000000" <!--皮肤的背景颜色-->
design_bgalpha="0.5" <!--皮肤的透明度-->
design_bgborder="0 0xFFFFFF 1.0" <!--皮肤的边框-->
design_bgroundedge="1" <!--皮肤边框圆角设置-->
design_bgshadow="0 0 9 0xFFFFFF 0.5" <!--皮肤的背景阴影-->
design_thumbborder_bgborder="4 0xFFFFFF 1.0" <!--皮肤的缩略图边框-->
design_thumbborder_padding="2" <!--皮肤缩略图边框间距-->
design_thumbborder_bgroundedge="5" <!--皮肤缩略图边框的圆角-->
design_text_css="color:#FFFFFF; font-family:Arial; font-weight:bold;"<!--皮肤文字样式-->
design_text_shadow="1" <!--皮肤的文字阴影-->

<!-- 如果你要更改皮肤样式，你可以改变上面的skin_settings数值，或者选择性地include下面一个预设的设计，可以通过移除特定include元素的if属性或者在html文件的embedpano()中增加initvar:{design:’flat_light’}。 -->

<include url="skin/vtourskin_design_glass.xml"       if="design === 'glass'"       />
<include url="skin/vtourskin_design_flat.xml"        if="design === 'flat'"        />
<include url="skin/vtourskin_design_flat_light.xml"  if="design === 'flat_light'"  />
<include url="skin/vtourskin_design_ultra_light.xml" if="design === 'ultra_light'" />
<include url="skin/vtourskin_design_117.xml"         if="design === '117'"         />
```
