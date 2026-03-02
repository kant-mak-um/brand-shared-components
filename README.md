# brand-shared-components

## Purpose
This repository contains **shared, non-proprietary components** used across multiple startup brands (OpCos).

It exists to prevent duplication and keep shared assets **brand-neutral**.

## Authority & Governance
- **Repository Role:** Shared components (UI, utilities, common interfaces)
- **Design Origin:** May reference KMU open designs when non-domain-specific
- **Standards:** Not a standards authority
- **Manufacturing:** Not included
- **Commerce:** Downstream-only (e.g., WaterWolf may consume this repo)

## Scope
Included:
- Common interfaces (non-brand-specific)
- Shared UI components and utilities (if applicable)
- Public configuration standards

Excluded:
- Proprietary manufacturing methods or tooling
- Brand-specific differentiation
- Advanced/licensable designs

## Dependency Declaration (Shared Components)
Allowed dependencies:
- Open-source libraries/frameworks required for shared components (UI, utilities)

Conditionally allowed:
- `kmu-open-*` only when importing **non-domain-specific** interface definitions or reference schemas

Must not depend on:
- `kmu-adv-*`
- `cc-*`
- `mba-*`
- `brand-waterwolf-storefront`
- Any OpCo repo (e.g., `brand-*-products`)

Dependency direction:
- OpCo repos and WaterWolf may depend on `brand-shared-components`
- `brand-shared-components` must not depend on OpCo repos

## License
See `LICENSE`.
