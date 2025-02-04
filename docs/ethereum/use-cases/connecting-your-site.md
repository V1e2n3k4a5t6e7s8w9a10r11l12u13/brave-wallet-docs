---
sidebar_position: 2
---

# Connecting your site

import Connect from '../../../src/components/connect'

Websites can call:

```ts
async function connectSite() {
  return await window.ethereum.request({ method: 'eth_requestAccounts' })
}
console.log(await connectSite())
```

<Connect/>

# More info

To make a request for permissions to an account.
If granted, the website will be able to see the allowed account address.
The website will also be able to ask the user to approve (sing / send) transactions and to sign data.
Signing transactions and messages require separate user confirmations after the initial account approval.

Permissions can be revoked in brave://settings/content/ethereum
A user can also open up the wallet panel and disconnect a connected site when they are on that site.

If a wallet is not yet setup and a page requests permissions, Brave opens brave://wallet for the user to setup the wallet.

# Brave logos

<a href='https://brave.com/static-assets/files/Brave-Logo-Package.zip'>Download Brave logo package</a>
