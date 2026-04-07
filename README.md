# Stormberry A.S. | Cryptographic Identity

This repository serves as the public verifiable root for cryptographic identities, PGP keys, and digital signatures belonging to **Stormberry A.S.** and its administrators.

## Public Keys
*   [`marcos.asc`](./marcos.asc): The public key used to verify signed git commits, encrypted communications, and software releases authored by Marcos.

## Usage
To verify commits or encrypt secured messages intended for Stormberry, you can import this public key into your local GnuPG keychain directly from this repository:

```bash
curl -s https://raw.githubusercontent.com/StormberryAS/identity/main/marcos.asc | gpg --import
```

---
*Maintained securely by [Stormberry A.S.](https://stormberry.as)*
