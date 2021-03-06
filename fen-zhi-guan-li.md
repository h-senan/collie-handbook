# 分支管理
## 分支介绍
- `master`: 当前最新正式版(production服务器)
  - 用于新项目的代码自动生成
- `dev`: 开发服务器版本(develop服务器)
  - 各个开发者的代码再次合并，并处理冲突，测试。
  - 完成集成测试后，将dev分支的推送到master分支。
- `dev_[yourName]_[branchName]`: 开发人员私有分支
  - 用名字来区别各个开发者
  - 供开发者按照自己的习惯来处理分支
  - 例如: `dev_senan`，`dev_senan_login`
- `[projectName]`: 项目线上版分支
- `[projectName]_dev`: 项目开发版分支
  - 用于项目开发，测试

## 常见工作流
### 启动一个新项目
1. 创建分支
  在`master`分支上分出一个项目分支，命名为`[projectName]_dev`。
1. 编写种子文件
  基于设计稿，编写种子文件，并生成基础代码。
1. 整理需求
  核对需求和`master`现有功能，整理出需要完善的地方，将需要完善的地方分为有复用性的和一次性的。
1. 开发组件
  针对有复用性的需求，以component的形式开发，提交到`dev`分支，并最终提交到`master`分支。
1. 更新基础代码
  更新`master`分支，更新基础代码。
1. 定制化开发
  针对一次性的需求，做定制化开发，完成最终代码。
1. 创建正式版分支
  创建正式版分支，并打包代码，上线。

### 修复一个项目的线上bug
1. 获取最新分支
  获取最新的`[projectName]`分支。
1. debug
  分出一个个人分支，用于debug。
1. 提交上线
  将`debug`分支分别提交到`[projectName]`和`[ProjectName]_dev`分支，并更新线上版本。
