# nodejs-ci-cd-demo

Simple Node.js app with CI/CD via GitHub Actions that builds a Docker image and pushes to DockerHub. 
Here are images of tools and methods used to do this task : 

#1.Initializing the node.js server and docker from the VS code Application :

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/52768eb8-d411-45ac-8dba-ff5d8ee310e5" />

#2. Running the docker image in localhost :
   
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c3fec9d5-24ae-4b1f-8018-1fc0a61e3fb5" />

#4. Running the docker image in docker hub :
   
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/58cbbfae-dc50-4b02-90c2-fbc413677359" />

#5. Reviewing the localhost server using the postman :
   
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/712e88a2-2477-480e-9665-1841543d7ad9" />

#5.Here is the image of the github action run :

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/442e4bb6-3160-4ac7-8ad4-c7a8e090cd9e" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/840a0353-4228-434f-8545-50a47225b53e" />


## How it works
- Push to `main` triggers GitHub Actions.
- Actions run `npm ci`, `npm test`, build Docker image, and push to DockerHub.

## Files
- `.github/workflows/main.yml` - CI pipeline
- `Dockerfile` - multi-stage Dockerfile
- `index.js` - sample Express app
- `tests/` - jest/supertest tests

## How to run locally
1. `npm install`
2. `npm test`
3. `docker build -t <your-image> .`
4. `docker run -p 3000:3000 <your-image>`

## Submission
GitHub repo: https://github.com/deepakjaiswal09/nodejs-ci-cd-demo


