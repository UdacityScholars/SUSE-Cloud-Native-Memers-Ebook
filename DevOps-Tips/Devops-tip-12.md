# DevOps Tip 12

[Kubectl](https://kubernetes.io/docs/tasks/tools/#kubectl) is a fantastic command line tool to manage  Kubernetes resources. It provides comprehensives functionalities and flexibility to manage your resources. But that also means you need to remember kubectl command (or search Google every time) for managing your resources, which could be quite cumbersome for some developers. Also often data shown in the command line is easier to understand if it's visualized properly, e.g. the pod's CPU and memory usage history.

As a solution for those problems, Kubernetes offers a GUI solution. It's called Kubernetes Dashboard. Dashboard is a web-based Kubernetes user interface. You can do many things through this dashboard including deploy containerized applications to a Kubernetes cluster, troubleshoot your containerized application, and manage the cluster resources. You can use Dashboard to get an overview of applications running on your cluster. Dashboard also provides information on the state of Kubernetes resources in your cluster and on any errors that may have occurred.

Try it for yourselves by following [this](https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/) guide and see whether this tool makes your life easier.

![Devops Tip 12](./img/devops-tip-12.png)