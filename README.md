# argocd-applications

Centralized repository for platform applications, Helm charts, and policies managed by Argo CD.

## Structure
- `istio/`:
  - `versions/`:
    - `1.30.7/charts/`: Packaged Helm charts for Istio Ambient v1.30.7 (base, cni, istiod, ztunnel, waypoint)
    - `1.30.8/charts/`: Packaged Helm charts for Istio Ambient v1.30.8 (base, cni, istiod, ztunnel, waypoint)
  - `policies/`: Ambient authorization, telemetry, and network policies
  - `samples/`: Ambient demo workloads (echo-server, sleep-client, waypoint-gateway)
  - `values/`: Ambient Helm value profiles
- `open-policy-agent/`:
  - `versions/`:
    - `3.23.0/charts/gatekeeper/`: Packaged Helm chart for OPA Gatekeeper v3.23.0
    - `3.23.1/charts/gatekeeper/`: Packaged Helm chart for OPA Gatekeeper v3.23.1
  - `charts/gatekeeper/`: Default Gatekeeper Helm chart (v3.23.1)
  - `policies/`: Rego ConstraintTemplates and Constraints
  - `samples/`: Workloads demonstrating compliance & violation
