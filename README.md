# Iconassets
Icons for TestNet contracts

Acts as a repo for holding icons for contracts not covered by our existing source.

The icon selection process looks like this:

1. If base chain, use SVG icon from the built-in asset (eg Eth, xDai).
2. Try Trust icon asset repo, if found use this.
3. Try iconassets here.

This applies to all chains on the basis that if contracts are the same on different networks they are owned by the same key holder.

There is no chain restriction because there should never (! very unlikely on a cosmic scale) be an address collision between chains unless the contract is created from the same key and same nonce.

The checking address should be in this format:

https://raw.githubusercontent.com/alphawallet/iconassets/master/YOUR_TOKEN_ADDRESS_HERE/logo.png

Note that the address needs to be checksummed eg:

https://raw.githubusercontent.com/alphawallet/iconassets/master/0xe52eCd3d16E7b194ad16a8C338b1805fE3F66644/logo.png
