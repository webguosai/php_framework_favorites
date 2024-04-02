# php高性能框架收藏

## 框架对比

- 整理时间：2024.04.02

| 框架                                                         | 类型                                                         | 地址                                                         | 维护频率/提交数 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | --------------- |
| webman ![Github stars](https://img.shields.io/github/stars/walkor/webman.svg) | workerman  | [仓库](https://github.com/walkor/webman)  [文档](https://webman.workerman.net/doc/zh-cn/) | 3周前 / 325     |
| hyperf ![Github stars](https://img.shields.io/github/stars/hyperf/hyperf.svg) | swoole  | [仓库](https://github.com/hyperf/hyperf)  [文档](https://hyperf.wiki/3.1/#/zh-cn/quick-start/install) | 23分钟前 / 8145 |
| easyswoole ![Github stars](https://img.shields.io/github/stars/easy-swoole/easyswoole.svg) | swoole  | [仓库](https://github.com/easy-swoole/easyswoole)  [文档](https://www.easyswoole.com/QuickStart/environment.html) | 上周 / 1604     |
| swoft ![Github stars](https://img.shields.io/github/stars/swoft-cloud/swoft.svg) | swoole  | [仓库](https://github.com/swoft-cloud/swoft)  [文档](https://www.swoft.org/documents/v2/quick-start/install/) | **2年前** / 1328 |
| Simps ![Github stars](https://img.shields.io/github/stars/simple-swoole/simps.svg) | swoole  | [仓库](https://github.com/simple-swoole/simps)  [文档](https://doc.simps.io/#/zh-cn/install) | **2年前** / 110 |
| fomo ![Github stars](https://img.shields.io/github/stars/fomo-framework/fomo.svg) | swoole  | [仓库](https://github.com/fomo-framework/fomo)  [文档](https://fomo-framework.github.io/docs/) | **2年前** / 330 |
| imi ![Github stars](https://img.shields.io/github/stars/imiphp/imi.svg) | 不限 | [仓库](https://github.com/imiphp/imi)  [文档](https://doc.imiphp.com/v2.1/base/new.html) | 2周前 / 3787  |
| mixphp ![Github stars](https://img.shields.io/github/stars/mix-php/mix.svg) | 不限 | [仓库](https://github.com/mix-php/mix)  [文档](https://openmix.org/mix-php/docs/3.0) | 3周前 / 2640 |
| Laravel-Swoole ![Github stars](https://img.shields.io/github/stars/swooletw/laravel-swoole.svg) | swoole  | [仓库](https://github.com/swooletw/laravel-swoole)  [文档](https://github.com/swooletw/laravel-swoole/wiki) | **1年前** / 793 |
| laravel-s ![Github stars](https://img.shields.io/github/stars/hhxsv5/laravel-s.svg) | swoole  | [仓库](https://github.com/hhxsv5/laravel-s)  [文档](https://github.com/hhxsv5/laravel-s) | 2周前 / 1772     |

### hyperf 

- Hyperf 是一个基于 Swoole 扩展的高性能框架，提供了依赖注入容器、AOP 面向切面编程、协程 MySQL 客户端等功能，适合构建高性能的 Web 应用。

### Swoft

- Swoft 是一个基于 Swoole 扩展的微服务框架，支持微服务治理、服务注册与发现、负载均衡等功能，类似于 Spring Cloud。

### Easyswoole

- Easyswoole 是一个开发简单、性能优秀的基于 Swoole 的框架，提供了 HTTP 服务器、TCP 服务器、自定义进程等功能，适合快速构建高性能的网络应用。

### simps

- 简单的 `Swoole` 框架

## 压测

- 压力测试排名：https://web-frameworks-benchmark.netlify.app/result?l=php
- `-n 800` 请求 800 次
- `-c 100` 100 个并发请求

```bash
ab -n 800 -c 100 -k http://127.0.0.1:8080/
```
