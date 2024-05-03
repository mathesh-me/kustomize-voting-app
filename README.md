# Building a simple Voting App using Kustomize and Kubernetes 🚀

This repository contains the **resource Manifests for a simple Voting App** that is built using Kustomize and Kubernetes. This Voting App is a simple web application that allows users to **vote for their favorite pets**. 

## Architecture Overview 🏗️

The Voting App consists of the following components:

- A `Frontend Service` that serves the web application to users to vote for their favorite pets (cats or dogs). It is Developed using **Python Flask**.
- A `Redis Service` that stores the votes.
- A `Worker Service` that processes the votes and stores them in the Postgres database. It is Written in **.NET**.
- A `Postgres Service` that stores the details of the votes such as the pet name and the number of votes.
- A `Result Service` that displays the results of the votes. It is Written in **Node.js**.

## Architecture Diagram 📊

![Voting App Architecture]()

## Prerequisites 📋

Before you begin, ensure you have the following installed on your local machine:

- A **Linux Machine** with `Docker` and `Kubernetes` installed.
- With `Kustomize CLI installed` on your linux machine.

## Usage 🛠️

To deploy the Voting App on your Kubernetes cluster, perform the following steps:

1. Clone this repository to your local machine:
```bash
git clone https://github.com/mathesh-me/kustomize-voting-app
```
2. Change into the directory of the cloned repository:
```bash
cd kustomize-voting-app
```
3. Deploy the Voting App on your Kubernetes cluster using the following command:
```bash
kubectl apply -k voting-app/
```
4. To access the Voting App, Use the below URL:
- **Vote for your favorite pet**: http://node-ip:30111
- **View the results of the votes**: http://node-ip:30112

You can also see my article on [Medium](https://medium.com/@mathesh-me/lets-build-a-voting-app-using-kustomize-and-kubernetes-1cbe07f75c04) for a detailed explanation of the Voting App and how to deploy it using Kustomize and Kubernetes.

## License 📄

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request. If you have better ideas you can create a PR and I will merge it.

## Author 👨‍💻

- [Mathesh M](https://www.linkedin.com/in/mathesh-me/) on LinkedIn.
- You Can also check out my [Medium](https://medium.com/@mathesh-me) for articles on **DevOps Tools and Technologies**.️