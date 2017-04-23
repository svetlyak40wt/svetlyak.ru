rsync -avz tuna:svetlyak.ru ./
docker build -t svetlyak-mirror .
docker run --rm -ti -p 1080:80 --name svetlyak-mirror svetlyak-mirror
