# Tutorial 11
Fikri Risyad Indratno</br>
2206031170</br>
Advanced Programming B</br>

---

> Compare the application logs before and after you exposed it as a Service. Try to open the app several times while the proxy into the Service is running. What do you see in the logs? Does the number of logs increase each time you open the app?

![](images/img1.png)

Yes the number of logs increase each time I open the app. After the I exposed it, the service can receive requests and each request will be recorded and shown in the logs.

> Notice that there are two versions of `kubectl get` invocation during this tutorial section. The first does not have any option, while the latter has `-n` option with value set to `kube-system`. What is the purpose of the `-n` option and why did the output not list the pods/services that you explicitly created?

The purpose of `-n` is to show services in the `kube-system` namespace. Without `-n`, it shows services in the default namespace. The output did not list the pods/services that I explicitly created because I created it in the default namespace.