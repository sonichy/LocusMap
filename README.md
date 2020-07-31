# 轨迹地图网页版
基于百度地图API的轨迹地图
![alt](preview.gif)
## 跨域问题
- Chrome：Access to XMLHttpRequest at 'file:///*.gpx' from origin 'null' has been blocked by CORS policy: Cross origin requests are only supported for protocol schemes: http, data, chrome, chrome-extension, https.  
Chrome 添加启动参数：--allow-file-access-from-files。  
- Firefox：已拦截跨源请求：同源策略禁止读取位于 file:///*.gpx 的远程资源。（原因：CORS 请求不是 http）。  
about:config，security.fileuri.strict_origin_policy = false。

## 注意
若经常使用，请自己申请免费的百度地图 JS API 的Key。

## 问题
- Firefox 只能删除第一个点

## 版本历史
### V3.0 (2020-07)
- 点击轨迹抓取最近点
- 删除点
- 保存轨迹

### V2.0 
- 标记在轨迹上自动移动和控制

### V1.0
- 读取gpx文件，在百度地图上显示轨迹