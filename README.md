# Public Keys

This repository contains my public keys for secure communication and identity verification.

## Purpose

- **Encrypt messages to send me**: Use my public key to encrypt files or messages that only I can decrypt
- **Verify my identity**: Confirm that messages, commits, or files claiming to be from me are authentic

## Available Keys

Check the repository for available public key files (typically `.pub`, `.asc`, or `.pem` files).

## Usage

### Encrypting a Message for Me

If you want to send me something securely:

**Using GPG/PGP:**
```bash
# Import my public key
gpg --import <keyfile.asc>

# Encrypt a file
gpg --encrypt --recipient <my-email> file.txt

# This creates file.txt.gpg which you can safely send to me
```

**Using SSH public key (for file encryption with age or similar tools):**
```bash
# If using age encryption tool
age -r <ssh-public-key> -o encrypted.txt.age message.txt
```

### Verifying My Identity

To verify a signed message or commit from me:

**GPG/PGP signature verification:**
```bash
# Import my public key
gpg --import <keyfile.asc>

# Verify a signed file
gpg --verify file.txt.sig file.txt
```

**Git commit verification:**
```bash
# Import my GPG key first, then
git verify-commit <commit-hash>
```

## Contact

If you need to reach me securely, encrypt your message using one of the public keys in this repository.

## Key Fingerprints

*Add your key fingerprints here for verification*

---

**Note**: Never share private keys. This repository only contains PUBLIC keys, which are safe to distribute.

