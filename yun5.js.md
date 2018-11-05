# yun5.js

1、方法名：yun5.getPageId\(\);

      作用：获取元素（‘.page-current’）上的Id

      输入参数：无

      输出参数：元素（'.page-current'）的Id

2、方法名：yun5.map\(\)；

      作用：调用高德地图选择地址，该方法的使用说明，例如：let map = yun5.map\(object\)

      输入参数：object，键名、键值如下

                           {

                                   address: \[ {} \],   // 对象内的键名为：point，键值为：以逗号分隔的经纬度值

                                   selector:  '',     //  显示地图的元素Id（前缀不要‘\#’号）

                                   searchInput: '',    //   搜索框元素的Id（前缀不要‘\#’号）

                                   resultSelector:  ' ',  //  显示选择地址的信息元素Id（前缀不要‘\#’号）

                                   isCheckAll: boolean    //  是否多选地址，true-是，false-否

                              }

       输出参数：写一个元素（‘\#submitBtn’）的点击事件获取输出参数，参数如下\(map变量是根据使用说明来使用的\)：

                            A: '单选地址'      map.pointData = {

                                                                       point:  '',    // 以逗号分隔的经纬度值

                                                                       clockAddressDetail: ''   //  详细地址信息

                                                         }

                            B: '多选地址'      map.selectAddressList = \[{

                                                                       point:  '',    // 以逗号分隔的经纬度值

                                                                       clockAddressDetail: ''   //  详细地址信息

                                                        }\]

3、方法名

