You should have the docker installed on your machine 
Step 1 : docker run --name my-redis -d -p 6379:6379 redis
Step 2 : docker exec -it container_id /bin/bash
Step 3 : redis-cli

Clone the repo.
Go to the express-backend npm i
To run express backend 
Step 1: tsc -b
Step 2: node dist/index.js

Go to worker 
Step 1: tsc -b
Step 2: node dist/index.js

Then hit with postman the route 
http://localhost:3000/submit
And request body with the value of json 
{
    "problemId":565,
    "code":"387383",
    "language":"hindi"

}
