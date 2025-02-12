# Custom policy for Kyverno

Custom policy rules 

- allow-actions-with-policys-only-silo-sa
Enables managing `ClusterPolicy` solely for the security management service account.

- deny-attach-by-pod-and-container
Disables attaching to a container (enables running commands).

- mutate-securitycontext-seccomp
Forcibly adds the `seccomp` profile (which protects against various vulnerabilities) to each `RuntimeDefault` deployment/pod.

- restrict-image-registries
Enables image pulls only from `cr.yandex/*`.

We will keep expanding the policy moving forward.
