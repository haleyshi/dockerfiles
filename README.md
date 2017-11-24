# Dockerfile

## nginx

cd nginx
tar zcvf html.tar.gz html
docker build -t="shiguohuang/nginx:v1"
docker run -d -p 80 --name nginx_v1 shiguohuang/nginx:v1

docker ps -a

http://localhost:xxxxx
