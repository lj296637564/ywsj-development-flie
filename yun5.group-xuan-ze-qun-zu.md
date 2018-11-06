# yun5.group;选择群组

实例：

```text
// 初始化页面
yun5.group.init(copyCrowdArr || []);
// 控制事件重复注册并获取选择的群组数据
if (addEventInfo.selectGroupPage) {
   addEventInfo.selectGroupPage = false;
   yun5.group.addEvent(function (data) {
      copyCrowdArr = data;
      history.back();
   });
}
```

输入参数：groupList - 选择的群组（Array）

输出参数：选择的群组信息（Array）

