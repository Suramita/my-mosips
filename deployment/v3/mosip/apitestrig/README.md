# APITESTRIG

## Introduction
ApiTestRig will test the working of APIs of the MOSIP modules.

## Install
* Review `values.yaml` and, Make sure to enable required modules for apitestrig operation.
* Install
```sh
./install.sh
```

## Run apitestrig manually
* Download Kubernetes cluster `kubeconfig` file from `rancher dashboard` to your local.
  ![apitestrig-1.png](../../docs/images/apitestrig-1.png)
* Install `kubectl` package to your local machine.
* Create a job from an existing k8s cronjob to run an apitestrig for a specific module.
  ```
  kubectl --kubeconfig=<k8s-config-file> -n apitestrig create job --from=cronjob/<cronjob-name> <job-name>
  ```
  example: 
  ```
  kubectl --kubeconfig=/home/xxx/Downloads/qa4.config -n apitestrig create job --from=cronjob/cronjob-apitestrig-masterdata cronjob-apitestrig-masterdata
  ```

  
