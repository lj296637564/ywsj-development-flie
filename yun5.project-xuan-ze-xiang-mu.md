# yun5.project;选择项目

实例：

```text
				yun5.project.init(false);
				if (!addEventInfo.selectProjectPage) {
					addEventInfo.selectProjectPage = true;
					yun5.project.addEvent(function (res) {
						console.log(res);
	
					});
				}
```

输入参数：

| 参数 | 参数说明 |
| :--- | :--- |
| isMulti | 是否多选（Boolean） |
| projectArr | 选择的项目（单选时传object，多选时传Array） |

输出参数：选择的项目信息

