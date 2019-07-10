# 下载指南
```
git clone --recursive git@github.com:gudqs-architecture/architecture.git
```
由于使用了Git子模块, 所以clone时需添加 `--recursive` 参数, 由于习惯使用了 git 协议,子模块的链接都是git协议, 请各位将电脑的ssh密钥添加到GitHub账号上

## behind
> 里面包含了 base(工具类, 系统包) 和 code-generator (代码生成)

## linux-script
> 里面包含了 Linux 部署所需一切, 如环境安装, 数据库安装, 部署脚本, webhook 服务

## start-template
> 这是一个轻示例(仅一个crud示例), 也是一个项目的起点, 除crud外, 集成的系统板块有用户权限, 系统字典, 省市区数据


## 使用指南
> 首先, 安装 Java, Maven 环境, 然后

### 安装几个项目所需的内部模块(maven依赖)
```
cd behind/base
./install.sh
```

> 然后复制一份 `start-template` 项目, 打开项目(使用 maven 方式)

### 安装数据库
> cd `start-template/src/main/resources/deploy/system/`
依次执行 `2019-04-23-procedure.sql`  --> `2019-04-22-system.sql`  --> `1111-all-menu.sql` --> `2019-05-06-sys-dictionary.sql` --> `1112-all-dictionary.sql`

> 最后, 参考 `start-template/README.md` 文档运行项目, 勾选权限查看系统用户角色管理及 小Demo
