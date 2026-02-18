# Bunker Genesis Trust Root
**Event:** GENESIS-001
**Date:** 2026-02-18
**Status:** Canonical & Immutable

## 1. Genesis Bundle Information
- **Filename:** `genesis-001.tar.zst`
- **SHA-256 Hash:** `efc78d565f679b0350814e5f3a1b6f0ce52c4a4e18acc6c23ce303167d214c70`
- **Compression:** zstd (Deterministic)

## 2. Public Key (k-sign-1)
This is the root public key used to verify all subsequent artifacts in the Bunker lineage.

```text
-----BEGIN PUBLIC KEY-----
MCowBQYDK2VwAyEAwO891g88YQGAtq44gKOtjLQqC+Yi+hPqhC8A3vKmHKc=
-----END PUBLIC KEY-----
```
*(Note: Replace with actual key content from file)*

## 3. Genesis Manifest
```json
{
  "bundle": {
    "compression": "zstd",
    "filename": "genesis-001.tar.zst",
    "hash_sha256": "efc78d565f679b0350814e5f3a1b6f0ce52c4a4e18acc6c23ce303167d214c70",
    "tar_version": "tar (GNU tar) 1.34",
    "zstd_version": "*** zstd command line interface 64-bits v1.4.8, by Yann Collet ***"
  },
  "event": "GENESIS",
  "invariants": [
    "Imutabilidade do Genesis",
    "Verificabilidade determinística byte-a-byte",
    "Raiz de confiança independente de host único"
  ],
  "key_id": "k-sign-1",
  "protocol_version": "1.0.0",
  "signature": "R+ykNtPmbkrKNM1Ad/h37wTigVJbMMEgZP4S5I0OEaFRSVtYF9dznZotVqhswk2tRvKcVcM4Q2TS5aXMsFOICw==",
  "timestamp_utc": "1970-01-01T00:00:00Z",
  "version": "001"
}
```

## 4. Verification Instructions
To verify the genesis bundle:
1. Download `genesis-001.tar.zst`.
2. Run `sha256sum genesis-001.tar.zst` and compare with the hash above.
3. Verify the manifest signature using the public key provided.

---
*Este documento é a âncora de confiança do Bunker. Não deve ser alterado.*
