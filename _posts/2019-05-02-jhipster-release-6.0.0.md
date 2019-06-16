---
layout: default
title: Release 6.0.0
---

JHipster v6.0.0 发布
===================

这是第一次官方正式发布 JHipster v6。

此次发布基于 v6.0.0.beta.0 发布，经过了一个月的 beta 测试，共关闭了 [120 问题单和代码合并请](https://github.com/jhipster/generator-jhipster/issues?q=milestone%3A6.0.0+is%3Aclosed).

一些重要的特性和升级
----------------

* 迁移到 Spring Boot 2.1.x
* 迁移到 Spring Cloud Greenwish.x
* 升级到 Spring Security 5.1 对 OIDC 提供的支持
* 支持 JDK 11 (同时保持兼容 JDK 8+)
* HTML 5 pushstate [#9098](https://github.com/jhipster/generator-jhipster/pull/9098)
* Kubernetes 相关增强 (Istio, Helm)
* 升级到 JUnit 5
* 支持使用 FakerJS 生成实体相关的样例数据 [#9104](https://github.com/jhipster/generator-jhipster/pull/9104)
* 升级到最新 Angular 版本 [#8161](https://github.com/jhipster/generator-jhipster/pull/8161)
* 升级到最新 React 版本
* 支持懒加载 Angular 实体
* 提供 Bootswatch 主题选择
* 删除 CSS 选项 [#9350](https://github.com/jhipster/generator-jhipster/pull/9350)
* 改善与 Sonar 的集成 [#9423](https://github.com/jhipster/generator-jhipster/pull/9423) [#9482](https://github.com/jhipster/generator-jhipster/pull/9482), 提供了外部使用的 sonar-project.properties 文件 
* 支持 Gatling 3，包括一些更好更快的增量构建，以及 BOM 支持
* 集成测试在 Maven 和 Gradle 的单独阶段设置
* 升级到 Gradle 5
* 迁移到 Liquibase 3.6.x
* 升级到 Elastic to 6.4.x
* 升级到 Couchbase 6.x
* 升级到 Infinispan 9.4.x
* 升级到 Cassandra 4.x
* 升级到 Hazelcast 3.11.x
* 输出到控制台的日志采用 JSON 格式
* 默认采用 Jar 形式打包，同时仍然支持输出 War 包 [#9034](https://github.com/jhipster/generator-jhipster/pull/9034)
* 使用 Prettier 来格式化 YAML 文件 [#9281](https://github.com/jhipster/generator-jhipster/pull/9281)
* 使用 Prettier transform 来美化所有的 sub-generators [#9371](https://github.com/jhipster/generator-jhipster/pull/9371)


与此同时，一些特性在这个版本被删除：

* 删除已废弃的 ‘rancher-compose’ sub-generator
* 删除 Chocolatey 和 Homebrew 安装方式，由于它们并没有给用户提供更多好处
* 暂时废弃 [JHipster Devbox](https://github.com/jhipster/jhipster-devbox)：社区正在寻找这部分功能的维护者，如果您感兴趣可以与我们联系！


Closed tickets and merged pull requests
------------
As always, __[you can check all closed tickets and merged pull requests here](https://github.com/jhipster/generator-jhipster/issues?q=milestone%3A6.0.0+is%3Aclosed)__.

How to upgrade
------------

**Automatic upgrade**

For an automatic upgrade, use the [JHipster upgrade sub-generator]({{ site.url }}/upgrading-an-application/) on an existing application:

Upgrade your version of JHipster:

```
npm update -g generator-jhipster
```

And then run the upgrade sub-generator:

```
jhipster upgrade
```

**Manual upgrades**

For a manual upgrade, first upgrade your version of JHipster with:

```
npm update -g generator-jhipster
```

If you have an existing project, it will still use the JHipster version with which it was generated.
To upgrade your project, you must first delete its `node_modules` folder and then run:

```
jhipster
```

You can also update your project and all its entities by running

```
jhipster --with-entities
```

You can also update your entities one-by-one by running again the entity sub-generator, for example if your entity is named _Foo_

```
jhipster entity Foo
```

Help and bugs
--------------

If you find any issue with this release, don't hesitate to:

- Add a bug on our [bug tracker](https://github.com/jhipster/generator-jhipster/issues?state=open)
- Post a question on [Stack Overflow](http://stackoverflow.com/tags/jhipster/info)

If the issue you have is an urgent bug or security issue, please:

- Contact [@java_hipster](https://twitter.com/java_hipster) on Twitter
