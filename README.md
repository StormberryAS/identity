# Stormberry A.S. | Cryptographic Identity

This repository serves as the public verifiable root for cryptographic identities, PGP keys, and digital signatures belonging to **Stormberry A.S.** and its administrators.

## Cryptographic Rotation Policy
> [!IMPORTANT]
> The `marcos.asc` key always points to the **currently active identity key** for the present year. 
> Stormberry enforces an annual cryptographic rotation sequence. At the start of every calendar year, a new key is generated and overwrites `marcos.asc`. Simultaneously, an immutable, version-controlled copy of the new key is stored as `marcosYYYY.asc` (e.g., `marcos2026.asc`, `marcos2027.asc`). This ensures the primary URL always returns the most up-to-date key, while historical keys are permanently preserved in the repository for backwards verification.

## Public Keys
*   [`marcos.asc`](./marcos.asc): The active, current-year public key used for verification and encryption.
*   [`marcos2026.asc`](./marcos2026.asc): The immutable snapshot of the 2026 identity key.

## Usage
To verify commits or encrypt secured messages intended for Stormberry, you can import this public key into your local GnuPG keychain directly from this repository:

```bash
curl -s https://raw.githubusercontent.com/StormberryAS/identity/main/marcos.asc | gpg --import
```

---
*Maintained securely by [Stormberry A.S.](https://stormberry.as)*
