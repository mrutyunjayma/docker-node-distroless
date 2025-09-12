📦 My Node.js Docker App

This is a simple Node.js + Express application that serves an HTML + CSS page. The project is fully containerized with Docker so you can run it anywhere.

🚀 Project Structure
`
my-node-app/
 ├── Dockerfile
 ├── package.json
 ├── server.js
 └── public/
      ├── index.html
      └── style.css
`


server.js → Express server to serve static files

package.json → Node.js dependencies and scripts

public/ → Contains static assets (HTML, CSS)

Dockerfile → Instructions to build the Docker image

⚙️ Running locally (without Docker)

Install dependencies:

`
npm install
`


Start the server:
`
npm start
`

Open in browser:
👉 http://localhost:3000

🐳 Running with Docker
1. Build the image
 `
docker build -t my-node-app .
`

3. Run the container
`
docker run -p 3000:3000 my-node-app           
`

5. Access the app
`
👉 http://localhost:3000
`

📤 Push to Docker Hub (optional)

Tag the image:
`
docker tag nodejs-docker mjdocker3112/nodejs-docker:latest
`

Push to Docker Hub:
`
docker push mjdocker3112/nodejs-docker:latest
`

Pull from any machine:
`
docker pull mjdocker3112/myapp-ex:latest
`



..................




✅ Features

Minimal Node.js + Express setup

Serves static HTML + CSS

Lightweight Docker image (using node:18-alpine)

Ready to deploy anywhere (Docker Hub, cloud, etc.)
