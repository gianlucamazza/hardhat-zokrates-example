# ZK-Hardhat Example

This project demonstrates how to integrate zero-knowledge proofs into a Hardhat-based Ethereum project using ZoKrates, a toolbox for zk-SNARKs on Ethereum.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed [Node.js](https://nodejs.org/) (required for Hardhat).
- You have a basic understanding of how to use Hardhat and smart contracts on the Ethereum network.
- You have installed [ZoKrates](https://zokrates.github.io/gettingstarted.html).

## Installing ZK-Hardhat Example

To install the dependencies, follow these steps:

1. Clone this repository to your local machine.
2. Run `npm install` to install all the necessary dependencies listed in the `package.json` file.

## Using ZK-Hardhat Example

This project uses several npm scripts to compile the ZoKrates code, generate proofs, and interact with the Ethereum network through Hardhat.

Here's what each script does:

- `pre:compile`: Cleans the relevant directories and prepares the environment.
- `compile`: Compiles the `.zok` file containing your program.
- `setup`: Generates a proving key and a verification key.
- `compute`: Computes a witness for a given set of parameters.
- `generate-proof`: Generates a proof with the witness and proving key.
- `verify`: Verifies the proof.
- `export-verifier`: Creates a Solidity contract that can verify proofs on-chain.
- `clean`: Cleans the build environment.
- `test`: Runs through the entire workflow from compilation to verification.

To execute the entire workflow, you can run:

```bash
npm test

```


This will compile the code, perform the setup, compute a witness, generate a proof, and verify it.

## Project Structure

- `contracts/`: Contains the Solidity smart contracts, including the verifier contract.
- `tmp/`: Used by ZoKrates for intermediary files such as proofs, keys, and witnesses.
- `example.zok`: The ZoKrates program file.

## Contributing to ZK-Hardhat Example

To contribute to this project, follow these steps:

1. Fork this repository.
2. Create a branch: `git checkout -b <branch_name>`.
3. Make your changes and commit them: `git commit -m '<commit_message>'`
4. Push to the original branch: `git push origin <project_name>/<location>`
5. Create the pull request.

## Contact

If you want to contact the project maintainer, you can reach out at `<your_email>@example.com`.

## License

This project uses the following license: [MIT](<link_to_license>).
