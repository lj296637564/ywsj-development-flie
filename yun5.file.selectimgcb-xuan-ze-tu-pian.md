# yun5.file.selectImgCb\(\);选择图片

实例：

```text
yun5.file.selectImgCb(addEditAnData.files, 'announcement', $this, true, true);
```

输入参数：

| 参数 | 参数说明 |
| :--- | :--- |
| images | 存储的选择的图片变量（Array） |
| moduleName | 模块名称（string） |
| activeComponent | 选择图片的元素（element） |
| isArr | 是否是数组（Boolean） |
| isTpl | 是否是tpl类型（Boolean） |
| formId | 表单Id（string） |
| maxL | 最多上传图片数量（number） |
| cb | 上传图片后的回调函数 |

输出参数：data - 选择图片的信息

