# yun5.department2;选择部门和项目

实例：

```text
yun5.department2.init(isMutli, selectedDepart);
				if (!addEventInfo.selectProAndDepartPage) {
					addEventInfo.selectProAndDepartPage = true;
					yun5.department2.addEvent(function (data) {
						
					});
				}
```

输入参数：

| 参数 | 参数说明 |
| :--- | :--- |
| isMutli | 是否多选（Boolean） |
| selectedDepart | 选择的部门数据（Array） |
| isPro | 是否选择项目（Boolean） |

输出参数：选择的部门/项目信息

