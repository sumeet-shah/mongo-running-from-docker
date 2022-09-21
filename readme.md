## How to use this project?

- run `docker-compose up -d`  command to bring the mongo db up and running. 
- now we need to attach to the process in which mongo is running. For that execute `docker exec -it docker-running-mongo-mongodbcontainer-1 bash`
- Once that is done, we can then enter into `mongosh` to start the server and run the commands. 
- Run below command to import the attached file into a database.
  
  `mongoimport --db movieData --collection=movies --file=tv-shows.json --jsonArray --drop`

