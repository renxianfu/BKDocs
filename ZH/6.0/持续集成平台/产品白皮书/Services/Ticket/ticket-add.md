# 创建凭证页

在流水线运行期间，你可能需要很多种凭据类型在拉取代码库、调用代码库 API、通过账号密码访问第三方服务时使用。

![png](../../assets/service_ticket_add.png)

目前支持以下几种凭据类型：
类型 | 描述
--- | ---
密码 | 定义后会作为流水线变量在各种插件中引用
用户名+密码 | 一般在关联 SVN 代码库时用到
SSH 私钥 | 关联 GitLab 代码库时（不需要 GitLab 事件触发）使用
SSH 私钥+私有 Token | 关联 GitLab 代码库时（需要 GitLab 事件触发）使用
用户名密码+私有 token | 关联 GitLab 代码库时（需要 GitLab 事件触发）使用

## 接下来你可能需要

* [查看凭据](ticket-list.md)