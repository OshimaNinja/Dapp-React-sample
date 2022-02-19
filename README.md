# Dapp React Sample

A set of useful components for common UI elements.

## Components

We provide components that support the React 16.3+ context API and also the legacy context API. The legacy context components will be deprecated in 2.0 with breaking changes to the `drizzle-react-components` API. We recommend usage of the new context components where possible.

For 1.x.x this is how you import the different components:

### React 16.3+ Context Components

```
import { newContextComponents } from "drizzle-react-components";
const { AccountData, ContractData, ContractForm } = newContextComponents;
```

`LoadingContainer` is not provided with the new context components currently. Also note that you must pass in `drizzle` and `drizzleState` for each of these components.

### Legacy Context Components

```
import {
  AccountData,
  ContractData,
  ContractForm,
  LoadingContainer
} from "drizzle-react-components";
```

Refer to the included [test apps](#test-apps) for usage examples.


### Installation

1. `cd ./test-app`
1. Install dependencies: `npm install`
1. Start your development blockchain: `truffle develop`
1. (In Truffle develop console) Compile contracts: `compile`
1. (In Truffle develop console) Migrate contracts: `migrate`
1. In another terminal window: `cd ./app`
1. Install dependencies: `npm install`
1. Start dev server: `npm start`

NOTE: Make sure to `migrate --reset` your contracts and reset your Metamask account when switching between test apps, otherwise errors may occur.
