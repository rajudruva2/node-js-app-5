# product-service — Node.js / Express
Run locally: `npm install && npm start`
Health check: `curl http://localhost:3000/health`
API: `curl http://localhost:3000/api/products`
Build/run: `docker build -t product-service:1.0.0 .` then `docker run --rm -p 3000:3000 product-service:1.0.0`
For Kubernetes, replace `YOUR_DOCKERHUB_USERNAME` in `k8s/deployment.yaml`, push the image, then run `kubectl apply -f k8s/deployment.yaml`.
