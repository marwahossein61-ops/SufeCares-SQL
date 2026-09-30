#SufeCares-SQL 校园美食推荐系统

<div align="center">
  <img src="WindowsApp7/WindowsApp7/Resources/logo与背景.png" alt="项目Logo" width="1000"/>
  <p><em>~上财美食，一查便知~</em></p>
</div>

---

## 📋 项目简介

**SufeCares-SQL** 是一款基于 **SQL Server + VB.NET** 开发的校园美食信息查询与推荐系统，由上海财经大学4人团队协作完成。本项目旨在为上财师生提供更便捷的食堂信息查询、菜品浏览与推荐服务，解决“今天吃什么”的日常难题。

---
## 👥 团队介绍

本项目由上海财经大学统计与数据科学学院 **数据科学与大数据技术** 专业4人团队历时2个月协作完成。四位成员分工明确，各司其职，共同完成了从需求分析、数据库设计、前后端开发到系统测试的全流程。

| 头像 | 姓名 | GitHub | 主要负责 |
|:----:|:----:|:------:|----------|
| <img src="https://github.com/AmeliaHistory.png" width="40" height="40" style="border-radius: 50%;"> | **Amelia_History** | [@AmeliaHistory](https://github.com/AmeliaHistory) | • 管理员界面开发<br>• 推荐/排行榜界面开发<br>• 项目意义与选题背景撰写<br>• 图标、背景设计及ER图绘制<br>• 页面美化 |
| <img src="https://github.com/yv5s5hkpr2-design.png" width="40" height="40" style="border-radius: 50%;"> | **yoooooo-2711** | [@yoooooo-2711](https://github.com/yoooooo-2711) | • 今天吃什么页面<br>• 菜品详情页面<br>• 随机生成菜品页面<br>• 评论页面、map页面<br>• 项目不足与经验总结撰写 |
| <img src="https://github.com/Fang-blkbns.png" width="40" height="40" style="border-radius: 50%;"> | **Fang-blkbns** | [@Fang-blkbns](https://github.com/Fang-blkbns) | • **数据库全权负责**：建表、触发器、视图、存储过程<br>• 核心数据注入（100+条测试数据）<br>• 数据库性能优化与完整性控制 |
| <img src="https://github.com/Moolady.png" width="40" height="40" style="border-radius: 50%;"> | **Moolady** | [@Moolady](https://github.com/Moolady) | • 登录/注册/密码模块（登录、用户登录、管理员登录、注册、忘记/修改密码）<br>• 个人中心、我的收藏、我的评论<br>• 校味互鉴、主页面<br>• 系统总体格式统一与美化<br>• PPT制作及报告相关部分 |

> 💡 四位成员均为一作贡献，共同完成了这个项目的需求分析、设计、编码、测试全流程。项目获课程设计90+高分，被用作学弟妹学习参考。

---

## 🛠️ 技术栈

### 开发环境
| 组件 | 技术选型 | 说明 |
|------|----------|------|
| **集成开发环境** | Visual Studio | 提供可视化窗体设计器，支持拖拽式界面开发 |
| **编程语言** | VB.NET | 基于.NET Framework框架，支持事件驱动编程 |
| **版本控制** | Git + GitHub | 四人团队协作，代码开源 |

### 数据库环境
| 组件 | 技术选型 | 说明 |
|------|----------|------|
| **数据库管理系统** | Microsoft SQL Server | 实例名：`2E79\MSSQLSERVER1` |
| **数据库名** | `sufe` | 存储菜品、食堂、用户等核心数据 |
| **数据量** | 6张核心表 + 5000+条测试数据 | 确保系统演示流畅 |

### 核心技术组件
| 技术组件 | 用途 | 实现细节 |
|----------|------|----------|
| **ADO.NET** | 数据访问 | SqlConnection建立连接，SqlCommand执行SQL，SqlDataAdapter填充数据集 |
| **DataSet / DataTable** | 数据绑定 | 与DataGridView联动，实现数据展示与更新 |
| **System.Drawing** | 图形处理 | 图片加载、缩放、自适应显示，提升用户体验 |
| **事件驱动编程** | 交互逻辑 | 按钮点击、窗体加载等事件响应 |

### 数据库高级功能
| 技术组件 | 用途 | 实现细节 |
|----------|------|----------|
| **存储过程** | 业务逻辑封装 | 用户注册/登录验证、找回密码、菜品添加与更新 |
| **触发器** | 数据自动维护 | 用户点赞/点踩时自动更新菜品评分（`TRG_UpdateRatings`） |
| **视图** | 简化查询 | 排行榜视图（`View_DishRanking`）、用户收藏视图（`View_UserFavorites`）、菜品评论视图（`View_DishComments`） |

---
## 📁 项目结构

```
SufeCares-SQL/
├── WindowsApp7/              # 主项目文件夹
│   ├── WindowsApp7/          # 源代码
│   │   ├── My Project/       # 项目配置
│   │   ├── Resources/        # 图片资源
│   │   ├── *.vb              # 窗体代码
│   │   ├── *.resx            # 窗体资源
│   │   ├── WindowsApp7.vbproj
│   │   └── WindowsApp7.sln
│   └── .vs/                  # VS配置（已忽略）
├── Database/                  # 数据库脚本
│   ├── CreateTables.sql      # 建表语句
│   └── InsertData.sql        # 测试数据
├── scriptfinal.sql           # 完整数据库脚本
├── 美食查看信息推荐SufeCares-介绍.pdf
├── 美食查看信息推荐SufeCares-报告.docx
├── README.md
├── .gitignore
└── LICENSE
```
## 📁 SQL-ER图
<div align="center">
  <img src="WindowsApp7/WindowsApp7/Resources/图片5.png" alt="ER1" width="500"/><img src="WindowsApp7/WindowsApp7/Resources/图片6.png" alt="ER2" width="500"/>
</div>
