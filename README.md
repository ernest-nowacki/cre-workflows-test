# CRE Workflows Tests

This project is demonstrating how CRE TS Javy Plugin works as an npm package.

## Usage

Download the CRE TS Javy Plugin like a regular npm dependency:

```bash
npm install
```

Before first usage run the setup command. Setup will download the right Javy binary based on your operating system and will compile a version with the Chainlink CRE Javy Plugin included:

```bash
npx cre-setup
```

Then you are ready touse the CRE TS Javy Plugin to compile your workflows to WASM. Copy any JS workflow file from `cre-sdk/dist/workflows` and run the following command:

```bash
npx cre-compile-workflow <input.js> <output.wasm>
```

Example:

```bash
npx cre-compile-workflow src/hello-world.js dist/hello-world.wasm
```
