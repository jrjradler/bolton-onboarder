# Padawagmi DAO Yeeter

Forked off: https://github.com/HausDAO/bolton-onboarder

This is the launch site to fund our multisig, deployed version here: https://padawagmi.on.fleek.co/


# Development guide

### To update config

 in /package/react-app/App.js
update the config object with what you want

```
const config = {
  network: "mainnet", // set network this will be using mainnet/xdai
  logo: logo, // change the logo here
  projectName: 'YEET',
  mainColor: '#fe1d5b',
  launch: "2021-10-29 16:00 ", // end date of the yeet
  goal: 20, // goal of the yeet
  gnosisSafe: "0xEE5504F0a3604d66470aE3c803A762D425000523", // safe address you want members to send to
  // nativeToken: true,  // not used
  token: "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2", // token yeeting in WETH
  tokenSymbol: "Ξ", // symbol to dsiplay
  website: "https://hackmd.io/@daohaus/H17m16ZwK", // information site
};
```

## Deployment

##### Fleek

* base directory: packages/react-app
* build command: yarn && yarn build
* Publish directory: build

Be sure to select "Create react-app" at inital configuration of the fleek site, will lead to errors otherwise.


# Available Scripts
### React App

#### `yarn react-app:start`

Runs the React app in development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will automatically reload if you make changes to the code.<br>
You will see the build errors and lint warnings in the console.

#### `yarn react-app:build`

Builds the React app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the React documentation on [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

