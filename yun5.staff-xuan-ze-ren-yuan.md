# yun5.staff;选择人员

实例：

```text
// 控制初始加载人员数据
if (controlDataLoading.selectStaffOnOff) {
   controlDataLoading.selectStaffOnOff = false;
   yun5.staff.addEvent();
}
let json = {};
if (groupId) {
   json = {'fromWhere': 'noticeModel', groupId: groupId || ''};
}
// 选取后的数据
yun5.staff.init(true, selectSatffList || [], function (data) {
   selectSatffList = data;
   for (let i = 0; i < selectSatffList.length; i++) {
      if (i === 0) {
         addEditAnData.staffIds = selectSatffList[0].memberCode;
         addEditAnData.staffNames = selectSatffList[0].staffName;
      } else {
         addEditAnData.staffIds = addEditAnData.staffIds + ',' + selectSatffList[i].memberCode;
         addEditAnData.staffNames = addEditAnData.staffNames + '、' + selectSatffList[i].staffName;
      }
   }
   history.back();
}, 0, '', '', '', true, json);
```

输入参数：

| 键值 | 键名说明 |
| :--- | :--- |
| isMulti | 是否多选（Boolean） |
| selectedStaff | 选择的员工（Array） |
| cb | 回调函数 |
| isSelf | 是否选择本人（0-可以选择本人） |
| selectStaffIds | 选择的员工id，以逗号分隔字符串 |
| companyCode | 公司Id |
| isCloud |  |
| isSelectAll | 是否多选（Boolean） |
| otheropt | 其他参数（obj） |

输出参数：选择的用户信息

