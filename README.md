# LocalTerra Protocol Integration Tests

Integration tests that calls Contracts using LCD.

# Instructions
Run `yarn install` and then `node index.js` with the desired env vars as described below.

On the 1st run, you must run it with `DEPLOY=all` to upload all the contracts to the chain and generate the code ids for the contracts.

# ENV Variables
**DEPLOY**: name of contract (name of the wasm file without the extension) or `all` to upload all the contracts.

**CONTRACTS**: the folder with the optmized wasm files.

**FACTORY**: factory address, if Factory is already instantiated you can pass its address on this parameter to skip the deployment process.

Example:

`DEPLOY=all CONTRACTS=../contracts/artifacts node index.js`

