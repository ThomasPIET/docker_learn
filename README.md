# docker_DEVOPS

Thomas PIET

3.a -> docker pull nginx
  
  b -> docker images | grep nginx (docker images pour voir toutes les images que j'ai et grep nginx pour rechercher la ligne nginx)

  c -> mkdir -p ./html && touch ./html/index.html 

  d -> docker run --name my-nginx -p 8080:80 -v $(pwd)/html:/usr/share/nginx/html -d nginx

