# Components

- [Pods](##Pods)
- [Services](##Services)
- [Controllers - Operators](##Controllers-Operators)

## Pods

Host and manage containers. It is possible to have mulitple containers in a single pod (Sidecar etc). There is 1 ip address per pod.

## Services

Handles access policies for pods based on selectors.

There are 2 selector types:

### equality-based

Filters via `=` `==` `!=` if mulitple values are used **ALL** must be matched

``` c#
kubectl get pods -l environment=production,tier=frontend
```

### set based

Filters to a set of values allowing the use of `in` `notin` `exists`

``` c#
kubectl get pods -l 'environment in (production),tier in (frontend)'
```

## Controllers-Operators

Controllers also known as watch-loops and operators compare state against a spec and execute code.

### Namespace

### ServiceAccounts

### Endpoints