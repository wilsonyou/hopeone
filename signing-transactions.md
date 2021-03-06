# Signing Transactions
Sign the pending transaction (the byte array obtained by the inverse hexadecimal encoding of the transaction_blob) with the ED25519 algorithm and the private key, and perform hexadecimal conversion to get sign_data, the signature string.

The following example shows how to sign the  transaction_blob with ED25519 and the private key.

The private key:

'''
b00115764cd017e0da753271fa26cd529451a21b8253d001f0d43612e19ec632570a74ab166b
'''

The transaction_blob:

_0A24627551566B5555424B70444B526D48595777314D553855376E676F5165686E6F31363569109F0818C0843D20E80732146275696C642073696D706C65206163636F756E743A5F08011224627551566B5555424B70444B526D48595777314D553855376E676F5165686E6F3136356922350A246275516E6936794752574D4D454376585850673854334B35615A557551456351523670691A0608011A02080128C7A3889BAB20_

After signing the transaction_blob with the signature interface of ED25519 and performing hexadecimal conversion, the resulting sign_data is:

_a46ee590a84abdeb8cc38ade1ae8e8a2c71bb69bdc4cd7dc0de1b74b37e2cbd1696229687f80dff4276b1a3dd3f95a9bc1d569943b337fe170317430f36d6401_
