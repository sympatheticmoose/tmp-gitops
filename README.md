# tmp-gitops

Simple multi-cluster example

Steps
1. kubectx kind-kind
2. gitops install --app-config-url https://github.com/sympatheticmoose/tmp-gitops/
3. gitops add app --app-config-url https://github.com/sympatheticmoose/tmp-gitops/ --url https://github.com/sympatheticmoose/podinfo-deploy
4. kubectx minikube
5. gitops install --app-config-url https://github.com/sympatheticmoose/tmp-gitops/
6. gitops ui run
7. Applications > Add App:  
Name: podinfo-deploy
Namespace: wego-system
Source Repo URL: https://github.com/sympatheticmoose/podinfo-deploy
Config Repo URL: https://github.com/sympatheticmoose/tmp-gitops/
Path: ./
Branch: main
8. Submit
