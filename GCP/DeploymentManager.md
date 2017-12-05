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


<h3>Install Deployment Manager for Linux System</h3>

Before you begin

Make sure that Python 2.7 is installed on your system:

```
python -V
```

2.Download the archive file best suited to your operating system. Most machines will run the 64-bit package. If you'd like to check, run uname -m to verify if you're running a 64-bit system.
```
google-cloud-sdk-182.0.0-linux-x86_64.tar.gz
```

3.Extract the archive to any location on your file system.

4.Set up the Cloud SDK for use. If you're having trouble getting the gcloud command to work, ensure your $PATH is defined appropriately. Run the install script to add Cloud SDK tools to your path, enable command-completion in your bash shell, and/or enable usage reporting:

```
./google-cloud-sdk/install.sh
```

for more refer link:https://cloud.google.com/sdk/docs/quickstart-linux







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
