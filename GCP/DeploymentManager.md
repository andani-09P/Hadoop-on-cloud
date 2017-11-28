# google-cloud
informations
<h3>deployment Manager</h3>
https://cloud.google.com/deployment-manager/docs/

Deployment Manager is an infrastructure deployment service that automates the creation and management of Google Cloud Platform resources for you.

Write flexible template and configuration files and use them to create deployments that have a variety of Cloud Platform services, 

such as Google Cloud Storage,

Google Compute Engine, 

and Google Cloud SQL,

configured to work together



create a YAML extesion file.

Set your default project ID. Replace [MY_PROJECT] with your own project ID:

```
gcloud config set project [MY_PROJECT]
```


Deploy your configuration

```
gcloud deployment-manager deployments create my-first-deployment --config vm.yaml
```

Deployment Manager creates the manifest and logs any errors or warnings that occurred during deployment, which makes the manifest useful for troubleshooting.

Describe the deployment:

```
gcloud deployment-manager deployments describe my-first-deployment
```
