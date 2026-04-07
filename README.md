# Stormberry A.S. | Cryptographic Identity

This repository serves as the public verifiable root for cryptographic identities, PGP keys, and digital signatures belonging to **Stormberry A.S.** and its administrators.

## Cryptographic Rotation Policy
> [!IMPORTANT]
> The current active key (`marcos.asc`) is strictly valid **only for the year 2026**. 
> Stormberry enforces an annual cryptographic rotation sequence. A newly generated `.asc` root public key will be issued at the start of every calendar year. The previous year's keys will be moved to a permanent archive directory to maintain historical verification availability.

## Active Public Keys
*   [`marcos.asc`](./marcos.asc) *(Valid: 2026)*: The public key used to verify signed git commits, encrypted communications, and software releases authored by Marcos.

## Usage
To verify commits or encrypt secured messages intended for Stormberry, you can import this public key into your local GnuPG keychain directly from this repository:

```bash
curl -s https://raw.githubusercontent.com/StormberryAS/identity/main/marcos.asc | gpg --import
```

---
*Maintained securely by [Stormberry A.S.](https://stormberry.as)*
