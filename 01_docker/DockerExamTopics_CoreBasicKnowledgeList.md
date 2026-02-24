# DOCKER EXAM ROUGH TOPIC LIST - upd. Feb 24, 2026 - Only multiple-choice questions

* What is Docker?
* What is Docker container vs virtual machine?
* What is Docker Engine
* What you can do with Docker? 
* Benefits of containerization/dockerization?
* What is Docker image?
    * What is Docker Hub and how to use it?
    * Docker Hub 'official images', trust/security in general
* Building images
* Dockerfile
    * ENV variables (will go also to running container), ARG variables (only for build-time)
    * a) builder image (npm i, nmp build) and b) the 'deployed image'/'runner image'/'server image' (npm run) concept
    * RUN here would mean running commands inside container while building the image
    * (port _exposing_ is not really doing anything, informative)
    * ENTRYPOINT, CMD
        * Examples of e.g. this can be found by browsing the folders of this repo
        * Detail: if define both, then CMD works as CLI arguments for the ENTRYPOINT
* YAML (just the very basics of YAML language markup/syntax and format rules)
* Running and stopping containers
* Docker CLI commands
    * -it (two flags -i and -t) vs --it (one whole word parameter 'it') 
* EXEC means running commands from outside, executed inside of a running container
* Docker networks (3 most common user-defined types (or 'drivers'): Bridge, Host, None)
    * Again there are some examples in the folders of this repo
    * +1 Docker's Default network e.g. 'Docker0', which is there automatically, and containers would be part of it automatically. It's of type/driver: Bridge
* container's ports  (expose=just informative vs. real **publish**=open)
* Docker volumes (3 most common types: Host, anonymous, named)
* Docker compose (Orchestration of multiple (images->)containers, networks, volumes, ENVs - connecting and/or isolating)
* Docker (or other containerization platform) as part of architecture design/selection
    * micro-service architecture could benefit most? monolithic the least?
* Kubernetes underlayer > OKD/OpenShift toppings > CSC Rahti (installation of OKD)
    * e.g. cluster-node-pod-container
    * etc. yellow highlighted parts of the 15-page document. 
        * Questions only about them (and text immediately around or inside them).
        * Do not read the whole doc / all the lines. Some you can leaf through fast of course.
        * Some text/pages skip totally. E.g. cPouta stuff. 