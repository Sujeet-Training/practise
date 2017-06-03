**Start the docker postgreSQL container**

$ docker run --name practise-db -e POSTGRES_PASSWORD=password -d postgres

This spins up a container at localhost port 5432

connect to the application using the db
$ docker run --name some-app --link some-postgres:postgres -d application-that-uses-postgres
