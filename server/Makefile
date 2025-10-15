postgresinit:
	docker run --name postgres18 -p 5433:5432 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=password -d postgres:18-alpine

postgres:
	docker exec -it postgres18 psql

createdb:
	docker exec -it postgres18 createdb --username=root --owner=root moonveil

dropdb:
	docker exec -it postgres18 dropdb moonveil


.PHONY: postgresinit postgres createdb dropdb