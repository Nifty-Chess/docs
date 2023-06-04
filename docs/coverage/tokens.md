---
sidebar_position: 3
sidebar_label: "Tokens & Currencies"
---

# Tokens and Currencies Supported

### All ERC20, ERC721, and ERC115 tokens are supported. 

If your token is on this list, you can use the `CurrencyType` to specify the specific token for transactions. 

Otherwise, select a token using its network and address. 

## Ethereum

 | Name     | `CurrencyType` |    Usage     | Decimals |                  Address                   |
 | :------- | :------------: | :----------: | :------: | :----------------------------------------: |
 | Ethereum | `MAINNET_ETH`  | Network Coin |    18    |                                            |
 | DAI      | `MAINNET_DAI`  |  Stablecoin  |    18    | 0x6B175474E89094C44Da98b954EedeAC495271d0F |
 | USD Coin | `MAINNET_USDC` |  Stablecoin  |    6     | 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48 |

## Polygon

| Name     | `CurrencyType`  |    Usage     | Decimals | Address |
| :------- | :-------------: | :----------: | :------: | :-----: |
| Matic    | `POLYGON_MATIC` | Network Coin |    18    |         |
| DAI      |  `POLYGON_DAI`  |  Stablecoin  |    18    |         |
| USD Coin | `POLYGON_USDC`  |  Stablecoin  |    6     |         |

## Mumbai

| Name          | `CurrencyType` |     Usage     | Decimals |                  Address                   |
| :------------ | :------------: | :-----------: | :------: | :----------------------------------------: |
| Mumbai        | `MUMBAI_MATIC` | Network Coin  |    18    |                                            |
| DAI           |  `MUMBAI_DAI`  |  Stablecoin   |    18    | 0x001B3B4d0F3714Ca98ba10F6042DaEbf0B1B7b6F |
| USD Coin      | `MUMBAI_USDC`  |  Stablecoin   |    6     | 0x2058A9D7613eEE744279e3856Ef0eAda5FCbaA7e |
| Wrapped Ether | `MUMBAI_WETH`  | Wrapped Token |    18    | 0xd8bD0a1cB028a31AA859A21A3758685a95dE4623 |


## Gnosis

| Name         | CurrencyType |    Usage     | Decimals |                  Address                   |
| :----------- | :----------: | :----------: | :------: | :----------------------------------------: |
| Gnosis Token | `GNOSIS_GNO` | Network Coin |    18    | 0x6810e776880C02933D47DB1b9fc05908e5386b96 |
| DAI          | `GNOSIS_DAI` |              |          |                                            |
| USD Coin     | `GNOSIS_USD` |              |          |                                            |

## Goerli

| Name     | `CurrencyType` |    Usage     | Decimals |                  Address                   |
| :------- | :------------: | :----------: | :------: | :----------------------------------------: |
| Ethereum |  `GOERLI_ETH`  | Network Coin |    18    |                                            |
| DAI      |  `GOERLI_DAI`  |  Stablecoin  |    18    | 0xc3dbf84Abb494ce5199D5d4D815b10EC29529ff8 |
| USD Coin | `GOERLI_USDC`  |  Stablecoin  |    6     | 0x07865c6E87B9F70255377e024ace6630C1Eaa37F |

## Optimism

| Name                     |  `CurrencyType`  |     Usage     | Decimals |                  Address                   |
| :----------------------- | :--------------: | :-----------: | :------: | :----------------------------------------: |
| Optimistic Ethereum      | `OPTIMISM_OETH`  | Network Coin  |    18    | 0x4200000000000000000000000000000000000006 |
| DAI | `OPTIMISM_DAI` Stablecoin | 18 | |
| USD Coin | `OPTIMISM_USDC` Stablecoin | 6 | |
| Optimistic Wrapped Ether | `OPTIMISM_OWETH` | Wrapped Token |    18    | 0x4200000000000000000000000000000000000007 |

## Optimism-Goerli

  | Name                     | `CurrencyType`          |     Usage     | Decimals | Address                                    |
  | ------------------------ | :---------------------- | :-----------: | :------: |
  | Optimistic Ethereum      | `OPTIMISM_GOERLI_OETH`  | Network Coin  |    18    |                                            |
  | Optimistic Wrapped Ether | `OPTIMISM_GOERLI_OWETH` | Wrapped Token |    18    | 0x4200000000000000000000000000000000000007 |

## Arbitrum

  | Name          | `CurrencyType`  |     Usage     | Decimals |                  Address                   |
  | :------------ | :-------------: | :-----------: | :------: | :----------------------------------------: |
  | Arbitrum      | `ARBITRUM_ETH`  | Network Coin  |    18    |                                            |
  | DAI           | `ARBITRUM_DAI`  |  Stablecoin   |    18    | 0xF8fF43E991A81e6eC886a3D281A2C6cC19aE70Fc |
  | USD Coin      | `ARBITRUM_USDC` |  Stablecoin   |    6     | 0xff970A61A04b1cA14834A43f5dE4533eBDDB5CC8 |
  | Wrapped Ether | `ARBITRUM_WETH` | Wrapped Token |    18    | 0x82aF49447D8a07e3bd95BD0d56f35241523fBab1 |

## Arbitrum-Nova

| Name          |    `CurrencyType`    |     Usage     | Decimals |                  Address                   |
| :------------ | :------------------: | :-----------: | :------: | :----------------------------------------: |
| Arbitrum Nova | `ARBITRUM_NOVA_ETH`  | Network Coin  |    18    |                                            |
| DAI           | `ARBITRUM_NOVA_DAI`  |  Stablecoin   |    18    | 0xF8fF43E991A81e6eC886a3D281A2C6cC19aE70Fc |
| USD Coin      | `ARBITRUM_NOVA_USDC` |  Stablecoin   |    6     | 0xff970A61A04b1cA14834A43f5dE4533eBDDB5CC8 |
| Wrapped Ether | `ARBITRUM_NOVA_WETH` | Wrapped Token |    18    | 0x82aF49447D8a07e3bd95BD0d56f35241523fBab1 |

## Sepolia

 | Name     | `CurrencyType` |    Usage     | Decimals |                  Address                   |
 | :------- | :------------: | :----------: | :------: | :----------------------------------------: |
 | Sepolia  | `SEPOLIA_SPL`  | Network Coin |    18    | 0x48E9d9A8e2021b35a6112114ad7847687aBbB4f4 |
 | DAI      | `SEPOLIA_DAI`  |  Stablecoin  |    18    | 0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063 |
 | USD Coin | `SEPOLIA_USDC` |  Stablecoin  |    6     | 0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174 |

## Avalanche

| Name          |  `CurrencyType`  |     Usage     | Decimals |                  Address                   |
| :------------ | :--------------: | :-----------: | :------: | :----------------------------------------: |
| Avalanche     | `AVALANCHE_AVAX` | Network Coin  |    18    |                                            |
| DAI           | `AVALANCHE_DAI`  |  Stablecoin   |    18    | 0xbA7dEebBFC5fA1100Fb055a87773e1E99Cd3507a |
| USD Coin      | `AVALANCHE_USDC` |  Stablecoin   |    6     | 0xA7D7079b0FEaD91F3e65f86E8915Cb59c1a4C664 |
| Wrapped Ether | `AVALANCHE_WETH` | Wrapped Token |    18    | 0xB31f66AA3C1e785363F0875A1B74E27b85FD66c7 |

## Avalanche-Fuji

 | Name          |    `CurrencyType`     |     Usage     | Decimals |                  Address                   |
 | :------------ | :-------------------: | :-----------: | :------: | :----------------------------------------: |
 | Avalanche     | `AVALANCHE_FUJI_AVAX` | Network Coin  |    18    |                                            |
 | DAI           | `AVALANCHCE_FUJI_DAI` |  Stablecoin   |    18    |                                            |
 | USD Coin      | `AVALANCHE_FUJI_USDC` |  Stablecoin   |    6     | 0xFa7c34183Cb1d12A99B19C14659b8F2b1401A8f9 |
 | Wrapped Ether | `AVALANCHE_FUJI_WETH` | Wrapped Token |    18    | 0xB31f66AA3C1e785363F0875A1B74E27b85FD66c7 |