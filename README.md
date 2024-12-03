🚀 Project Setup
Follow these steps to set up and run the project:

🛠 Prerequisites
Docker 🐋: Ensure it's installed and running.
Node.js 🌟: Install it to run the project.
📦 Steps


1️⃣ Set Up Redis
1 Run Redis
docker run --name my-redis -d -p 6379:6379 redis  
2 Access Redis
docker exec -it <container_id> /bin/bash  
redis-cli  
2️⃣ Install & Run Express Backend
1 Navigate to express-backend
cd express-backend  
npm install  
2 Build and start
tsc -b  
node dist/index.js  

3️⃣ Set Up & Run Worker
1 Navigate to worker
cd worker  
2 Build and start
tsc -b  
node dist/index.js  

4️⃣ Test the API

Use Postman to send a POST request:
URL: http://localhost:3000/submit
Body:
{  
  "problemId": 565,  
  "code": "387383",  
  "language": "hindi"  
}  

🎉 That's it! You're ready to go! 🚀
