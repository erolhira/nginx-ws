# nginx-ws

docker run --name my-nginx -v $(pwd)/reverse-proxy/nginx/nginx.conf:/etc/nginx/nginx.conf -v $(pwd):/nginx-ws -d -p 8080-8083:8080-8083 nginx
docker exec -it my-nginx nginx -s reload
