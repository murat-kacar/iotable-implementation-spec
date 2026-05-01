# IoTable Implementation Specification

IoTable is a multi-tenant cafe and restaurant operations platform.

This repository contains the implementation specification for IoTable.

## Repository Purpose

This repository is the canonical source for machine-readable implementation specifications used by LLM coding agents.

The specification precedes code. Code generated for IoTable must follow the specification documents in this repository.

## Format

- Source documents are written in YAML.
- Every YAML specification document must have a matching JSON Schema.
- Specification documents are written as the current final form of the system.
- The repository does not use migration-style, changelog-style, or patch-style specification language.

## Canonical Structure

```text
specs/
  00-meta/
  01-product/
  02-system-architecture/
  03-domain-model/
  04-tenancy/
  05-identity-access/
  06-application-surfaces/
  07-api-contracts/
  08-data-contracts/
  09-realtime-device-contracts/
  10-implementation-plan/
  11-testing-verification/
  12-operations-deployment/
  13-security-compliance/
  14-ui-ux-system/
  15-engineering-rules/
  16-research-decisions/

schemas/
  00-meta/
  01-product/
  02-system-architecture/
  03-domain-model/
  04-tenancy/
  05-identity-access/
  06-application-surfaces/
  07-api-contracts/
  08-data-contracts/
  09-realtime-device-contracts/
  10-implementation-plan/
  11-testing-verification/
  12-operations-deployment/
  13-security-compliance/
  14-ui-ux-system/
  15-engineering-rules/
  16-research-decisions/

tools/
```

## Required Meta Documents

Specification work must start by reading the meta documents under `specs/00-meta/`.

Initial required documents:

- `specs/00-meta/specification-constitution.yaml`
- `specs/00-meta/documentation-index.yaml`

## Validation

Run:

```bash
pnpm install
pnpm validate
```

The validation command checks YAML specification files against their matching JSON Schemas.
