# NoteBook for openshift v4

## Overview
- Add a topology view for the applications (developer console)
- Add a odo client for the java developers
- Helm 3 is better supported
- Operator is better supported (Ex. CNO - Cluster Network Operator) 

## Docker is removed
- CRI-O was created to provide a lightweight runtime for Kubernetes which adds an abstraction layer between the cluster and the runtime that allows for various OCI runtime technologies
- CRI-O usage transfer : https://github.com/cri-o/cri-o/blob/master/transfer.md
  - Most replaced by : podman
  - runtime exception: crictl exec (docker exec), crictl ps (docker ps)
  - Build is replaced by buildah : buildah bud (docker build)
- Buildah allows you to have a Kubernetes cluster without any Docker daemon for both runtime and builds
- Buildah specializes in **building** OCI images
- Podman allows you to do all of the Docker commands without the daemon dependency
- Podman specializes in **all of the commands** and functions that help you to **maintain and modify** those OCI container images, such as pulling and tagging

## Applications
  later
  
## Nodes
- Add tune management

## Service Mesh
- The service mesh on Openshift is not totally same with Istio
- Kiali is the Istio observability console
  
## Serverless
  later

## Not useful
  - Machine management (Public Cloud)
  - Telemetry (Security)
