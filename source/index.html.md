---
title: Home

# language_tabs: # must be one of https://git.io/vQNgJ
#   - json: JSON 

toc_footers:
    - <a href='https://hashkeypro.github.io/api'>API home page</a>
    - <a href='https://pro.hashkey.com'>Hashkey Pro Official Site</a>
    
search: true
---

# 1. Preview Environment Overview<br \>&emsp;^预览环境概述

HashKey Pro API Preview Environment is a pre-publish test environment related to API features, in which API users can experience new functions and features as well as verify the compatibility very early. Only users that have been verified can have access to this environment. The version that has completed the test period in preview environment will be released to production environment according to the schedule.

HashKey Pro程序化交易预览环境是有关程序化交易API功能的预发布测试环境，API用户可以在该环境中尽早地进行新功能特性体验及兼容性验证。该预览环境仅接受已认证的API用户地址访问。在预览环境完成测试阶段的版本，将在约定时间点发布至生产环境。

# 2. Become a User for Preview Environment<br \>&emsp;^成为预览环境用户

## 2.1. Get API Access Qualification<br \>&emsp;^获取API接入资格

Please visit
[https://hashkeypro.github.io/api-intro/](https://hashkeypro.github.io/api-intro/)
Get HashKey Pro API access qualification following the document.

请您移步
[https://hashkeypro.github.io/api-intro/](https://hashkeypro.github.io/api-intro/)
按照文档所述方式获取HashKey Pro的API接入资格。

## 2.2. Get Account and Asset<br \>&emsp;^获取预览环境账号和资产

If you have passed API verification, we will create a test account for you in the preview environment and provide the digital assets for your account. Once your test account is ready, our Support team will notify you via email. In the email, an account name and initial password will be provided to you.

Test assets will be deposited from time to time for your test account in the preview environment. The assets cannot be withdrawn to any wallets of any form or test chains.

Currently, the defined maintenance window period is from 1:30 PM to 3:30 PM (UTC+8) every Thursday. During this period, we will perform maintenance procedures like version update, account deposit, which may affect your access to the preview environment.

若您已成功获取API接入资格，我们会及时为您在预览环境开通测试账户并进行测试资产充值。一旦测试账户准备就绪，我们的客服团队会通过邮件提供给您用以登录的用户名和初始密码。

预览环境中会定期为测试账户补充测试资产，其无法被提现至任何正式、测试链上的任何钱包内。

目前，HashKey Pro常规的维护窗口为每周四的1:30PM~ 3:30PM（UTC+8）。在这段期间内，我们可能进行版本升级、账户充值等维护工作，这将可能对您预览环境访问业务的连续性受影响。

# 3. Access to Preview Environment<br \>&emsp;^预览环境接入

You can access the preview environment through the domain [preview-pro.hashkey.com](https://preview-pro.hashkey.com). Please refer to above parts relates to your account name and initial password.

If your host is unable to easily resolve the domain name, you can bind [preview-pro.hashkey.com](https://preview-pro.hashkey.com) with
45.249.244.103 by setting the hosts, then you can proceed to access the request. Before the test, the following prerequisites are necessary:

1. You need to bind your 2FA verification in the preview environment.
2. You need to choose API Key authentication method. The following two methods can be used in parallel:
* Public-Private Mode: This authentication method is based on asymmetric encryption (ECDSA, to be more specific). In this case, the public-private key pair is generated in the user’s browser. The private key is stored locally. Only the public key is uploaded to the server. Therefore, no one but the user has the private key.

* Message Authentication Code Mode: This authentication method is based on symmetric encryption (SHA256, to be more specific). In this case, a secret key is generated in the server and a copy of the key is sent to the user to keep. If you do not want that the secret key is held by the exchange as well, you should choose to use the public-private key pair method.

您可以通过前述的用户名和初始密码访问[preview-pro.hashkey.com](https://preview-pro.hashkey.com)这一站点来登录预览环境。

如果您的主机无法进行域名解析，您可以通过hosts设置来绑定[preview-pro.hashkey.com](https://preview-pro.hashkey.com)与45.249.244.103，然后再进行访问请求。在开始测试前，还需要完成以下前置条件：

(1)您需要在预览环境绑定2FA验证方式；

(2)您需要选择API-KEY授权模式，这两个模式可并行使用：

* 公钥-私钥模式：基于非对称加密的公钥-私钥模式（采用ECC算法），公钥和私钥由客户浏览器生成，私钥由用户保存，交易所仅保存用户提交的公钥信息。本方式可以保证用户的私钥信息仅有其本人保管。

* 消息验证码模式：基于对称加密的消息验证码模式（采用SHA256算法），密钥由交易所服务器生成并下发至用户保存。如用户不希望由交易所保管密钥，可不采用本方式，而是使用公钥-私钥模式。

# 4. Connector References<br \>&emsp;^接口文档

Refer to the link below to know more details about the HashKey Pro connector:
[https://hashkeypro.github.io/api-spec/](https://hashkeypro.github.io/api-spec/)

Refer to the FAQ link below to know more details about the HashKey Pro interface:
[FAQ](https://support.pro.hashkey.com/hc/en-us/search?utf8=%E2%9C%93&query=API)

若您想了解关于HashKey Pro接口的文档，请您移步：
[https://hashkeypro.github.io/api-spec/](https://hashkeypro.github.io/api-spec/)

若您想了解关于HashKey Pro接口的FAQ，请您移步：
[FAQ](https://support.pro.hashkey.com/hc/zh-cn/search?utf8=%E2%9C%93&query=API)

# 5. Preview Environment Regulations<br \>&emsp;^预览环境守则

The preview environment also deploys strategies like threat-awareness strategies, connector traffic limit. In order to provide a stable test environment for you and other users, we will reject all security, performance and traffic testing to be performed.

If a similar behavior occurs, it may be perceived as a malicious action and HashKey Pro will not provide service for you.

预览环境亦部署了威胁感知、接口流量限制等策略，为了保障您与其他用户的测试可以稳定运行，我们谢绝所有对于预览环境的安全测试、性能测试和流量测试。

如若发生类似行为，可能会被系统判定为恶意行为，并拒绝提供服务。

# 6. Listening to Valuable Suggestions<br \>&emsp;^聆听宝贵建议

If you encounter any issues or for any suggestions during the test, you are welcome to contact us through support@pro.hashkey.com. Your email will be carefully handled.

All issues or malfunctions that impact the implementation of your test will be responded within 24 hours to facilitate solution.

在测试过程中有任何问题和建议，都欢迎您发送邮件到support@pro.hashkey.com与我们取得联系，我们将仔细阅读您的来信。

对于影响您测试持续开展测试工作的故障问题，我们会在24小时内作出回复，并为您提供解决方案。