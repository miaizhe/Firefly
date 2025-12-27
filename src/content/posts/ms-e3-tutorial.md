---
title: 'Microsoft 365 E3 订阅保姆级教程：免费拿下 5T OneDrive (附风险提示)'
published: 2025-12-27
description: '整合多方教程，教你如何申请免费的 Microsoft 365 E3 订阅并扩容至 5T OneDrive，同时包含重要的风险避坑指南。'
image: './images/ms-e3.png'
tags: [Microsoft 365, E3, OneDrive, 教程, 羊毛]
category: '技术分享'
draft: false
---

## 📢 前言

最近微软又放出了 **Microsoft 365 E3 Developer** 的订阅“福利”，虽然 E5 开发者订阅已经封车很久，但这次 E3 的回归给了不少错过的同学一个上车的机会。本文将结合 AcoFork 和奶昔论坛的多方教程，整理出一份完整的申请与扩容指南。

> **⚠️ 特别提醒**：此次 E3 订阅疑似微软后端配置失误（特别是 Symphony 版本），存在极高的翻车风险。请务必阅读文末的 **风险提示**。

---

## 🛠️ 第一步：注册全局管理员账号

如果你已经有 M365 管理中心账号（即便 E5 已经过期被 ban），可以直接跳到第二步。

![注册页面 - 1](./images/ms-e3-1.png)
![注册页面 - 2](./images/ms-e3-2.png)
![注册页面 - 3](./images/ms-e3-3.png)
*选择正确的地区（CN）是成功的关键，扫码后即可进入管理中心*

1.  **访问注册页面**: [点击进入 Microsoft 365 注册页](https://signup.microsoft.com/get-started/signup?products=35dffc92-9eb4-4d5c-82c2-2582b37bb9c4&culture=zh-cn&country=cn)
2.  **填写信息**: 按照提示一路“下一步”。
3.  **关键点**:
    - **国家/地区**: 务必选择 **CN (中国)**，否则后续无法使用支付宝，需要绑定外币信用卡。
    - **纳税人识别号**: 随便填或认真编一个。
    - **地址**: 建议精确到区县。
4.  **跳过绑卡**: 到达绑卡步骤时，直接退出或关闭页面。使用你刚刚注册的 `xxx@xxx.onmicrosoft.com` 账号登录 [Microsoft 365 Admin Center](https://admin.microsoft.com/) 即可。

---

## 💰 第二步：购买（白嫖）E3 订阅

![购买订阅 - 1](./images/ms-e3-4.png)
![购买订阅 - 2](./images/ms-e3-5.png)
![购买订阅 - 3](./images/ms-e3-6.png)
*确认订单金额为 $0.00，选择支付宝扫码即可白嫖*

1.  **访问购买链接**: [Office 365 E3 Developer 购买页](https://admin.cloud.microsoft/?pid=C69E7747-2566-4897-8CBA-B998ED3BAB88&quan=25&bc=1&sku=189a915c-fe4f-4ffa-bde4-85b9628d07a0&ru=PDP#/Purchase/checkout)
2.  **设置数量**: 在许可证数量处填写 **25** 个（即便填 25 个，总额依然应显示为 **$0.00**）。
3.  **支付方式**: 选择“添加新付款方式”，如果你的账号区域是 CN，此时会看到 **支付宝** 选项。
4.  **完成下单**: 扫码验证（可能会扣除 1 元进行验证，随后会退回）。
5.  **改为年付**: 在 `账单 > 你的产品 > Office 365 E3 Developer` 中，将月付改为 **按年支付**，以减少风控。

---

## 📦 第三步：扩容 OneDrive 至 5TB

![OneDrive 扩容 - 1](./images/ms-e3-7.png)
![OneDrive 扩容 - 2](./images/ms-e3-8.png)
![OneDrive 扩容 - 3](./images/ms-e3-9.png)
![OneDrive 扩容 - 4](./images/ms-e3-10.png)
*进入 SharePoint 管理中心，将存储限制手动修改为 5120 GB*

默认情况下，订阅提供的 OneDrive 空间为 1TB。

1.  **进入管理中心**: 在左侧菜单点击“全部显示”，选择 **SharePoint** 管理中心。
2.  **更改设置**:
    - 导航到 `设置 > OneDrive > 存储限制`。
    - 将默认限制修改为 **5120 GB** 并保存。
3.  **手动强制扩容 (针对老用户)**:
    - 如果保存后没变化，回到“活跃用户”，选择对应账号。
    - 在“OneDrive”选项卡下，选择“管理角色”或直接在存储部分点击“编辑”，强制手动修改上限。

---

## 🚨 风险提示与避坑指南 (必读)

在决定长期使用前，请务必了解以下几点：

### 1. 尽量避开 Symphony 版本
奶昔论坛等多方反馈建议不要碰 **Symphony** 版本（即便它显示可以订阅 200 万个许可）。这种异常的数据极易触发微软的清理脚本。

### 2. 不要污染“老全局”
如果你手里有珍贵的 **MSDN E3** 或正在使用的教育版/公益版全局，**千万不要** 在同一个租户下订阅这次的羊毛 E3。微软运维一旦开始清理，可能会连累整个租户下的所有订阅。

### 3. 数据备份是第一要务
由于这次订阅极大概率是微软印度运维的失误，随时可能“翻车”被封。
- **不要** 存储不可替代的唯一数据。
- **必须** 配合 Rclone 或其他工具进行多地备份。

### 4. 账户安全
及时前往 [My Sign-Ins](https://mysignins.microsoft.com/security-info) 绑定 MFA（多重身份验证）和备用邮箱，防止因安全风控导致账号丢失。

---

## 🔗 参考资料

- [AcoFork Blog - 永久免费OneDrive 5T，MS 365 E3保姆级拿下教程！](https://blog.acofork.com/posts/ms-e3/)
- [奶昔论坛 - 微软Office365 E3订阅回归？25个E3 Dev免费开通指南](https://forum.naixi.net/thread-6702-1-1.html)
- [奶昔论坛 - 垃圾Dev！Office E3 Symphony可以订阅200万个授权许可](https://forum.naixi.net/forum.php?mod=viewthread&tid=6723)
