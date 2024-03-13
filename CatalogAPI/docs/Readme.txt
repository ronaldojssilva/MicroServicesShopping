docker run -d -p 27017:27017 --name catalog-mongo mongo

docker exec -it catalog-mongo /bin/bash
docker exec -it catalog-mongo bash
mongosh ou mongo
show dbs
use ProductDb
db.createCollection('Products')
db.Products.insertOne({"Name":"Caderno 2", "Category":"Material Escolar", "Image":"caderno.jpg", "Price":7})
db.Products.find({}).pretty()
show collections
db.Products.remove({}) ou db.Products.deleteMany({})

Redis
	docker run --name local-redis -p 6379:6379 -d redis
	docker exec -it local-redis sh
	executa a interface de linha de comando do Redis
	#redis-cli
	 set name bem-vindo
	get name
	ping
	incr contador
	get contador

	olha o basket
		type ronaldo
		hgetall ronaldo