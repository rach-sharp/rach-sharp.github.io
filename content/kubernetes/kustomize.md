
Kustomize is official. It's officially more official than Helm, although this seems to me to be 2 competing standards.

I have settled on:

- Helm is the Kubernetes Package Manager
- Helm is also better if you want to create a Generic Thing that is used amongst multiple repos, e.g. codifying 'you know that way that we deploy Flask which is the same everywhere'
- Kustomize is better than writing raw k8s manifests for your infrastructure yamls that sit alongside application code and aren't going to get reused