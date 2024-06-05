# 使用官方的Nginx镜像作为基础镜像
FROM nginx:alpine

# 将构建的静态文件复制到Nginx的html目录
COPY dist /usr/share/nginx/html

# 拷贝自定义的Nginx配置文件
COPY /docker/nginx/nginx.conf /etc/nginx/nginx.conf
COPY /docker/nginx/default.conf /etc/nginx/conf.d/default.conf

# 暴露Nginx的默认端口
EXPOSE 80

# 启动Nginx
CMD ["nginx", "-g", "daemon off;"]
