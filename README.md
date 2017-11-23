# docker-php-dev

基于Docker的PHP开发环境。

### 目录结构如下：

```bash
|____.env-example	环境相关参数配置
|____.gitignore
|____docker-compose.yml
|____mysql
| |____data			MySQL数据文件
|____nginx
| |____conf
| | |____nginx.conf
| | |____vhost		vhost方便多域名绑定
| | | |____default.conf
| |____Dockerfile
| |____logs			Nginx Log目录，便于查看日志
|____php
| |____Dockerfile
|____www			webroot目录
| |____html
| | |____index.php
```


### 使用说明：
	
	Docker版本支持：Docker 17.0+

	Docker编排工具：Docker-compose 1.10+


	步骤：
		```bash
		git clone https://github.com/zhuzhenyu/docker-php-dev.git
		cd docker-php-dev && mv .env-example .env
		sudo docker-compose build
		sudo docker-compose up -d
		```
	最后

		**使用`docker ps -a 或者 docker-compose ps` 看是否正常运行**







