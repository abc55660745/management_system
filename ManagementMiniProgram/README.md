# 物资管理小程序后端
##### 由于整套物资管理系统均只有一人开发和维护，代码中多有bug少有注释请见谅，若有其他问题请提issue
### 本程序基于GNU GPL 3.0协议开放源代码，在使用源代码时请务必注意以下几点
1. 任何基于本程序修改或衍生发布的代码应同样使用GPL 3.0协议开放源代码，并在显要位置提及本仓库。
2. 强烈建议其他以任何形式间接接触本程序的代码使用GPL 3.0协议开放源代码，并在文档中提及本仓库。
3. 若您将此代码用于盈利，则必须在显要位置说明此代码可以免费获得。
4. 您使用此代码及其衍生代码造成的一切后果本仓库不负任何责任。

## 联系开发者
本人联系方式
> QQ 3040585972  
> WX abc55660745abc  
> email zuoqingyu@nuaa.edu.cn  

欢迎骚扰（bushi

## 已经实现的功能(需配合后端使用
1. 物资的按种类管理，及物资新建、借出、项目使用、还入、送修、报废全生命流程管理。
2. 普通成员所有操作均需管理员审批，保障安全。
3. 支持条形码扫描，快速对应物品与ID。
4. 支持多地点WIFI定位签到签退、工时计算、请假管理，保证出勤率
5. 所有申请记录可追溯，确定责任人。
6. 重要信息通过mirai推送到QQ群，第一时间掌握信息。

## 配置方式
1. 在微信开放平台注册一个小程序。
2. 进入公众平台->开发管理->开发设置，找到并记录`AppID`与`AppSecret`。
3. 在上述界面，服务器域名中将后端域名加入白名单。
4. 在上述界面，数据预拉取功能设置开发者服务器为`小程序后端地址/backgroundLoad`
4. 在`project.config.json`中找到`appid`并填入第二步的`AppID`。
5. 在`app.js`的底部找到`apiUrl`并修改为自己后端的访问链接。
6. 使用微信开发工具导入工程，上传代码，发布！