---
layout: page
title: "Git 操作手册"
permalink: /git_handbook/
---

# Git 操作手册

## 什么是版本控制系统

版本控制系统，或称VCS，可以随着人员和团队协作进行项目来跟踪变更的历史。随着项目的发展，团队可以运行测试，修复错误，并贡献新的代码，可以随时恢复任何版本的代码。开发人员可以通过查看项目历史记录来了解：

- 进行了哪些更改？
- 谁做的改变？
- 什么时候做出的改变？
- 为什么需要改变？

## 什么是分布式版本控制系统？

Git是一个分布式版本控制系统（ DVCS ）的示例，它通常用于开放源代码和商业软件开发。DVCS允许对项目的每个文件、分支和迭代的完全访问，并且允许每个用户访问所有更改的完整和自包含的历史记录。与曾经流行的集中版本控制系统不同，像Git这样的DVCS不需要与中央存储库保持恒定的连接。开发人员可以在任何地方工作，也可以从任何时区异步协作。

如果没有版本控制，团队成员会面临冗余任务、较慢的时间表以及单个项目的多个副本。为了消除不必要的工作， Git和其他VCS给每个贡献者一个统一的、一致的项目视图，表面工作已经进行。看到一个透明的变更历史，谁做出这些变更，以及这些变更如何对项目的开发做出贡献，有助于团队成员在独立工作的同时保持一致。

## 为什么是Git？

根据最新的Stack Overflow开发人员调查，超过70%的开发人员使用Git ，使其成为世界上使用最多的VCS。Git经常用于开源和商业软件开发，对个人、团队和企业都有重大好处。

- Git让开发人员在一个地方看到他们的变更、决策和任何项目的进度的整个时间线。从他们访问项目历史的那一刻起，开发人员就拥有了他们理解项目并开始贡献所需的所有上下文。

- 开发人员在各个时区工作。有了像Git这样的DVCS ，协作可以随时进行，同时保持源代码的完整性。使用分支，开发人员可以安全地提出对生产代码的更改。

- 使用Git的企业可以打破团队之间的沟通障碍，并让他们集中精力做好自己的工作。此外， Git使得能够使企业中的专家在重大项目中进行协作。

## 什么是仓库？

存储库（或Git项目）包含与项目关联的文件和文件夹的整个集合，以及每个文件的修订历史。文件历史记录在时间上以快照的形式出现，称为提交，而提交以链表关系的形式存在，并且可以组织成多个开发行，称为分支。因为Git是一个DVCS ，所以存储库是自包含的单元，任何拥有存储库副本的人都可以访问整个代码库及其历史。使用命令行或其他易于使用的接口， git仓库还允许：与历史交互、克隆、创建分支、提交、合并、比较代码版本间的更改等等。

在存储库中工作可使开发项目得到组织和保护。鼓励开发人员修复错误，或者创建新的特性，而不必担心主线开发工作脱轨。Git通过使用主题分支来促进这一点：在历史记录中轻量级提交指针，当不再需要时可以很容易地创建和弃用。

通过GitHub等平台，Git也为项目透明度和协作提供了更多机会。公共存储库帮助团队一起工作，以构建最佳的最终产品。



## Git基本命令

为了使用Git ，开发人员使用特定的命令来复制、创建、更改和合并代码。这些命令可以直接从命令行执行，也可以使用GitHub Desktop或GitKraken等应用程序执行。以下是一些使用Git的常用命令：

- `git init`初始化一个全新的Git存储库，并开始跟踪现有的目录。它在现有目录中添加一个隐藏的子文件夹，该文件夹包含版本控制所需的内部数据结构。

- `git clone`创建远程已存在的项目的本地副本。克隆包括所有项目文件、历史记录和分支。
- `git add`分阶段更改。Git跟踪对开发人员代码库的更改，但是有必要对更改进行暂存和快照，以便将它们包含在项目历史记录中。此命令执行分段，这是该两步过程的第一部分。进行的任何更改都将成为下一个快照的一部分，也是项目历史的一部分。分阶段和提交使开发人员能够完全控制其项目的历史，而不会改变他们的代码和工作方式。
- `git commit`将快照保存到项目历史记录中，并完成更改跟踪过程。简而言之，commit就像拍照一样。任何使用`git add`暂存的东西都会成为`git commit`的快照的一部分。
- `git status`显示更改的状态是未跟踪、修改或暂存。
- `git branch`显示本地正在处理的分支。
- `git merge`将开发线合并在一起。此命令通常用于合并对两个不同分支所做的更改。例如，当开发人员希望将特性分支的更改合并到主分支进行部署时，他们就会合并。
- `git pull`更新本地开发线与更新从其远程对应。如果团队成员已经向远程的分支提交过，并且他们希望在他们的本地环境中反映这些更改，则开发人员会使用此命令。
- `git push`使用本地对分支所做的任何提交来更新远程存储库。

从[Git命令的完整参考指南](https://git-scm.com/docs)中了解更多信息。