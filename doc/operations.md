# 接口操作

## <a id="user"></a>User Info

<a id="createUser"></a>
### <a id="op2"></a>创建User Info记录
> POST /user

给User Info创建一行新的记录
<!--Content Type-->

<!--Parameters-->
#### 请求参数

参数名|数据类型|必填|参数位置|参数说明
---|:---|:---:|:---:|:---
user|[User](definitions.md#user)|Y|body|user

#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
201|Success|[User](definitions.md#user)|*无*


<a id="queryUser"></a>
### <a id="op3"></a>查询User Info列表
> GET /user

按条件查询User Info的多行记录
<!--Content Type-->

<!--Parameters-->
#### 请求参数

参数名|数据类型|必填|参数位置|参数说明
---|:---|:---:|:---:|:---
select|string|N|query|结果字段选择表达式,具体请看API规范
expand|string|N|query|expand
page_size|integer|N|query|每页返回记录数,默认50,只能结合page使用
page|integer|N|query|第几页,从1开始
limit|integer|N|query|限制返回多少条记录(limit和page不能同时使用)
offset|integer|N|query|从0开始,表示从第几条开始返回,结合limit使用
total|boolean|N|query|是否返回总数,默认返回
orderby|string|N|query|查询结果排序表达式,具体请看API规范
viewId|string|N|query|viewId
filters|string|N|query|查询过滤条件,具体请看API规范
aggregates|string|N|query|聚合字段,具体请看API规范
groupby|string|N|query|分组字段,具体请看API规范
joins|string|N|query|joins

#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
200|Success|[User](definitions.md#user)[ ]|`X-Total-Count` integer : The total count of query records.<br>


<a id="updateUser"></a>
### <a id="op4"></a>更新User Info记录
> PATCH /user/{id}

按主键更新User Info的一行记录
<!--Content Type-->

<!--Parameters-->
#### 请求参数

参数名|数据类型|必填|参数位置|参数说明
---|:---|:---:|:---:|:---
id|integer|Y|path|id
user|[User](definitions.md#user)|Y|body|user

#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
204|Success|*无*|*无*


<a id="deleteUser"></a>
### <a id="op5"></a>删除User Info记录
> DELETE /user/{id}

按主键删除User Info的一行记录
<!--Content Type-->

<!--Parameters-->
#### 请求参数

参数名|数据类型|必填|参数位置|参数说明
---|:---|:---:|:---:|:---
id|integer|Y|path|id

#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
204|Success|*无*|*无*


<a id="findUser"></a>
### <a id="op6"></a>获取User Info记录
> GET /user/{id}

按主键获取User Info的一行记录
<!--Content Type-->

<!--Parameters-->
#### 请求参数

参数名|数据类型|必填|参数位置|参数说明
---|:---|:---:|:---:|:---
id|integer|Y|path|id
select|string|N|query|结果字段选择表达式,具体请看API规范
expand|string|N|query|expand

#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
200|Success|[User](definitions.md#user)|*无*



## <a id="default"></a>未分类

<a id="get"></a>
### <a id="op1"></a>get
> GET /

Just prints 'It works!'.
<!--Content Type-->

<!--Parameters-->
#### 请求参数

*无*
#### 返回结果

状态码|说明|返回值|响应头
:---|:---|:---
200||string|*无*



