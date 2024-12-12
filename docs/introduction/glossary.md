# Glossário de Tecnologias Relacionadas ao ESO.

Este Glossário está organizado em ordem alfabética. 

--- 

??? note "Cluster"

- **What is it?**  
    A group of nodes (computers) that execute workloads in Kubernetes, i.e., run containerized applications.

    It's a technique that groups multiple computational resources into a single logical unit. These resources are interconnected and work together to execute tasks, process data, and store information in a way that improves application performance, ensures high availability, reduces costs, and increases scalability, as resources can be shared and distributed efficiently to meet real-time application demands. Each computer is a "node," and there's no limit to the number of nodes that can be interconnected. The structure is : Project (Clusters(Nodes(Pods))).


    The cluster is what provides the main advantage of Kubernetes: the ability to program and execute containers on a set of physical, virtual, on-premise, or cloud machines. Kubernetes containers are not tied to individual machines. In fact, they are abstracted across the entire cluster.

- **What is it for?**  
    The cluster's function is to group multiple machines into a single, efficient system, allowing distributed applications to be executed with higher performance and scalability. In Kubernetes, it facilitates container management, reducing complexity, ensuring high availability, and reducing costs. A Kubernetes cluster typically has a master node that manages pods and the system's execution environment.

- **Useful links:**  
  - [Introduction to Clusters](https://kubernetes.io/docs/concepts/cluster-administration/)
  - [What is a Kubernetes cluster?](https://aws.amazon.com/pt/what-is/kubernetes-cluster/)
  - [Kubernetes Clusters: Everything You Need to Know](https://www.atatus.com/blog/kubernetes-clusters-everything-you-need-to-know/)
---


??? note "Docker"

- **What is it?**  
  Docker is an open platform for developing, shipping, and running applications. It allows you to separate your applications from the infrastructure, facilitating the delivery of software quickly and efficiently, enabling the creation, sharing, and execution of containerized applications and microservices.

- **What is it for?**  
  It enables infrastructure management. This significantly reduces the time between writing code and executing it in production. 
  It simplifies complex processes such as port mapping, file system concerns, and other standard configurations, allowing you to focus on writing code.
  With Docker, you can develop an application and its supporting components using containers. In this context, the container becomes the unit for distributing and testing the application. Once ready, you can deploy the application to the production environment, whether it's local, cloud-based, or hybrid.

- **Useful links:**  
  - [Official documentation](https://docs.docker.com/)


??? note "Go"

- **What is it?**  
  An open-source programming language created by Google, known for its simplicity, performance, clarity, and conciseness.
- **What is it for?**  
  Used in the development of applications, backend systems, and tools, especially in cloud and Kubernetes environments.
  It's a language that offers concurrency mechanisms that facilitate writing programs capable of taking full advantage of multi-core machines and networks, while its innovative type system enables the construction of flexible and modular programs. Go compiles quickly to machine code and, at the same time, offers convenience with garbage collection and the power of runtime reflection. It's a compiled, statically typed language that has the agility of dynamically typed and interpreted languages.
- **Useful links:**  
  - [Official documentation](https://go.dev/doc/)

??? note "Helm"

- **What is it?**  
  A package manager for Kubernetes that facilitates the deployment and management of applications using templates called "charts."
- **What is it for?**  
  Simplifies the configuration, installation, and update of applications in Kubernetes.
- **Useful links:**  
  - [Official documentation](https://helm.sh/docs/)
  - [GitHub project](https://github.com/helm/helm)

??? note "HPA"

- **What is it?**  
  Horizontal Pod Autoscaler (HPA)
- **What is it for?**  
  It's used to control the number of Pods in a Deployment. For example, if CPU usage is too high, the HPA would increase the number of Pods. It's also possible to use the Vertical Pod Autoscaler (VPA), which would increase the amount of resources for each Pod instead of increasing the number of Pods.

??? note "Ingress"

- **What is it?**  
  In a Kubernetes cluster where all requests arrive at the same IP and port, Ingresses are responsible for directing (based on rules you define via the Kubernetes API) these requests to the appropriate Services. It can also be used for other purposes.

- **What is it for?**  
  It provides a single entry point for routing traffic to internal services.
- **Useful links:**  
  - [About Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/)

??? note "Issuer"

- **What is it?**  
  A component in tools like Cert-Manager for issuing certificates.
- **What is it for?**  
  Manages the issuance of automatic TLS certificates for services in Kubernetes. It issues the SSL certificate for Ingresses to encrypt (with HTTPS) incoming and outgoing requests, for example.

- **Useful links:**  
  - [Cert-Manager documentation](https://cert-manager.io/docs/)

??? note "Kind"

- **What is it?**

Kind means "Kubernetes in Docker", so it is a tool for running local Kubernetes clusters using Docker containers as cluster "nodes."

- **What is it for?**

Kind was initially designed for testing Kubernetes itself, but it can also be used for local development or continuous integration (CI). It enables the creation of Kubernetes clusters easily in local environments, facilitating testing and development without requiring complex infrastructure.

- **Useful Links:**

- [Official Website](https://kind.sigs.k8s.io/)


---

??? note "Kubectl"

- **What is it?**

Kubectl is a command-line tool for communicating with the control plane of a Kubernetes cluster, using the Kubernetes API.

- **What is it for?**

It performs operations in Kubernetes, such as creating pods and monitoring the cluster status.

It allows you to interact with the Kubernetes cluster by performing operations like creating, managing, and viewing resources. It searches for a configuration file called `config` in the `$HOME/.kube` directory, which contains information about how to connect to the cluster.

- **Useful Links:**

- [Official Documentation - Kubernetes](https://kubernetes.io/docs/reference/kubectl/)

---

??? note "Kubernetes"

- **What is it?**

A container orchestration open source platform that automates the deployment, scaling, and management of applications.

- **What is it for?**

Ensures high availability, scalability, and monitoring of containerized applications.

- **Useful Links:**

- [Official Documentation](https://kubernetes.io/docs/)

- [Project GitHub](https://github.com/kubernetes/kubernetes)

---

??? note "Nginx"

- **What is it?**

It is an open-source HTTP web server that can also function as a reverse proxy, load balancer, content cache, TCP/UDP proxy server, and email proxy server. It is widely used due to its high performance and ability to handle large volumes of traffic.

- **What is it for?**

Nginx is used to serve web content, manage network traffic, and balance load between servers, as well as act as a reverse proxy and content cache. It can be used to improve the scalability and performance of web applications by efficiently distributing requests across multiple servers.

It has a main process that manages the configuration and several worker processes that handle request processing. The number of worker processes can be adjusted according to the number of processor cores.

- **Useful Links:**

- [Official Documentation](https://nginx.org/en/docs/)

---

??? note "Lint"

- **What is it?**

A static code analysis process for identifying errors, style issues, and non-compliance with best coding practices.

- **What is it for?**

Ensures code quality, consistency, and adherence to predefined standards by identifying syntax errors, formatting issues, and poor development practices before code execution. It contributes to maintaining clean, readable, and efficient code.

- **Useful Links:**

- [Introduction to linting](https://eslint.org/)

---

??? note "Pods"

- **What is it?**

The smallest unit of computation in Kubernetes, which groups one or more containers.

- **What is it for?**

Manages containers that share resources and act as a single entity in a cluster. The structure is : Project (Clusters(Nodes(Pods))).

- **Useful Links:**

- [About Pods](https://kubernetes.io/docs/concepts/workloads/pods/)

---

??? note "Secrets"

- **What is it?**

Sensitive data we want to store, manage, and use with ESO.

---

??? note "Tilt"

- **What is it?**

A tool that helps with local development for Kubernetes, enabling quick visualization and management of changes to applications.

- **What is it for?**

Facilitates the development workflow in Kubernetes by automatically updating the cluster's state based on code changes. It has an interface and automates many tasks that would otherwise need to be done manually.

- **Useful Links:**

- [Official Website](https://tilt.dev/)

- [Documentation](https://docs.tilt.dev/)

---

??? note "yq"

- **What is it?**

A tool we will install to manipulate YAML files in the command line, similar to jq for JSON.

- **What is it for?**

Edits, transforms, and queries YAML files. YAML files are used to configure applications, services, or clusters.

- **Useful Links:**

- [yq GitHub](https://github.com/mikefarah/yq)

---
