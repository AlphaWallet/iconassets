# Iconassets
Icon repo for AlphaWallet UI improvement.

Acts as a repo for holding icons for contracts not covered by our existing sources, and is implemented on both platforms.

The icon selection look like this:

(process was re-ordered to improve wallet aesthetics)

1. If base chain, use SVG icon from the built-in asset (eg Eth, xDai).
2. Try iconassets here, if found use the graphic asset from this repo.
3. Try Trust icon asset repo, if found use the graphic.
4. If no asset found, render a text icon using the Token Symbol name if appropriate.

This applies to all chains on the basis that if contracts are the same on different networks they are owned by the same key holder.

There is no chain restriction because there should never be an address collision between chains unless the contract is created from the same key and same nonce.

The checking address should be in this format:

https://raw.githubusercontent.com/alphawallet/iconassets/master/YOUR_TOKEN_ADDRESS_HERE/logo.png

Note that the address needs to be lowercased (i.e. not apply EIP55) eg:

https://raw.githubusercontent.com/alphawallet/iconassets/master/0xe52ecd3d16e7b194ad16a8c338b1805fe3f66644/logo.png

# How to add new assets

1. clone the repo ```> git clone https://github.com/AlphaWallet/iconassets.git```
2. add a directory with the name of your address, all lowercased eg: BUSD `0xe9e7cea3dedca5984780bafc599bd69add087d56`, not `0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56`

```
> mkdir 0xe9e7cea3dedca5984780bafc599bd69add087d56
```

3. Copy the logo into this directory as ```logo.png``` which should be in PNG/JPG format, preferrably around 3k -> 9k size; 128 x 128 pixels is found to be ideal.
```
Directory: /dev/iconassets/0xe9e7cea3dedca5984780bafc599bd69add087d56

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         7/06/2021   5:31 PM           3128 logo.png
```

Then commit changes as normal.
