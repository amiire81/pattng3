# PattNG3

This repository contains Sing-box configuration with custom settings applied to dashax configs.

## Settings Applied

- **Fragment (Finalmask)**: 
  ```json
  {
    "tcp": [
      {
        "type": "fragment",
        "settings": {
          "packets": "tlshello",
          "lengths": ["0", "104", "1"],
          "delays": ["0"],
          "maxSplit": "0"
        }
      },
      {
        "type": "fragment",
        "settings": {
          "packets": "1-1",
          "lengths": ["114", "1"],
          "delays": ["1"],
          "maxSplit": "11"
        }
      }
    ]
  }
  ```

- **Fingerprint**: `unsafe`
- **ALPN**: `http/1.1`
- **Cipher Suites**: 
  `TLS_AES_256_GCM_SHA384:TLS_CHACHA20_POLY1305_SHA256:TLS_AES_128_GCM_SHA256:TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384:TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384:TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256:TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256:TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256:TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256:TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA:TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA:TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA256:TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`

## Usage

Import the `config.json` file into any Sing-box compatible client (SagerNet, FoXray, etc.).

## Source

Configs derived from: https://github.com/amiire81/dashax
