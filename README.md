# Liam Gamache · D1srupt3d

This repo serves a single static page at [pub.d1srupt3d.dev](https://pub.d1srupt3d.dev) publishing my PGP public key.

## Verify

```
87AE 6904 63DE 69CF D129  6961 086E 2A2C F6CD 0CD5
```

## Import

```bash
curl -s https://pub.d1srupt3d.dev/key.asc | gpg --import
```

## Use

```bash
# Encrypt a message to me
gpg --encrypt --armor --recipient liam@gamache.dev message.txt

# Verify a signature from me
gpg --verify file.sig file
```

## Contact

<liam@gamache.dev>

---

Only public keys live here.
