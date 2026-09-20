# KRB encrypted bus

Public transport surface for Kartushin Remote Bridge.

Only encrypted KRB1/KRB1R envelopes belong in the command-bus issue. Never post plaintext commands, credentials, file contents, or business data.

Authorization: the hub accepts command comments only when GitHub reports the exact allowlisted author speccasper.

Cryptography: RSA-OAEP-SHA256 protects a random AES-256-GCM command key. Each encrypted command carries a random reply key used for AES-256-GCM result encryption.

The public encryption key is hub-public.pem.
