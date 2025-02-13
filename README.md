# secure-bin-signer-action
github action for signing binaries

This GitHub Action signs binaries for multiple platforms:
- Code signs macOS binaries using Apple certificates
- GPG signs binaries for all platforms


```yaml
uses: your-org/sign-binaries-action@v1
with:
  target: 'aarch64-apple-darwin'
  binary-path: './dist'
  binary-name: 'my-binary'
  op-service-account-token: ${{ secrets.OP_SERVICE_ACCOUNT_TOKEN }}
  version: '1.0.0'
```