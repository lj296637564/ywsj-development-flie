# yun5.map\(\);调用高德选择地址

实例：

```text
map = new yun5.map({
   address: [{point: longitude + ',' + latitude}],
   selector: 'container',
   searchInput: 'tipinput',
   resultSelector: 'addText'，
   isCheckAll: true
});
map.init();
```

输入参数object，键名、键值如下：

| 键值 | 键名 |
| :--- | :--- |
| selector | 显示地图的元素Id |
| searchInput | 搜索框的Id值 |
| address | 选择的地址，point：以逗号分隔的经纬度值 |
| resultSelector | 显示详细地址信息的元素Id |
| isCheckAll | 是否多选 |

输出参数：

写一个元素（‘\#submitBtn’）的点击事件获取输出参数，参数如下\(map变量是根据使用说明来使用的\)：

```text
$(document).on('click', '#submitBtn', function () {
   console.log(map);
   addresses = [{
      'longitude': map.pointData.point.split(',')[0],
      'latitude': map.pointData.point.split(',')[1],
      'addressName': map.pointData.clockAddressDetail
   }];
});
```

 A: '单选地址' map.pointData = {

     point: '', // 以逗号分隔的经纬度值

     clockAddressDetail: '' // 详细地址信息

 }

 B: '多选地址' map.selectAddressList = \[{

      point: '', // 以逗号分隔的经纬度值

      clockAddressDetail: '' // 详细地址信息

 }\]

