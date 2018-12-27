# openssl

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-openssl.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-openssl)

Ansible role for openssl

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.openssl`

# Default settings

```
---
openssl_generate_ca: false
openssl_ca_name: Local Certificate Authority

openssl_generate_selfsigned_cert: false
openssl_generate_signed_cert: false
openssl_cert_common_name: "example.com"
openssl_cert_email: "user@example.com"

openssl_cert_name: "self_signed_cert"
openssl_cert_path: "/etc/ssl/"

openssl_cert_template_chain_crt: ""
openssl_cert_template_crt: ""
openssl_cert_template_key: ""

openssl_cert_file: ""
openssl_key_file: ""

openssl_generate_p12: false
openssl_p12_file: "/etc/ssl/example.com.p12"
openssl_p12_pass: "change-me"

openssl_countryname: US
openssl_province: New York
openssl_locality: New York
openssl_organization: Corporation

openssl_cert_alternate_names: []
openssl_cert_ips: []
```

# Development

Please check [development guide](DEVELOPMENT.md) for details about developing and testing this role.
