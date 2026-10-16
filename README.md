## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）

---

# 基于SpringBoot+Vue的在线拍卖系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向艺术品、文玩与收藏品在线竞价场景的综合拍卖平台，针对传统线下拍场受地域场次限制、保证金冻结退还不透明、截拍易出现截胡、送拍鉴定与落槌交割流程割裂等问题，把专场与拍品浏览、保证金冻结、阶梯出价与防截胡延时、成交订单交割、收藏家送拍鉴定、关注评价与公告资讯，以及管理员运营大屏整合到同一套前后端分离工程中。

系统采用 SpringBoot + Vue 架构，区分竞买人、收藏家与系统管理员三类角色：竞买人完成浏览竞价与履约；收藏家提交送拍并跟踪鉴定进度；管理员维护拍品专场、评审送拍、监管保证金与出价台账并查看 ECharts 经营指标。关键规则包括有保证金才可出价、加价幅度校验、截拍窗口延时防截胡，以及鉴定通过后一键转正式拍品，适合作为毕设、课设与拍卖电商学习参考。

## 主要功能模块

- **用户认证与角色分流**：竞买人、收藏家、管理员统一登录注册，JWT 鉴权；登录后按角色进入买家前台、送拍工作台或运营中台，管理端路径与接口双重隔离
- **拍品大厅与专场**：按分类、专场、关键词与价格筛选标的；首页推荐专场与热门拍品，详情展示图录、当前价与结拍倒计时
- **保证金与阶梯竞价**：参拍前冻结保证金；出价须高于当前价并满足加价幅度；临近截拍触发防截胡延时，并保留出价轨迹可追溯
- **成交订单交割**：落槌后生成订单，买受人支付尾款，卖家发货与买家签收确认，支持评价晒单闭环
- **收藏家送拍鉴定**：提交藏品信息与实物图，跟踪待审/复鉴/通过/婉拒进度；管理员填写建议价与意见，通过后可一键转入拍品档案
- **关注收藏与公告**：收藏拍品、阅读竞买须知与行业公告，个人中心维护资料、密码与演示余额充值
- **运营数据大屏**：成交额、落槌数、在拍数、注册用户与保证金池等 KPI，以及走势、品类占比等 ECharts 图表
- **拍品与专场中台**：维护图录、起拍价、保留价、加价幅度、保证金与上下架；专场封面、起止时间与推荐标记
- **台账与履约监管**：保证金冻结/退还流水、出价轨迹查询、成交订单发货状态监管
- **评价公告与用户管理**：藏友评价审核回复、公告资讯配置、系统用户启停与角色维护
- **论文与 UML 概览**：配套论文设计实现页拼图与 UML 图列表，便于答辩材料对照

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E6%8B%8D%E5%93%81%E5%A4%A7%E5%8E%85.png" alt="拍品大厅" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E6%8B%8D%E5%93%81%E8%AF%A6%E6%83%85.png" alt="拍品详情" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E6%8F%90%E4%BA%A4%E9%80%81%E6%8B%8D%E9%89%B4%E5%AE%9A.png" alt="提交送拍鉴定" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E6%94%B6%E8%97%8F%E5%AE%B6%E9%80%81%E6%8B%8D%E6%A1%A3%E6%A1%88.png" alt="收藏家送拍档案" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E7%AE%A1%E7%90%86%E5%91%98%E4%BB%AA%E8%A1%A8%E7%9B%98.png" alt="管理员仪表盘" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E6%8B%8D%E5%93%81%E7%AE%A1%E7%90%86.png" alt="拍品管理" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://raw.githubusercontent.com/vvsgxmn/OnlineAuction/main/screenshots/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->
