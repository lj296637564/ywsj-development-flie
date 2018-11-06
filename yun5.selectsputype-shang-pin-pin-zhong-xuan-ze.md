# yun5.selectSpuType；商品品种选择

实例：

```text
yun5.selectSpuType.init(
   yun5.getQueryString("typeId"),
   res => {
      console.log(res);
    });
```

输入参数：

| 参数 | 参数说明 |
| :--- | :--- |
| typeId | 商品类型Id（string） |
| fn | 选择后执行的回调函数 |
| chooseMore | 是否多选（Boolean） |
| spuArr | 多选时，已选择的数据（如：\[{spuTitle: '桂花树', spuId: '123'}\]） |

输出参数：选择的商品品种信息（Array）

