# CRE Workflows Tests

This project is demonstrating how CRE TS Javy Plugin works as an npm package.

## REQUIREMENTS:

## Usage

- Bun 1.2.21 installed

Download the CRE TS Javy Plugin like a regular bun dependency:

```bash
bun install
```

Before first usage run the setup command. Setup will download the right Javy binary based on your operating system and will compile a version with the Chainlink CRE Javy Plugin included:

```bash
bunx cre-setup
```

Then you are ready touse the CRE TS Javy Plugin to compile your workflows to WASM. Copy any JS workflow file from `cre-sdk/dist/workflows` and run the following command:

```bash
bunx cre-compile <input.ts> <output.wasm>
```

Example:

```bash
bun cre-compile src/hello-world.ts dist/hello-world.wasm
```
