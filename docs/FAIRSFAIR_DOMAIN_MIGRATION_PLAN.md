# FairsFair Domain Migration Plan

## Current State

Current deployment:
- befairsfair.com points directly to FairsFair Money.

## Target State

### Root Domain
- https://befairsfair.com

Acts as:
- ecosystem HQ
- trust layer
- marketing layer
- navigation hub

### Product Subdomains
- https://money.befairsfair.com
- https://petcare.befairsfair.com

## Recommended Migration Sequence

### Phase 1 — Prepare HQ Site
Create:
- fairsfair-hq repository
- separate Cloudflare Pages project
- lightweight ecosystem landing site

### Phase 2 — Move Money App
Move FairsFair Money to:
- money.befairsfair.com

### Phase 3 — Prepare Petcare
Create:
- fairsfair-petcare
- independent deployment
- independent repo

## Important Architectural Principle

Each vertical should remain independently deployable.
