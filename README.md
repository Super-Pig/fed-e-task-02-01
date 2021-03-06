# fed-e-task-02-01 简答题答案

# 1. 谈谈你对工程化的初步认识，结合你之前遇到过的问题说出三个以上工程化能够解决问题或者带来的价值

## 答：

前端工程化是遵循一定的标准和规范，通过工具来提高效率，降低成本的一种手段

前端工程化可以解决的问题：

开发阶段：

- 想要使用 ES6+ 、Less/Sass、模块化开发这些新特性，但是运行环境不能支持，可以用工程化工具对这些兼容性问题的代码进编译，转换成被支持的代码

- 通过脚手架工具自动完成基础结构的搭建，创建特定类型的文件，可以硬性约束大家的编码规范和项目结构；避免不同的人基于各自的爱好创建个性化的代码结构和编码风格，以致于以后代码交接给他人维护的过程中理解成本很高

预览/测试/联调阶段：

- 可以使用工程化工具提供的开发环境web server来对项目进行预览，解除对服务端的web server（比如nginx或者其他web资源服务器）的依赖；通过模块热更新来提升测试和debug的效率；

- 在联调阶段，可以预先和服务端开发团队约定好接口文档，然后利用mock工具生产假接口和假数据，便于前端闭环开发联调，也使前后端可以并行开发，在后端接口开放出来前项目进度不会block

代码提交阶段：

- 可以使用githook和lint工具对代码规范和 git commit 进行强约束和管控；可以保证团队成员提交的代码风格保持一致；可以保证提交记录有明确的注解，便于后续的版本回滚

部署阶段：

- 集成 CI/CD, 一键部署，自动发布；通过工程化方式让繁杂的代码打包、压缩、上传，代码版本回滚等繁杂操作透明化，使用机器自动完成，提升效率同时也避免认为操作过程中可能会出现的错误

# 2. 你认为脚手架除了为我们创建项目结构，还有什么更深的意义？

## 答： 

- 脚手架工具可以创建项目基础结构、提供项目规范和约定；
- 可以减少重复性的工作；可以约束团队开发成员采用相同的组织结构、相同的开发范式、相同的模块依赖、相同的工具配置、相同的基础代码，以便于降低后期由于组织架构调整或者人员流动带来的维护成本；
- 可以让代码结构设计透明化，让开发人员专注于业务开发