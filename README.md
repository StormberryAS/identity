# Stormberry Cryptographic Identity

Public verifiable root for cryptographic identities, PGP keys and digital signatures belonging to Stormberry AS and its administrators.

## Rotation policy

> [!IMPORTANT]
> The `marcos.asc` key always points to the **currently active identity key** for the present year.

Stormberry enforces an annual cryptographic rotation. At the start of every calendar year a new key is generated and overwrites `marcos.asc`. Simultaneously an immutable, version-controlled copy is stored as `marcosYYYY.asc` (for example, `marcos2026.asc`, `marcos2027.asc`). The primary URL therefore always returns the most up-to-date key, while historical keys remain preserved in the repository for backwards verification.

## Public keys

- [`marcos.asc`](./marcos.asc): the active, current-year public key used for verification and encryption.
- [`marcos2026.asc`](./marcos2026.asc): the immutable snapshot of the 2026 identity key.

## Usage

Import the public key from this repository into your local GnuPG keychain to verify commits or encrypt messages intended for Stormberry:

```bash
curl -s https://raw.githubusercontent.com/StormberryAS/identity/main/marcos.asc | gpg --import
```

## Credits

Maintained by [Stormberry AS](https://stormberry.as). Proudly powered by sovereign AI agents.
