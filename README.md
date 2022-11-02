# 1

Aby zbudować opracowany obraz kontenera nalezy wykorzystac polecenie ```docker build -f Dockerfile . --ssh default="C:\Users\nikes\.ssh\id_ed25519" -t lab2.v1```.

Aby uruchomić kontener na podstawie zbudowanego obrazu należy wykorzystać polecenie ```docker run -d -p 8080:8080 --name simple-web-app-container lab2.v1```.

# 2. 

Aby przesłać stworzony obraz do repozytorium DockerHub należy wykorzystać polecenia ```docker login -u nikesz -p <password>```, ```docker commit simple-web-app-container nikesz/lab2.v1``` i ```docker push nikesz/lab2.v1```.