# list all of the containers whether running or stopped
$ docker container ls -a
# nothing is listening on port 5432 which is the default port for Postgres
$ telnet localhost 5432

# Persist data by mounting a directory from the host machine
# we don´t want to lose the data each time we rerun a container

# Ubuntu laptop computer
$ ls /pgdata

$ docker container run -d --name=pg -p 5432:5432 -e POSTGRES_PASSWORD=secret -e PGDATA=/pgdata -v /pgdata:/pgdata postgres:11.4
