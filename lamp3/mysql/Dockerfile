##############################################################
# 基于官方 MySQL 镜像制作（系统 Debian 8 jessie）
# VERSION 1.0
# 暴露端口：3306
# 数据文件地址：/var/lib/mysql
##############################################################

FROM mysql:5.6

MAINTAINER whoru.S.Q <whoru.sun@gmail.com>

# 时区设置
ENV TZ=Asia/Shanghai

# 写权限
RUN /bin/cp /usr/share/zoneinfo/$TZ /etc/localtime \
	&& echo $TZ > /etc/timezone \
	&& usermod -u 1000 mysql \
	&& chown mysql.mysql /var/run/mysqld/

