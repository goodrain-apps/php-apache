# dockerfile for php-apache

## 使用
可以根据具体情况替换默认的 `httpd.conf` 文件。

- 拉取镜像

```bash
docker pull goodrainapps/php-apache:5.6.32
```

- 运行镜像

```bash
docker run -it --rm -p 80:80 goodrainapps/php-apache:5.6.32
```

## 持久化目录
镜像默认使用 `/data` 目录作为web的主目录，请将应用代码存放到该目录下，并修改正确的属主 `chown rain.rain /data -R`

## 支持的参数
镜像支持`debug`和`version` 参数

| 参数 | 说明|
|------|---------|
| debug| 进入容器命令行 |
| version |显示PHP和Apache版本信息|



## 支持的环境变量

暂无