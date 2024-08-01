<h1>DOME Access Node Directory</h1>

# Introduction

The directory of the Access Node contains the public data of the organizations that are part of the DOME network.

The data is stored in a YAML file that contains the following information:
```yaml
organizations:
  - name: "Organization 1"
    publicKey: "Mg5v8CDaEnJkSJfP1Q6Q6Q=="
    url: "https://organization1.com"
  - name: "Organization 2"
    publicKey: "EsThbaGlaZIPB6xN6Q6Q6Q=="
    url: "https://123.162.194.139:8080"
```

> NOTE: The `publicKey` field is the public key of the organization that is used to verify the signature of the JWT token. This public key is the one generated and used to sign the Blockchain transactions in the DLT-Adapter and the generated Token in the Replication Service.

> NOTE 2: The `url` must be the URL of the organization's Access Node, and it can be an IP address or a domain. 

# How to set new organizations

To add a new organization to the directory, you need to follow the steps below:
1. Fork the repository
2. Edit the `organizations.yaml` file
3. Create a pull request
4. Wait for the pull request to be approved --> This will need to be verified by the onboarding organization.
5. The organization will be added to the directory
