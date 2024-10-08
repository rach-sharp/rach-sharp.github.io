
Kubernetes does not store a `User` object. I find this confusing. They are Right There in the `Binding`s.

### When to engage in Role Play

Levels:
1. If you can access the k8s cluster you are a god. If you cannot then you are nothing. Just guard the door carefully
2. The principle of mid privilege: you want some RBAC but it's not worth establishing the exact permissions that everyone requires and it is not a tragedy for users to personally moderate their usage of the system. `admin`, `edit`, `view`
3. The principle of least privilege: time to hand-craft some artisanal `ClusterRole`s

### RBAC: Much Less Than You "Needed" To Know

1. `Roles` are a set of permissions
2. `Binding` grants them to users
3. `Aggregating` allows Roles to inherit from other Roles
4. 