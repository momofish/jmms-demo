# 模型定义

## <a id="error"></a>Error
服务端返回的错误信息

#### 属性定义

属性名|数据类型|必填|属性说明
---|:---|:---:|:---
code|string|N|错误代码
message|string|N|错误描述

## <a id="user"></a>User Info (*User*)


#### 属性定义

属性名|数据类型|必填|属性说明
---|:---|:---:|:---
id|integer|N|主键
firstName|string|Y|
lastName|string|Y|
loginName|string|Y|
password|string|Y|
gender|string|N|
birthday|string|N|
createdAt|string|N|创建时间
updatedAt|string|N|更新时间

