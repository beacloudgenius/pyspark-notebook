Run your docker with `docker-compose`. It helps to keep your arguments/settings in a single file and run together in an isolated environment.

Install `docker-compose`
```Python
pip install -U docker-compose
```

To start your apllication. Run following command 
```shell
docker-compose up -d
```

Visit ```http://127.0.0.1:8888```

To stop the service 
```shell
docker-compose stop
```

### Build and run

	docker build -t cloudgenius/pyspark-notebook .

	docker push cloudgenius/pyspark-notebook  

	docker run -d -v /home/cloudgenius/notebook:/notebook -p 8888:8888 cloudgenius/pyspark-notebook:latest 

	docker-compose up -d
	
	firefox ip:8888

### Remember to add to the notebook

	%matplotlib inline