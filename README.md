# Proof of When certificate signing key

Proof of When signs its certificates with this OpenPGP key. The private key lives on hardware
keys and is never on a server.

- Master key fingerprint: 5C79 9371 E77B 1D83 360B  7470 AC60 C4C2 FF79 6754
- Signing subkey fingerprint: 8C44 3DCA A5B1 ED3B 1AE8  DCA7 291C 37F8 46F3 6A39
- Identity: ProofOfWhen <admin@proofofwhen.io>
- Created: 2026-10-18 (UTC)
- Public key: proofofwhen-signing-key-public.asc (this repo), https://keys.openpgp.org,
  and https://proofofwhen.io (when live)

To check a certificate, download the certificate text and its signature from the certificate page,
then run:

    gpg --import proofofwhen-signing-key-public.asc
    gpg --verify certificate-XXXX.txt.asc certificate-XXXX.txt

Compare the fingerprint it shows to the one above.

An earlier key (fingerprint 4521 BCFB D10B 159C 7308  B763 E03B D3E5 CEED 5C85) was created on
2026-09-23 but never signed any certificate and is abandoned. Do not trust it.
