### Test deploying contract

Simple package to deploy sample smart contract into Rinkeby, by using the private key to sign transactions locally.

### Have the public + private keys

You'll need a pair of private + public keys, along with some balance on Rinkeby to make it happen.

Generate one pair (that's unused for anything else) with MetaMask, https://mycrypto.com or similar.

Follow instructions to obtain test ether https://faucet.rinkeby.io/

Have Node.js >8.9 and npm

```
npm install

export WEB3_URL=<authed URL from either infura / alchemy>
export PRIV=<private key here> 
export FROM_ADDRESS=<public key here>


npm run deploy-rinkeby
```

The process run for about 1 minute to deploy all of it. By the end of it you should see logs like:

...
Saving successful migration to network...
  ... 0x3161c9f37f3686fb8ad5292cf4e57bd8feff4f9746ca2304e97aa61e09eaaaaa
Saving artifacts...
