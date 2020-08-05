# Iconassets
Icons for TestNet contracts

Acts as a repo for holding icons for TestNet token contracts. 

Useful for demos etc.

The wallet should pick up contract icons from these chains:

- Rinkeby
- Ropsten
- Sokol
- Kovan
- Goerli

There is no chain restriction because there should never (! very unlikely on a cosmic scale) be an address collision between chains unless the contract is created from the same key and same nonce. Since this only caters for test net contracts the consequences of an icon collision are very minor.

The checking address should be in this format:

https://raw.githubusercontent.com/alphawallet/iconassets/master/YOUR_TOKEN_ADDRESS_HERE/logo.png

Note that the address needs to be checksummed eg:

https://raw.githubusercontent.com/alphawallet/iconassets/master/0xe52eCd3d16E7b194ad16a8C338b1805fE3F66644/logo.png
