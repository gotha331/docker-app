docker build \                                                                        
-f ./docker/Dockerfile \
-t "docker-app:latest" . 


docker push gotha331/docker-app:latest