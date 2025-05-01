# classisland-mgmt-cfg
classisland-mgmt-cfg
# ClassIsland 集控服务配置 - 常熟市浒浦高级中学

![GPL-3.0 License](https://img.shields.io/badge/License-GPL%203.0-blue.svg)

本仓库存储常熟市浒浦高级中学ClassIsland集控服务的配置文件及相关文档，为学校信息化管理提供标准化配置方案。

## 项目简介

本项目包含针对ClassIsland教育管理系统的集中控制服务配置方案，主要功能包括：
- 学校定制化部署的基础配置模板
- 班级设备管理策略配置
- 教学应用白名单配置
- 网络访问控制规则
- 系统更新与维护策略

## 快速开始

### 前置要求
- ClassIsland 服务端 v1.6+
- MySQL/MariaDB 数据库
- Redis 缓存服务

### 配置部署
1. 克隆本仓库：
git clone https://github.com/WFX9485/classisland-mgmt-cfg.git
复制配置文件到部署目录：

2.加入集控
在ClassIsland主文件夹中放入mgmt-CSSXPSH-github.json
运行 ClassIsland。

如果您是第一次运行 ClassIsland，此时 ClassIsland 会弹出欢迎向导。
同意许可协议，然后点击【加入集控】按钮。
此时会弹出集控加入界面，并自动加载了我们刚刚放置在应用目录下的mgmt-CSSXPSH-github.json文件。您可以点击【浏览】按钮选择其它的配置文件。
在 ID 一栏填入{您的班级号}(如115、112等)
ID 在此处可以标识 ClassIsland 实例。在后续的实际应用中，您可以将自定义 id 设置为班级名、教室编号等易于识别的名称。
点击【连接】按钮。
此时应用会下载集控清单文件，速度因网络环境而异。在下载完成后，应用会弹出最后的集控加入确认窗口。
在弹出的确认提示框上，点击【加入】按钮。
在弹出的加入成功提示框上，点击【确定】按钮。
此时应用会重新启动。在重新启动后，进入【应用设置】，您可以看到右上角出现了【由贵单位管理】徽章。
恭喜！您现在已经成功地加入了集控！

主要配置文件
classplans.json - 课程表计划

subjects.json - 科目及任课教师

timelayouts.json - 时间表（全校统一）

Settings.json - 应用设置（默认统一）

manifest.json - 集控连接档案索引文件

policy.json - 策略文件（一致统一，不得更改）

自定义配置
修改策略文件后需执行：

## 后期维护

贡献指南
欢迎通过以下方式参与贡献：

提交Issue报告问题或建议

Fork仓库后提交Pull Request

完善配置文档说明

请确保贡献内容符合GPL-3.0协议要求。

许可证
本项目采用 GNU General Public License v3.0 开源协议，您可以在遵守协议条款的前提下：

自由使用和修改代码

用于商业用途

分发原作品/修改版本

附加条款：基于本项目修改的衍生作品需明确标注原始出处。

联系方式
项目维护：QQ：573963986 @张家瑜 高一15班 
电话：18013070820（住校回复不便）
常熟市浒浦高级中学课岛QQ联络群：1044899787