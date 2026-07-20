# wecom-bot-helper
企业微信API外部群，支持消息推送、通讯录管理、客户联系等核心接口

[qiwe官网](https:www.qiweapi.com) 

[开发文档](https://doc.qiweapi.com) 

这是一个基于企业微信（WeCom）官方 API 封装的二次开发工具/接口集成项目，旨在帮助开发者快速实现企业微信的自动化与功能对接。

---

## 🌟 核心功能

- [x] **消息推送**：支持文本、卡片、图文、Markdown 等多种类型消息发送
- [x] **通讯录管理**：成员/部门同步与查询
- [x] **客户联系 (SCRM)**：客户列表获取、标签管理、外部联系人回调处理
- [x] **回调解析**：已内置签名校验与消息加解密逻辑

---

## 🚀 快速上手
请求
```
curl -X POST http://manager.qiweapi.com/qiwe/api/qw/doApi
 -H "X-QIWEI-TOKEN: YOUR_API_KEY"
 -H "Content-Type: application/json"
 -d 
 '{
 "method": "/msg/sendText",
 "params": {
 "guid": "你的设备ID",
 "told": "external_user_id",
 "content": "Hello, 你的第一条企微消息"
 }
 }'
```
 响应
```
{
 "code": 0,
 "msg": "success"
}
```
