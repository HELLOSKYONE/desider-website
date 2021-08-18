---
title: "联系我们"
date: 2021-07-26T20:14:09+08:00
menu: "footer"
weight: 20
draft: false
---

### 上海斗望工坊科技有限公司

上海市闵行区龙湖虹桥天街购物中心B馆512室（申长路869号）
地铁2号线、10号线、17号线，虹桥火车站站D出口

<style>
    #container {
        overflow: hidden;
        width: 100%;
        height: 500px;
        margin: 0;
    }
</style>
<div class="border rounded"  id="container"></div>
<script src="//api.map.baidu.com/api?type=webgl&v=1.0&ak=mru1CkU69r4eFEDSESpImCmFBn5e2ee8"></script>
<script>
var map = new BMapGL.Map('container');
var point = new BMapGL.Point(121.320207,31.197518);
map.centerAndZoom(point, 17);
var opts = {
    width: 200,
    height: 60,
    title: '斗望工坊'
};
var infoWindow = new BMapGL.InfoWindow('龙湖虹桥天街购物中心B馆（申长路869号）512室', opts);
map.openInfoWindow(infoWindow, point);
function getInfoContent() {
    alert(infoWindow.getContent());
}
</script>