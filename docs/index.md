# Trusted Application Pipeline Software Template

This application, **backend-tests-go-zmedwqtv**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv ](https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv-gitops ](https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |
| **tssc-app-ci** | The namespace used for CI workloads |
| **tssc-app-development** | The default application during development. Every build will be deployed to this namespace for testing. |
| **tssc-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv-gitops ) in the components/backend-tests-go-zmedwqtv/overlays/stage directory |
| **tssc-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-rhdh-qe/backend-tests-go-zmedwqtv-gitops ) in the components/backend-tests-go-zmedwqtv/overlays/prod directory |