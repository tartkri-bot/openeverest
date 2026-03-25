# OpenEverest

![!image](logo.png)

[![CNCF Landscape](https://img.shields.io/badge/CNCF%20Landscape-5699C6)](https://landscape.cncf.io/?item=app-definition-and-development--database--openeverest) [![GitHub License](https://img.shields.io/github/license/openeverest/openeverest)](LICENSE) [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/12239/badge)](https://www.bestpractices.dev/projects/12239) [![Documentation](https://img.shields.io/badge/Documentation-white?logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+Cjxzdmcgd2lkdGg9Ijk3LjM2MjgxNm1tIiBoZWlnaHQ9Ijk3LjM2MjgxNm1tIiB2aWV3Qm94PSIwIDAgOTcuMzYyODE2IDk3LjM2MjgxNiIgdmVyc2lvbj0iMS4xIiBpZD0ic3ZnMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZyBpZD0ibGF5ZXIxIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtNTIuMTYwNjE2LC04Ni4zNzg0MzEpIj48cGF0aCBkPSJtIDEwOS4yNDQ2NSwxNTAuMjY3NDggLTcuNjE0NDksLTcuMzkzMzQgNy4yOTM2NCwtNy42Mzg3IGMgMCwwIDEuNDE5MywtMC45OTY2NyAyLjM3NjY0LC0wLjAzOTMgMC45NTc1OCwwLjk1NzU3IC0wLjQyODIzLDMuNTQwMjQgMi4xNTkzOCw1LjAyMTc2IDAsMCAyLjAzMjg4LDEuMDc4OSA1LjEzMzg2LC0yLjAyMjMxIDMuMTAxLC0zLjEwMSAxLjc4MzcyLC00Ljg5NTI4IDEuNzgzNzIsLTQuODk1MjggLTEuNDgxNTIsLTIuNTg3NiAtNC4wNjQxOSwtMS4yMDE4IC01LjAyMTc2LC0yLjE1OTM3IC0wLjk1NzM0LC0wLjk1NzM2IC0wLjAwNCwtMi4zODk0NCAtMC4wMDQsLTIuMzg5NDQgbCA3LjU1MDU5LC03LjE0Njg0IDIxLjQ0MTEsMjEuMzMwNDkgLTcuNDA0MDIsNy40MDQwMSBjIDAsMCAtMC45NTMzLDEuNDMyMDkgMC4wMDQsMi4zODk0NSAwLjk1NzU3LDAuOTU3NTYgMy41NDAyMywtMC40MjgyNSA1LjAyMTc1LDIuMTU5MTQgMCwwIDEuMzE3MjgsMS43OTQ1MSAtMS43ODM3LDQuODk1NDkgLTMuMTAxMDEsMy4xMDEgLTUuMTMzODksMi4wMjIzMiAtNS4xMzM4OSwyLjAyMjMyIC0yLjU4NzYxLC0xLjQ4MTUyIC0xLjIwMTc5LC00LjA2NDE4IC0yLjE1OTM2LC01LjAyMTc1IC0wLjk1NzM2LC0wLjk1NzM2IC0yLjM4OTQ1LC0wLjAwNCAtMi4zODk0NSwtMC4wMDQgbCAtNy40MjU1OCw3LjQyNTU4IC03LjQzNDM1LC03LjQ5NTkgYyAwLDAgLTEuMzY2NywtMC45MzczNSAtMi4zMjA2OSwwLjAxNjggLTAuOTU0MiwwLjk1NDIgMC40NDAzNywzLjU0MTYgLTIuMTQyMDcsNS4wMTQzNiAwLDAgLTIuMDI5MjksMS4wNzE3IC01LjE0MTA2LC0yLjA0MDA4IC0zLjExMTU2LC0zLjExMTc3IC0xLjgwMDU3LC00LjkwMTU2IC0xLjgwMDU3LC00LjkwMTU2IDEuNDcyNzYsLTIuNTgyNDMgNC4wNjAxNCwtMS4xODc4NiA1LjAxNDM0LC0yLjE0MTg1IDAuOTU0MjIsLTAuOTU0MiAtMC4wMDQsLTIuMzg5NjYgLTAuMDA0LC0yLjM4OTY2IHoiIGZpbGw9IiMxMjdiZTgiIGlkPSJwYXRoMS00LTQiIHN0eWxlPSJzdHJva2Utd2lkdGg6MC4yMjQ2NzciLz48cGF0aCBkPSJtIDcyLjQzODQ2NCwxMjkuMDk2NTkgNy43NzU0MDcsLTcuNzc1MyA3LjQ2Mzc3OSw3LjQ2MzY3IGMgMCwwIDEuMDA1NTg2LDEuNDQyNTkgMC4wMzU4OCwyLjQxMjI5IC0wLjk2OTkzMSwwLjk2OTk0IC0zLjU4OTQ0OCwtMC40Mzc0NCAtNS4wODkxNjksMi4xODQ1NCAwLDAgLTEuMDkxNzA5LDIuMDU5ODQgMi4wNTQ4OTIsNS4yMDY2NyAzLjE0NjYwNSwzLjE0NjYgNC45NjQ3MDMsMS44MTI3IDQuOTY0NzAzLDEuODEyNyAyLjYyMTc1MiwtMS40OTk3MyAxLjIxNDYwMiwtNC4xMTkyMyAyLjE4NDMwOSwtNS4wODg5NCAwLjk2OTkzMSwtMC45Njk5MyAyLjQyMjQ3NSwtMC4wMDMgMi40MjI0NzUsLTAuMDAzIGwgNy4zODUxNSw3LjU2MzY0IC0yMS43Mzc5ODgsMjEuODE0OTQgLTcuNTA2NjE4LC03LjUxNTYyIGMgMCwwIC0xLjQ1Mjc2NSwtMC45Njc2OCAtMi40MjI0NzEsMC4wMDMgLTAuOTY5OTMyLDAuOTY5OTMgMC40Mzc0NDgsMy41ODk0NCAtMi4xODQ0OTIsNS4wODg5NCAwLDAgLTEuODE3OTU1LDEuMzMzOTEgLTQuOTY0NjAyLC0xLjgxMjcgLTMuMTQ2NjI4LC0zLjE0NjYgLTIuMDU0ODMzLC01LjIwNjY2IC0yLjA1NDgzMywtNS4yMDY2NiAxLjQ5OTY5OCwtMi42MjE5OSA0LjExOTIzNCwtMS4yMTQ2MiA1LjA4OTAxLC0yLjE4NDMzIDAuOTY5Nzk1LC0wLjk2OTkzIDAuMDAyMSwtMi40MjI0NiAwLjAwMjEsLTIuNDIyNDYgbCAtNy41MzQ4NjQsLTcuNTM0NzggNy41OTI1NDIsLTcuNTMwMDYgYyAwLDAgMC45NDg5NjgsLTEuMzg0NjkgLTAuMDE5MjMsLTIuMzUyODIgLTAuOTY4MjA0LC0wLjk2ODE0IC0zLjU5MDA1MiwwLjQ0MzI5IC01LjA4NTQzNSwtMi4xNzYgMCwwIC0xLjA4ODQyOCwtMi4wNTgyNiAyLjA2MzM5MSwtNS4yMTAwNCAzLjE1MTgxOCwtMy4xNTIgNC45Njc1NjksLTEuODIxMDEgNC45Njc1NjksLTEuODIxMDEgMi42MTk1NTcsMS40OTU0NiAxLjIwNzkxMSw0LjExNzIxIDIuMTc2MDQ1LDUuMDg1MzQgMC45NjgxMzQsMC45NjgzNyAyLjQyMjQ3MSwtMC4wMDMgMi40MjI0NzEsLTAuMDAzIHoiIGZpbGw9IiMwZTVmYjUiIGlkPSJwYXRoMi0zLTQiIHN0eWxlPSJmaWxsOiMwYjRhOGM7ZmlsbC1vcGFjaXR5OjE7c3Ryb2tlLXdpZHRoOjAuMjI0Njc3Ii8+PHBhdGggZD0ibSA4Ny44MDU0OTgsMTI4LjkzNzk2IC03LjU5MjMwMiwtNy42MTU4OSA3LjI3MTQ1OCwtNy40MTYxNyBjIDAsMCAxLjQxOTI4MSwtMC45OTY3MyAyLjM3NjYzNSwtMC4wMzkzIDAuOTU3NTc3LDAuOTU3NDUgLTAuNDI4MjMsMy41NDAxMiAyLjE1OTM3OCw1LjAyMTcyIDAsMCAyLjAzMjg3LDEuMDc4NzcgNS4xMzM4NywtMi4wMjIyNyAzLjEwMTAwMywtMy4xMDEwNCAxLjc4MzcxOCwtNC44OTU0NSAxLjc4MzcxOCwtNC44OTU0NSAtMS40ODE1MjMsLTIuNTg3NTggLTQuMDY0MTg5LC0xLjIwMTc1IC01LjAyMTc2NiwtMi4xNTkyMSAtMC45NTczNTQsLTAuOTU3NDUgLTAuMDAzOSwtMi4zODk1NCAtMC4wMDM5LC0yLjM4OTU0IGwgNy40MzIwOTEsLTcuMzc1ODggMjEuNTU5NTcsMjEuNTU5NiAtNy40MDQwMSw3LjQwNDAzIGMgMCwwIC0wLjcwNTMxLDEuMzI0NDEgMC4yNTIwNSwyLjI4MTk4IDAuMjIwMjIsMC4yMjAxOCAwLjUzNDMxLDAuMjAxODIgMC45MDIxOCwwLjIyNDMgMC4zNDY2OCwwLjAyMTIgMC43MDc1OSwwLjAyOSAxLjEwMjAzLDAuMDc4NiAwLjE0NDk2LDAuMDE4MSAwLjMwMDUyLDAuMDcyNCAwLjQ1MjkyLDAuMDkxNiAwLjkwNjAzLDAuMTE0MDcgMS42ODExLDAuNjA1MzUgMi4zODI3NSwxLjgzMDg3IDAsMCAxLjI1MTE2LDEuODM1ODMgLTEuODQ5ODMsNC45MzY4MyAtMy4xMDEsMy4xMDA5OCAtNS4xMzM4OCwyLjAyMjMxIC01LjEzMzg4LDIuMDIyMzEgLTEuNjMxMDMsLTAuOTMzOTggLTEuODI3MzcsLTIuMjQ1OCAtMS44ODI5OCwtMy4zNzE4NSAtMC4wMTc0LC0wLjM1MDc5IC0wLjA2MzksLTAuNjg0NjUgLTAuMDkxNiwtMC45ODI5NSAtMC4wMjQ0LC0wLjI2MzI4IC0wLjAxODksLTAuNTAxMDQgLTAuMTg0ODIsLTAuNjY2OTYgLTAuOTU3MzUsLTAuOTU3MzQgLTIuMzg5NDUsLTAuMDA0IC0yLjM4OTQ1LC0wLjAwNCBsIC03LjQyNTU3LDcuNDI1NiAtNy40MzQzNiwtNy40OTYxNCBjIDAsMCAtMS4zNjY2OTgsLTAuOTM3MTMgLTIuMzIwNjg3LDAuMDE3MSAtMC45NTQyLDAuOTU0MjEgMC40NDAzNzMsMy41NDE1OSAtMi4xNDIwNyw1LjAxNDM2IDAsMCAtMC43ODM4NDgsMC42NzIxMiAtMi4xMjQyMDksMC4yMzg0NSAtMC40NTIyNTQsLTAuMTQ2MzMgLTEuMDA3NTg0LC0wLjM2OTMgLTEuNTc3ODE3LC0wLjc1NzA5IC0wLjQ1ODk4MywtMC4zMTIxMyAtMS4wMzI3NzcsLTAuODU3MiAtMS41NTc5NzEsLTEuMzgyNDMgLTMuMTExNzc4LC0zLjExMTc4IC0xLjg5OTg1MywtNS4wODAyOSAtMS44OTk4NTMsLTUuMDgwMjkgMC4yOTk1MjYsLTAuNTI1MjkgMC43MjQ2MjksLTEuMDQ0OTEgMS4wOTMyOTQsLTEuMjk0MzQgMC41MzIwMDIsLTAuMzU5OTQgMS4zMzAzNiwtMC41MDc5MyAxLjg4ODY1OSwtMC41NjQyNyAwLjk1NjgxNSwtMC4wOTY2IDEuNTkxOTcxLDAuMDU3NiAyLjA3MTg3NywtMC40MjI0OCAwLjI5MjQ5NiwtMC4yOTI0IDAuNDA1Mjk2LC0wLjUxMDkxIDAuNDIxMDgsLTAuODM4NiAwLjAzNTc1LC0wLjc0MTM0IC0wLjI0NjM3OSwtMS4zNzIxIC0wLjI0NjM3OSwtMS4zNzIxIHoiIGZpbGw9IiNiNmQ5ZmYiIGlkPSJwYXRoMy02LTkiIHN0eWxlPSJzdHJva2Utd2lkdGg6MC4yMjQ2NzciLz48L2c+PC9zdmc+Cg==)](https://openeverest.io/documentation/current/)

[OpenEverest](https://openeverest.io/) is an open source cloud-native database platform that helps developers deploy code faster, scale deployments rapidly, and reduce database administration overhead while regaining control over their data, database configuration, and DBaaS costs.

Why you should try OpenEverest:

- Launch database instance with just a few clicks
- Enable your team to develop faster and reduce time to market
- Scale seamlessly
- Simplify maintenance
- Monitor and optimize
- Automate backups
- Ensure data security

[Discover all the features and capabilities of OpenEverest](https://openeverest.io/) and see how it can transform your database management experience.

## Documentation

For comprehensive information about OpenEverest, see the [documentation](https://openeverest.io/documentation/current/).

## Install OpenEverest Using Helm (Recommended)

Helm is the recommended installation method for OpenEverest as it simplifies deployment and resource management in Kubernetes environments.

### Prerequisites

- Ensure you have a Kubernetes cluster set up (e.g., Amazon EKS, Google GKE).
- Install Helm on your local machine: [Helm Installation Guide](https://helm.sh/docs/intro/install/).

### Steps to Install

1. **Add the Percona Helm repository:**

```bash
helm repo add openeverest https://openeverest.github.io/helm-charts/
helm repo update
```

2. **Install the OpenEverest Helm Chart:**

```bash
helm install everest-core openeverest/openeverest \
--namespace everest-system \
--create-namespace
```

3. **Retrieve Admin Credentials:**

```bash
kubectl get secret everest-accounts -n everest-system -o jsonpath='{.data.users\.yaml}' | base64 --decode | yq '.admin.passwordHash'
```

- Default username: **admin**
- You can set a different default admin password by using the server.initialAdminPassword parameter during installation.

4. **Access the OpenEverest UI:**

   By default, OpenEverest is not exposed via an external IP. Use one of the following options:

- Port Forwarding:

```bash
kubectl port-forward svc/everest 8080:8080 -n everest-system
```

Access the UI at http://127.0.0.1:8080.

For more information about our Helm charts, visit the official [OpenEverest Helm Charts repository](https://github.com/openeverest/helm-charts/tree/main/charts/everest).

## Install OpenEverest using CLI


### Prerequisites

- Ensure you have a Kubernetes cluster set up (e.g., Amazon EKS, Google GKE).

- Verify access to your Kubernetes cluster:

  ```bash
  kubectl get nodes
  ```

- Ensure your `kubeconfig` file is located in the default path `~/.kube/config`. If not, set the path using the following command:

  ```bash
  export KUBECONFIG=~/.kube/config
  ```

## Steps to Install

Starting from version **1.4.0**, `everestctl` uses the Helm chart to install OpenEverest. You can configure chart parameters using:

- `--helm.set` for individual parameters.
- `--helm.values` to provide a values file.

1. **Download the OpenEverest CLI:**

   Linux and WSL

   ```sh
   curl -sSL -o everestctl-linux-amd64 https://github.com/openeverest/openeverest/releases/latest/download/everestctl-linux-amd64
   sudo install -m 555 everestctl-linux-amd64 /usr/local/bin/everestctl
   rm everestctl-linux-amd64
   ```

   macOS (Apple Silicon)

   ```sh
   curl -sSL -o everestctl-darwin-arm64 https://github.com/openeverest/openeverest/releases/latest/download/everestctl-darwin-arm64
   sudo install -m 555 everestctl-darwin-arm64 /usr/local/bin/everestctl
   rm everestctl-darwin-arm64

   ```

   macOS (Intel CPU)

   ```sh
   curl -sSL -o everestctl-darwin-amd64 https://github.com/openeverest/openeverest/releases/latest/download/everestctl-darwin-amd64
   sudo install -m 555 everestctl-darwin-amd64 /usr/local/bin/everestctl
   rm everestctl-darwin-amd64

   ```

2. **Install OpenEverest Using the Wizard:**

   Run the following command and specify the namespaces for OpenEverest to manage:

   ```sh
   everestctl install
   ```

   If you skip adding namespaces, you can add them later:

   ```bash
   everestctl namespaces add <NAMESPACE>
   ```

3. **Install OpenEverest in Headless Mode:**

   Run the following command to set namespaces and database operators during installation:

   ```bash
   everestctl install --namespaces <namespace-name1>,<namespace-name2> --operator.mongodb=true --operator.postgresql=true --operator.mysql=true --skip-wizard
   ```

4. **Access Admin Credentials:**

   Retrieve the generated admin password:

   ```bash
   everestctl accounts initial-admin-password
   ```

5. **Access the OpenEverest UI:**

   Use one of the following methods to access the UI:

- Port Forwarding:

  ```bash
  kubectl port-forward svc/everest 8080:8080 -n everest-system
  ```

  Open the UI at http://127.0.0.1:8080.

- LoadBalancer (Optional):

  ```bash
  kubectl patch svc/everest -n everest-system -p '{"spec": {"type": "LoadBalancer"}}'
  ```

# Need help?

| **Commercial Support** | **Community Support** |
| :---: | :---: |
| Get enterprise-grade support and services for OpenEverest from certified partners. | Connect with our engineers and fellow users for general questions, troubleshooting, and sharing feedback and ideas. |
| **[Get Commercial Support](https://openeverest.io/support/)** | **[Talk to us](https://github.com/openeverest#getting-in-touch)** |

# Contributing

We believe that community is the backbone of OpenEverest. That's why we always welcome and encourage you to actively contribute and help us enhance OpenEverest.

See the [Contribution Guide](CONTRIBUTING.md) for more information on how you can contribute.

## Communication

We value your thoughts and opinions and we would be thrilled to hear from you! [Get in touch with us](https://openeverest.io/#community) to ask questions, share your feedback, and spark creative ideas with our community.

# Submitting Bug Reports

If you find a bug in OpenEverest, [create a GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue#creating-an-issue-from-a-repository) in this repository.

Learn more about submitting bugs, new features ideas and improvements in the [documentation](https://openeverest.io/documentation/current/contribute.html).
