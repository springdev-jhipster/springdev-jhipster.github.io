---
layout: default
title: Release 6.1.0
---

JHipster v6.1.0 发布
===================

这是 JHipster v6 之后的第一次小版本发布，总共关闭了 [182 个问题单和代码合并请求](https://github.com/jhipster/generator-jhipster/issues?q=milestone%3A6.1.0+is%3Aclosed)。

下面是一些重要的更新：

- 迁移到 Angular 8 版本 - [#9817](https://github.com/jhipster/generator-jhipster/pull/9817)
- 改进 Kafka 支持 - [#9567](https://github.com/jhipster/generator-jhipster/pull/9567)
- 修复复杂区域设置的本地化电子邮件 - [#9722](https://github.com/jhipster/generator-jhipster/pull/9722)
- 新增语言支持：Finnish - [#9843](https://github.com/jhipster/generator-jhipster/pull/9843)
- 为关系型数据库提供 UUID 字段类型 - [#9794](https://github.com/jhipster/generator-jhipster/pull/9794)

其中一些第三方依赖库的升级如下：

- Spring Boot 2.1.5
- Spring Framework 5.1.7.RELEASE
- Spring Security Oauth 2.3.6.RELEASE
- Jhipster Framework v3.0.2
- Jhipster Registry v5.0.2
- NodeJS 10.16.0
- Dropwizard Metrics 4.1.0
- Hibernate 5.3.10.Final
- Infinispan 9.4.14.Final
- Test Containers 1.11.3
- JIB 1.3.0
- ng-jhipster 0.10.1

同时，使用到的 Docker 镜像版本也已升级到最新版本：

- Mongo docker image 4.0.10
- Grafana docker image 6.2.2
- Memcached docker image 1.5.16-alpine
- Mariadb docker image 10.4.5
- Postgres docker image 11.3
- Consul docker image 1.5.1
- Prometheus docker image v2.10.0
- Prometheus operator docker image v0.30.0
- Alertmanager docker image v0.17.0
- Traefik docker image 1.7.12


Closed tickets and merged pull requests
------------
As always, __[you can check all closed tickets and merged pull requests here](https://github.com/jhipster/generator-jhipster/issues?q=milestone%3A6.1.0+is%3Aclosed)__.

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
