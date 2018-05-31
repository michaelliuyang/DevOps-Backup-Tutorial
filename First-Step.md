# 第一阶段
所谓第一阶段，是指在Team实施DevOps初期，很多流程工具都需要资源和时间进行Build，但是由于各种资源限制或者上线压力，我们需要分部Build DevOps体系，
在第一阶段，先打好基础，把DevOps的流程Build全，但是在细化和工具上，可能有所欠缺，在后面的阶段去Update他。

第一阶段主要包含

### 基础全流程Build
* Project Manager: 规范文档，Wiki和Jira的使用规范，敏捷方式（看板还是瀑布）
* DevOps Tools Env Build: 各种DevOps工具的搭建和管理(Git / SonarQube / Nexus / Jenkins / Wiki & Jira)
* Flow Build: Git -> Code Review -> CI & CD -> Monitor

#### Docker
几乎所有的工具和服务，都可以[Docker](https://www.docker.com)化，所以我们先要一个Docker环境，进行一些必要的Docker配置，让我们的DevOps有一个良好的基础
* [Docker Install&Config](https://michaelliuyang.github.io/docker/2017/05/31/docker-install.html)
* 搭建Docker私有仓库，[TODO Build](http://xxx)

#### Project Manager
一个好的项目管理流程，可以省很多沟通成本，这里面采用一些工具是很有必要的，工具方面首选的是Atlassian公司旗下的项目管理工具集合包含了

PS: Atlassian都可以破解，由于都是Java的，所以泡在Docker也不难，后面介绍每一种Docker的搭建方式

- [Wiki](https://www.atlassian.com/software/confluence)文档管理工具，[TODO Build](http://xxx)
- [Jira](https://www.atlassian.com/software/jira)项目管理工具，[TODO Build](http://xxx)
- [Crowd](https://www.atlassian.com/software/crowd)账号认证管理工具，[TODO Build](http://xxx)

#### Git
* Git Branch Model: 每个Team都有自己的分支管理方式，和业务场景，团队氛围有很大关系，这里哟一篇介绍Git Branch Model的文章，
比较经典和通用，[Branch Model](https://nvie.com/posts/a-successful-git-branching-model)
* Git Commit Message: 每次的提交记录，应该遵循一定的规范，让每次提交都变得规范有意义，一目了然，
目前常用的git提交工具是[commitizen](https://github.com/commitizen/cz-cli)；检查提交Message是否规范工具[validate-commit-msg](https://github.com/conventional-changelog/conventional-changelog)；导出Change Log工具[conventional-changelog](https://github.com/conventional-changelog/conventional-changelog)
* Gitlab，[TODO Build](http://xxx)

#### Code Review
* [SonarQube Install&Config](https://michaelliuyang.github.io/projectsupport/2016/09/11/build-sonarqube-env.html)
* Code Review Meeting

#### CI & CD
* Jenkins

#### Monitor
* xxx
* xxx
