
### 请求地址

/api/c/compapi/v2/cc/create_classification/



### 请求方法

POST


### 功能描述

添加模型分类

### 请求参数


#### 通用参数

| 字段 | 类型 | 必选 |  描述 |
|-----------|------------|--------|------------|
| bk_app_code  |  string    | 是 | 应用 ID     |
| bk_app_secret|  string    | 是 | 安全密钥(应用 TOKEN)，可以通过 蓝鲸智云开发者中心 -&gt; 点击应用 ID -&gt; 基本信息 获取 |
| bk_token     |  string    | 否 | 当前用户登录态，bk_token 与 bk_username 必须一个有效，bk_token 可以通过 Cookie 获取 |
| bk_username  |  string    | 否 | 当前用户用户名，应用免登录态验证白名单中的应用，用此字段指定当前用户 |

#### 接口参数

| 字段                       |  类型      | 必选   |  描述                                      |
|----------------------------|------------|--------|--------------------------------------------|
| bk_classification_id       | string     | 是     | 分类 ID，英文描述用于系统内部使用           |
| bk_classification_name     | string     | 是     | 分类名     |
| bk_classification_icon     | string     | 否     | 模型分类的图标,取值可参考，取值可参考[(classIcon.json)](resource_define/classIcon.json)|



### 请求参数示例

```python
{
    "bk_classification_id": "cs_test",
    "bk_classification_name": "test_name",
    "bk_classification_icon": "icon-cc-business"
}
```

### 返回结果示例

```python

{
    "result": true,
    "code": 0,
    "message": "",
    "data": {
        "id": 18
    }
}
```

### 返回结果参数说明

#### data

| 字段       | 类型      | 描述                |
|----------- |-----------|--------------------|
| id         | int       | 新增数据记录的 ID   |