

## submitFeedback


**接口地址**:
```
测试环境：https://test.cloud.weizhi.com:30052/service/sys/feedback/submitFeedback
生产环境：https://location-safe.cloud.weizhi.com:18888/service/sys/feedback/submitFeedback
```

**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
    "name":"tang",
    "phone":"15120747111",
    "email":"31a231@weizhi.com",
    "content":"这是测试2",
    "industry":"医院",
    "organizationName": "位置网医院"
}
```


**请求参数**:


| 参数名称 | 参数说明 | 数据类型    | 是否必须 |
| -------- | -------- | ----- | -------- |
|&emsp;&emsp;content|留言内容|string|false|
|&emsp;&emsp;email|邮箱|string|false|
|&emsp;&emsp;industry|行业|string|false|
|&emsp;&emsp;name|留言人姓名|string|false|
|&emsp;&emsp;organizationName|组织机构|string|false|
|&emsp;&emsp;phone|手机号码|string|false|


**响应状态**:


| 状态码 | 说明 |
| -------- | -------- |
|0|true|
|50|false|


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code||integer(int32)|integer(int32)|
|message||string||
|success||boolean||


**响应示例**:
```javascript
{
  "code": 0,
  "message": "反馈成功!",
  "success": true
}
{
  "code": 50,
  "message": "重复提交",
  "success": false
}
```
