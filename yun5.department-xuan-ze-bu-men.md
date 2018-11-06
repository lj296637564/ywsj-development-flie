# yun5.department；选择部门

实例：

```text
		// 初始化部门数据
			yun5.department.init();
				if (changeDepartment) {
					changeDepartment = false;
					yun5.department.addEvent(function (data) {
						addData.orgName = data.orgName;
						addData.orgId = data.orgId;
					});
				}
```

输入参数：无

输出参数：选择的部门信息

