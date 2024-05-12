<details>

<summary>Modul 11 </summary>

Reflection on minicube

Answer the following questions to guide your reflection:

1. Compare the application logs before and after you exposed it as a Service.

Before exposing your application as a service in Kubernetes, the application is running in a pod, but it's not accessible from outside the Kubernetes cluster. The logs of the application at this stage would typically show the internal workings of the application, such as startup logs, internal processes, and any interactions it might have with other services within the cluster.

When you expose your application as a service, you're making it accessible from outside the Kubernetes cluster. This could be from other services within the cluster, from other pods, or from the internet, depending on how you've configured the service.

After exposing the application as a service, if the application logs incoming requests, We should start seeing these in the logs. Each time a request is made to the application, a new log entry should be created. This means that the more I access the application, the more log entries you'll see.

In summary, before exposing the application as a service, the logs primarily show internal application processes. After exposing it as a service, the logs also start showing incoming network requests.

2. Notice that there are two versions of `kubectl get` invocation during this tutorial section.
13
The first does not have any option, while the latter has `-n` option with value set to
`kube-system`.
What is the purpose of the `-n` option and why did the output not list the pods/services that you
explicitly created?




</details>