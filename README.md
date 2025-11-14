Access the latest version of our Prestashop plugin by downloading the zip file available on this page.

For more information, you can consult our documentation : https://docs.axepta.bnpparibas

Available versions:
<table>
  <thead>
   <tr>
      <th>Version</th>
      <th>Size</th>
      <th>SHA56</th>
   </tr>
  </thead>
  <tbody>
    <tr>
      <td>2.0.0</td>
      <td>799.36 KB</td>
      <td>ff80b0dea4629eaeb1dca54f9ad8e3c05aee8f0208dc4d79e8c90ead566fda02</td>
    </tr>
  </tbody>
</table>

## 🔐 Digital Signature

The release is signed with an RSA private key. You can verify the authenticity of the downloaded file using the signature file and public key.

## ✅ Verification Instructions

### Step 1: Download Required Files

```bash
# Download the public key (from our public repository)
curl -LO https://raw.githubusercontent.com/AxeptaBNPParibas/.github/refs/heads/main/axepta-online-github.crt
```

### Step 2: Verify the Signature

```bash
# Verify using OpenSSL
openssl x509 -in axepta-online-github.crt -pubkey -noout > public_key.pem
openssl dgst -sha256 -verify public_key.pem -signature axepta-prestashop-2.0.0.zip.sig axepta-prestashop-2.0.0.zip
```

**Expected output if verification succeeds:** `Verified OK`

---

**⚠️ Security Warning:** Only use this release if signature verification succeeds. A failed verification means the file may have been tampered with.

