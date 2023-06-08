---
sidebar_position: 1
sidebar_label: "@usekeyp/js-sdk"
---

# `@usekeyp/js-sdk`

Keyp's SDK provides a simple interface for interacting with Keyp's API.

Currently, the SDK supports the following:
- Plugin for logging into Keyp and persisting session data with NextAuth.js
- Helper function for signing in using Keyp and NextAuth.js
- Helper function for ERC20 and ERC721 token transfers
- Helper functions for reading and writing to smart contracts
- Axios client for easily making requests to Keyp's API

## Usage 📖

1.  Add package to your project:  
    `yarn add @usekeyp/js-sdk`

2. Choose from a variety of SDK plugins and helpers:

Easy Keyp logins with NextAuth.js

```js
// pages/api/auth/[...nextauth].js
import { KeypAuth } from "@usekeyp/js-sdk";
import NextAuth from "next-auth";

const NextAuthOptions = KeypAuth({
    clientId: process.env.KEYP_CLIENT_ID, // From dev portal
    secret: process.env.KEYP_COOKIE_SECRET, // Random string
    redirectUrl: "http://localhost:3000/api/auth/callback/keyp",
});

export default NextAuth(NextAuthOptions);
```

Easy user sign in using Keyp and NextAuth.js

```js
import { signInKeyp } from "@usekeyp/js-sdk"

export default function SignInPage() {
    return (
        <div>
        <button onClick={() => signInKeyp("GOOGLE")}>Sign in with Google</button>
        <button onClick={() => signInKeyp("DISCORD")}>Sign in with Discord</button>
        </div>
    )
}
```

Easy token transfers

```js
const ACCESS_TOKEN = session.user.accessToken

const data = {
    accessToken: ACCESS_TOKEN,
    toUserUsername: "pi0neerpat#1337",
    toUserProviderType: "DISCORD",
    tokenAddress: '0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063',
    tokenType: 'ERC20',
    amount: '.01',
}

const res = await tokenTransfer(data)
```

Easy smart contract interactions

```js
import { readContract, writeContract } from "@usekeyp/js-sdk";
import { useSession } from "next-auth/react";
const { data: session } = useSession();

// Read from a smart contract
const result = await readContract(
    {
        accessToken: session?.user.accessToken,
        address: "0x2791bca1f2de4661ed88a30c99a7a9449aa84174",
        abi: "balanceOf(address) public view returns (uint256)",
        args: ['0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063'],
    });

// Write to a smart contract
const result = await writeContract(
    {
        accessToken: session?.user.accessToken,
        address: "0x55d4dfb578daa4d60380995fff7a706471d7c719",
        abi: "pay(uint256,uint256,address) public returns (bool success)",
        args: ['1', '10000000', '0x9ca6a77c8b38159fd2da9bd25bc3e259c33f5e39'],
    });
```

Easy API requests with keypClient, a helper for your axios requests

```js
 useEffect(() => {
    const ACCESS_TOKEN = session?.user.accessToken;
    const userId = session?.user.id;

    const options = {
        headers: {
            Authorization: `Bearer ${ACCESS_TOKEN}`,
        },
    };

    const firstRequest = `/users/${userId}/balance`;
    const secondRequest = `/users/${userId}/balance/${supportedAssets.DAI}`;

    axios
        .all([
            keypClient.get(firstRequest, options),
            keypClient.get(secondRequest, options),
        ])
        .then(
            axios.spread((firstResponse, secondResponse) => {
                let DAI = Object.values(secondResponse.data);
                setAssets({ ...firstResponse.data, DAI: DAI[0] });
                setIsLoading(false);
            })
        )
        .catch((error) => console.error(error));
}, []);
```


## Resources 🧑‍💻

- [SDK Repository](https://github.com/UseKeyp/usekeyp-js-sdk)
- [NextAuth.js](https://next-auth.js.org/)

More functionality coming soon!
