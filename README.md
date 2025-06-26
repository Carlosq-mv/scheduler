### setup for MAC
```shell
# create env
$ python3 -m venv venv

# activate env 
$ source venv/bin/activate

# install 
$ pip3 install -r requirements.txt
```

### setup for Windows
```shell
# install virtualenv
pip install virtualenv

# create env
virtualenv venv

# activate env 
.\venv\Scripts\activate

# install 
pip install -r requirements.txt
```

> Run application: `uvicorn main:app --reload`


### Useful Docker Commands 
```shell
# create and start posgres docker container
$ docker run --name my-postgres -e POSTGRES_PASSWORD=postgres -p 5433:5432 -d postgres

# enter psql
$ docker exec -it my-postgres psql -U postgres

# stop docker container
$ docker stop my-postgres

# start without creating docker container
$ docker start my-postgres

# all docker containers
$ docker ps -a

# all running docker containers
$ docker ps

# build docker image
$ docker build -f Dockerfile -t carlosqmv/ember-alert-scheduler:[tagname] .

# push docker image to docker hub
$ docker push carlosqmv/ember-alert-scheduler:[tagname]

# docker compose cmd
$ docker compose up -d
```
