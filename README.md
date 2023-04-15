predictab-le/config - Something Something Kubernetes
----------------------------------------------------

This is a configuration monorepo for the Predictab.le system.

This this repository is organized by service.
Each directory under the `services` directory contains the configuration required to deploy said service.

We practice continuous trunk-based deployments and GitOps methodologies.
Everything in `main` is destined for production.

In order to decouple deployments from releases Predictab.le uses Flipt.
Each service has a `features.yaml` containing the flag configuration for that service.
