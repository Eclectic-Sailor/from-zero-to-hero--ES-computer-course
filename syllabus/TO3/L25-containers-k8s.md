# L25: Containers and Kubernetes Primer (EO4)
**Objectives:** Build/run Docker images; understand K8s pods/deployments/services and service discovery/load balancing concepts.

## Resources
- Watch: NetworkChuck Kubernetes intro (~30m): https://www.youtube.com/watch?v=7bA0gTroJjw
- Docker Get Started Part 1: https://docs.docker.com/get-started/
- K8s docs “Pods”: https://kubernetes.io/docs/concepts/workloads/pods/
- K8s “Deployments”: https://kubernetes.io/docs/concepts/workloads/controllers/deployment/
- K8s “Services”: https://kubernetes.io/docs/concepts/services-networking/service/

## Tasks
- Write a Dockerfile for a small API; `docker build` and `docker run -p ...` locally.
- (Optional if tooling available) Run minikube/k3d: apply a Deployment and Service manifest; port-forward to test.
- Sketch how service discovery and load balancing work in K8s.

## Example to Analyze
- Dockerfile best-practice: why prefer a slim base image and separate build/runtime stages?

## Knowledge Check
- Difference between image and container.
- What is a pod vs deployment vs service?
- How does a service find pods?

## Exit Criteria
- Docker image builds and runs locally.
- You can describe the path: client → Service → Pod (and what handles LB).
