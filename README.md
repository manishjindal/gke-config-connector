https://cloud.google.com/anthos-config-management/docs/tutorials/config-sync-multi-repo


confif-controller
* https://cloud.google.com/anthos-config-management/docs/concepts/config-controller-overview

hosted version of config connector 
    - also includes policy controller, config sync and config connector 


config connector -> Declarativly deploy resource on the cloud

Policy controller -> Policy Controller enables the application and enforcement of programmable policies for your Kubernetes clusters.

Config Sync -> GitOps is considered a universal best practice for organizations managing Kubernetes configuration at scale


Config Sync:

* https://cloud.google.com/anthos-config-management/docs/how-to/unstructured-repo
* https://cloud.google.com/anthos-config-management/docs/concepts/hierarchical-repo


```
kubectl get RootSync --all-namespaces
NAMESPACE                  NAME                RENDERINGCOMMIT                            RENDERINGERRORCOUNT   SOURCECOMMIT                               SOURCEERRORCOUNT   SYNCCOMMIT                                 SYNCERRORCOUNT
config-management-system   sample-repository   94b8d94e126af1a91e09803e81a56d97b8656598                         94b8d94e126af1a91e09803e81a56d97b8656598                      94b8d94e126af1a91e09803e81a56d97b8656598
config-management-system   test-sync           22544dd8b6dc42504842d9e6a3312607e8fba091                         22544dd8b6dc42504842d9e6a3312607e8fba091                      22544dd8b6dc42504842d9e6a3312607e8fba091
```


```
kubectl get RepoSync --all-namespaces
NAMESPACE   NAME        RENDERINGCOMMIT                            RENDERINGERRORCOUNT   SOURCECOMMIT                               SOURCEERRORCOUNT   SYNCCOMMIT                                 SYNCERRORCOUNT
gamestore   repo-sync   94b8d94e126af1a91e09803e81a56d97b8656598
```


