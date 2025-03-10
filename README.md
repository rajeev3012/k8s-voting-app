# K8s-Voting-App

## Project Summary:  

- **Voting App:** A Python-based web application where users can cast their votes.  
- **Result Page:** A Node.js web application that displays real-time voting results.  
- **Database:** PostgreSQL is used to store the votes persistently.  
- **Message Queue:** Redis acts as a message broker, temporarily storing votes before processing.  
- **Worker Service:** A background process retrieves votes from Redis and updates the PostgreSQL database.  
- **Kubernetes Deployment:**  
  - All components (Voting App, Result App, Redis, Worker, PostgreSQL) are defined in `deployment.yaml` and `services.yaml`.  
  - A single command (`kubectl create -f k8s-voting-app/`) deploys the entire infrastructure.  
  - A single command (`kubectl delete -f k8s-voting-app/`) removes everything for cleanup.  

This setup ensures efficient vote processing, real-time result updates, and easy deployment/management using Kubernetes. 🚀

