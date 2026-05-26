# GitOps Environment Config
This repository stores environment-specific values for all applications managed by the Hub.

## Role in GitOps (The "Where")
This repo is the source of truth for the state of specific environments (Prod, Staging, Dev).

## Structure
- `values/laura-app/prod.yaml`: Production overrides for Laura App.
- `values/laura-app/stg.yaml`: Staging overrides for Laura App.
- `values/printolito/prod.yaml`: Production overrides for Printolito (WordPress).

## Isolation
Access is controlled via GitHub CODEOWNERS to ensure tenant applications (like `laura-app`) cannot modify other tenants' (like `printolito`) configs.
