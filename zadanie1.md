polecenie do budowania obrazu:
docker build -t server-zad1 .

polecenie do uruchomienia kontenera:
docker run -p 8080:8080 --name container-zad1 server-zad1

polecenie do znalezienia informacji o logach:
docker logs container-zad1

polecenie do sprawdzenia ilosci warstw:
docker inspect server-zad1

polecenie do budowania obrazu na architekturach linux/amd64 oraz linux/arm64 za pomoca docker-container:

docker buildx build -t docker.io/qwe357/zad1:server-zad1 --platform linux/amd64,linux/arm64 --push .
