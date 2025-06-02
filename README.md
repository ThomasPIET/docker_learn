# docker_DEVOPS

Thomas PIET

3.a -> docker pull nginx
  
  b -> docker images | grep nginx (docker images pour voir toutes les images que j'ai et grep nginx pour rechercher la ligne nginx)

  c -> mkdir -p ./html && touch ./html/index.html 

  d -> docker run --name my-nginx -p 8080:80 -v $(pwd)/html:/usr/share/nginx/html -d nginx

  e -> docker stop my-nginx && docker rm my-nginx

  f -> docker run --name my-nginx -p 8080:80 -d nginx && docker cp ./html/index.html my-nginx:/usr/share/nginx/html/index.html


4.b -> docker build . -t my-nginx

  c -> Je remarque que c'est plus rapide pour tester en environnement dev d'utiliser l'exemple 4. Je pense que l'environnement avec le Dockerfile est plus approprié pour de la prod.
