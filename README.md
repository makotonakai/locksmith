# locksmith
Open source software that provides AWS temporary credentials with k8s clusters running outside AWS

## Usage

### (Optional) Create your own root CA certificate and private key
- Your new root CA certificate is stored in locksmith/build/secrets/ca_crt.pem
- Your new root CA private key is stored in locksmith/build/secrets/ca_key.pem

```
cd locksmith/build
chmod +x ./create_secret_ca.sh
./create_secret_ca.sh
```
### (Optional) Create your own server certificate and private key
- Your new server certificate is stored in locksmith/build/secrets/server_crt.pem
- Your new server private key is stored in locksmith/build/secrets/server_key.pem

```
cd locksmith/build
chmod +x ./create_secret_server.sh
./create_secret_server.sh
```

### Create a trustanchor on AWS

#### 1. Click "Create a trust anchor"
![trust-anchor](/images/trust-anchor.png)

#### 2. Paste your Root CA key to External certificate bundle
![create-trust-anchor](/images/create-trust-anchor.png)


### Create a special IAM role on AWS


### Create an AWS profile on AWS

### Create a docker image for locksmith

### Add locksmith to your manifest file

### Run your deployment on your k8s cluster
