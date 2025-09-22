# nodejs-ci-cd-demo

Simple Node.js app with CI/CD via GitHub Actions that builds a Docker image and pushes to DockerHub. 
Here are images of tools and methods used to do this task : 

1.Initializing the node.js server and docker from the VS code Application :
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/db87756a-368a-4044-9d14-b101cc8b1a93" />
2. Running the docker image in localhost :
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c3fec9d5-24ae-4b1f-8018-1fc0a61e3fb5" />
3. Running the docker image in docker hub : 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/686da839-ec88-4f9d-a2af-c10272b9ddec" />
4. Reviewing the localhost server using the postman :
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/712e88a2-2477-480e-9665-1841543d7ad9" />
5.Here is the image of the github action run :





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
