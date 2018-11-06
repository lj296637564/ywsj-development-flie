# yun5.DepartmentFilter\(\);部门筛选

实例：

```text
								let area = new yun5.DepartmentFilter({
									data: departmentData,
									departArr: [],
									selector: $('#departmentList'),
									cb: (a, b) => {
										$('#departmentList').addClass('hide');
										$('#department').removeClass('color-blue');
										filterFun(a);
										pageIndex = 1;
										getData();

									}
								});
								area.init();
```

输入参数：

| 参数 | 参数名称 |
| :--- | :--- |
| opt.data | 部门数据 |
| opt.departArr | Array |
| opt.selector | 展示部门的元素（element） |
| cb | 回调函数 |

输出参数：选择的部门信息

