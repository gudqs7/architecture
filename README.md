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
