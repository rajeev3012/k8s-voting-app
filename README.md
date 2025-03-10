# K8s-Voting-App

## Project Summary:  

- **Kubernetes Manifests:** Uses `deployment.yaml` and `services.yaml` to define the voting app components.  
- **Components:** Includes a voting page, result page, PostgreSQL database, Redis, and a worker.  
- **Redis Role:** Acts as a message queue to temporarily store votes.  
- **Worker Role:** Processes votes from Redis and updates the PostgreSQL database.  
- **Easy Deployment:** Runs with a single command – `kubectl create -f k8s-voting-app/`.  
- **Easy Cleanup:** Removes the entire infrastructure with – `kubectl delete -f k8s-voting-app/`.  
- **Efficiency & Scalability:** Ensures smooth processing and real-time result updates. 🚀

