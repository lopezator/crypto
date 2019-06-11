# crypto sandbox

Encrypt file using sops and a GPG key.

1. Get your GPG key fingerprint.

$> gpg --list-secret-keys

2. Copy fingerprint.

3. Use sops to edit the encrypted file.

$> sops -pgp `fingerprint-here` pgpfile.yaml

Congrats, you got your encrypted file.