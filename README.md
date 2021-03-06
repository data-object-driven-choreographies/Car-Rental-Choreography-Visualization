# Blockchain Choreography Frontend

## Screencast

A screencast of the running project can be downloaded [here](https://github.com/data-driven-choreographies/Car-Rental-Choreography-Visualization/blob/master/screencast/Screencast.mp4).

## Installation

### Ganache

```bash
sudo npm install ganache-cli -g
```

### Truffle

```bash
sudo npm install -g truffle
```


### Build Project


Init truffle project in new folder (`truffleproject/`):

```bash
truffle init
```
Add contract to `contracts/` folder and migration (2_deploy_contracts.js) to `migrations/` folder. An example for a complete truffle project can be found [here](https://github.com/data-driven-choreographies/Smart-Contracts).

Compile contract:

```bash
sudo truffle compile
```

Start local blockchain in a new terminal:

```bash
ganache-cli
```

Adapt configuration in `truffle-config.js` according to output of ganache-cli. Set the used port as shown in ganache-clis output.

Migrate contract:

```bash
sudo truffle migrate
```

Create symlink for the smart contracts:

```bash
ln -s ./truffleproject/build/contracts ./Car-Rental-Choreography-Visualization/src/contracts
```


## Execution

Start a local blockchain with:

```bash
npm start
```
