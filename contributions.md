# Core Program Brazil 2025: Contributions

## How to add your project (PR template)

Note: Maintain the existing formatting exactly.

- Add a row to the table in "Core Program Brazil 2025 Projects" linking to your section.
- Append your full project section at the end of the file using the template.
- Keep spacing, headings, and list styles unchanged. Do not reformat existing content.

Anchor rule: Use your section heading text in lowercase with spaces replaced by hyphens. Example: `### ZK Multiverse` → `#zk-multiverse`.

Table row template (copy and edit):
```markdown
| [Your Project Name](#your-project-name) 🇧🇷 | Short description of your project. |
```

Project section template (append at file end):
```markdown
---

### Your Project Name

**Contributors:**

- Full Name - [@handle](link)

**Project Description:**
Paragraph describing the project.

**Technical Stack:**

- List your technologies here

**Project Goals:**

- Goal 1
- Goal 2

**GitHub Link:**
[https://github.com/your-org/your-repo](https://github.com/your-org/your-repo)

**Other Links:**
https://your-demo-video-url (optional)
```

## **Core Program Brazil 2025 Projects**

This is a complete list of contributions made by the program participants.

| Project Name                                                                                                     | Project Description |
| :--------------------------------------------------------------------------------------------------------------- | :------------------ |
| [TEMPLATE](#template) 🇧🇷                                                                                          | One-line description of your project. |
| [RISC Zero REVM Integration](#risc-zero-revm-integration) 🇧🇷                                                      | Zero-knowledge EVM bytecode execution using RISC Zero zkVM and revm library. |
| [ZK Air Drop](#zk-air-drop) 🇧🇷                                                                                       | Private airdrop claims using zero-knowledge proofs and Merkle trees. |
| [Farewell](#farewell) 🇧🇷                                                                                       | Farewell is a proof-of-concept dApp that allows people to leave posthumous encrypted messages to their loved ones. |
| [Circom circuit verification in Clean](#circom-circuit-verification-with-clean) 🇧🇷                                | Verification of Circom circuits in Clean |
| [Post-Quantum Smart Account](#post-quantum-smart-account) 🇧🇷                                                      | Smart Account (EIP-4337 Account Abstraction) that uses post-quantum cryptography (PQC) signatures |
| [zkintro Portuguese Translation](#zkintro-portuguese-translation) 🇧🇷                                              | Translation of zkintro's first chapter to Brazilian Portuguese. |
| [FHE VWAP Auction (FHEVM Full-Stack)](#fhe-vwap-auction) 🇧🇷                                    | Privacy-preserving batch auction on EVM using FHE; computes VWAP on-chain. |

---

### [TEMPLATE]

**Contributors:**

- Full Name - [@handle](link)

**Project Description:**
Paragraph describing the project.

**Technical Stack:**

- List your technologies here

**Project Goals:**

- Goal 1
- Goal 2

**GitHub Link:**
[https://github.com/your-org/your-repo](https://github.com/your-org/your-repo)

**Other Links:**
https://your-demo-video-url

---

### RISC Zero REVM Integration

**Contributors:**

- Antonio Viggiano - [@aviggiano](https://github.com/aviggiano)

**Project Description:**
This project demonstrates the integration between RISC Zero zkVM and the revm Ethereum Virtual Machine library, enabling zero-knowledge proof generation for EVM bytecode execution. The implementation showcases how to execute smart contracts privately while maintaining verifiable correctness through zkSNARKs, opening possibilities for private smart contract execution, EVM-compatible rollups, cross-chain verification, and auditing tools.

The main objective of this proof-of-concept is to showcase how a Zero-Knowledge Bug Bounty Program (ZKBBP) can be built. In such a system, a whitehat proves knowledge of a private bytes input $I$ that, when sent to a public function $F$ on public bytecode $B$, produces a public $true$ output. The proof reveals only commitments (hashes of code and calldata), ensuring the exploit input remains secret until disclosure is negotiated. Verifiers (on-chain or off-chain) can check the ZK receipt and be assured the claim is valid without ever learning the exploit itself. 

This minimal implementation provides the scaffold for building more advanced ZKBBPs where: Arbitrary EVM bytecode can be executed under proof, vulnerability classes can be modeled as verifiable predicates, and payout mechanisms can be automated on-chain once proofs are verified.

**Technical Stack:**

- Rust
- RISC Zero zkVM
- revm (Rust EVM implementation)
- Ethereum Virtual Machine
- Zero-Knowledge Proofs (zkSNARKs)

**Project Goals:**

- Demonstrate seamless integration between RISC Zero and revm
- Enable private smart contract execution with proof generation
- Provide foundation for EVM-compatible zero-knowledge applications
- Showcase cross-chain verification capabilities
- Create auditing tools for contract behavior verification

**GitHub Link:**
[https://github.com/risc0/demos/pull/52](https://github.com/risc0/demos/pull/52)

**Other Links:**
N/A

---

### ZK Air Drop

**Contributors:**

- Arthur F. Abeilice - [@afa7789](https://github.com/afa7789)

**Project Description:**
ZK Air Drop enables any eligible user to privately claim tokens from an airdrop using zero-knowledge proofs and Merkle trees. The user’s wallet address is included in the Merkle tree, and a ZK proof is generated off-chain to prove eligibility without revealing the full list or identity. The proof can be used to claim tokens from any wallet, anywhere, ensuring privacy and flexibility for claimants.

**Technical Stack:**

- Solidity
- Circom
- Next.js
- TypeScript
- Ethers.js
- Foundry
- Zero-Knowledge Proofs (Groth16) snarkjs

**Project Goals:**

- Allow private, universal token claims for airdrops
- Enable proof generation for any wallet address in the Merkle tree
- Prevent double-claims and Sybil attacks with ZK verification
- Provide a simple web interface for proof generation and claiming

**GitHub Link:**
[https://github.com/afa7789/zk-token-distributor](https://github.com/afa7789/zk-token-distributor)

**Other Links:**
N/A

---

### Farewell

**Contributors:**

- Pedro G. M. R. Alves - [@pdroalves](https://www.iampedro.com)

**Project Description:**
Farewell is a proof-of-concept dApp that allows people to leave posthumous encrypted messages for their loved ones. Using blockchain smart contracts combined with [fhEVM](https://github.com/zama-ai/fhevm), the system securely stores secret shares of keys and encrypted payloads. A “check-in” mechanism ensures that messages are only released after a period of user inactivity, making Farewell a cryptographic time capsule designed to endure for decades.

**Technical Stack:**

- Solidity
- Hardhat
- fhEVM
- React (frontend)

**Project Goals:**

- Provide a reliable and private mechanism for leaving encrypted messages that will only be released after death or prolonged inactivity.
- Leverage blockchain persistence and cryptography to ensure fairness, security, and decentralization.
- Explore integration of FHE and ZK proofs (e.g., ZKMail) for privacy-preserving proofs of delivery.

**GitHub Link:**
[github.com/pdroalves/farewell-core](https://github.com/pdroalves/farewell-core)

**Other Links:**
[Live demo](https://www.iampedro.com/farewell)

---

### Circom circuit verification with Clean

**Contributors:**

- Christiano Braga - [@christianobraga](https://github.com/ChristianoBraga)
- Semar Augusto Martins - [@semaraugusto](https://github.com/semaraugusto)

**Project Description:**

ZK circuit verification is a major task in software engineering for ZK protocols. Given a verification framework, one needs to:
1. specify the circuit in the framework specification language;
2. state the pre and post-conditions of the circuit (as in [Hoare Logic](https://cs.stanford.edu/people/eroberts/courses/soco/projects/2008-09/tony-hoare/logic.html));
3. prove the circuit's soundness and completeness using the verification framework. Quoting [https://blog.zksecurity.xyz/posts/clean/](https://blog.zksecurity.xyz/posts/clean/):
- Soundness: if the prover can exhibit any witness that satisfies the constraints and lookup relations defined by the circuit, then some specification property holds over that witness. Proving this property ensures that the circuit is not underconstrained.
- Completeness: for every possible input, an honest prover can always exhibit a witness that satisfies the constraints and lookup relations defined by the circuit. Proving this property ensures that the circuit is not overconstrained.

We took a deep dive in Lean 4 and Clean in the 2nd. half of the program and interacted with Clean's team to understand their approach. These interactions lead to jointly concluding the specification and proof (of soundness and completeness) of Circomlib's [`Num2Bits`](https://github.com/Verified-zkEVM/clean/blob/62eb4edde2855c0403df9ad7e8d0c0a391958103/Clean/Circomlib/Bitify.lean#L135). Our team alone [proved](https://github.com/ChristianoBraga/clean/blob/ff2f656a325c974dfcf3ec9df4795584db85a36f/Clean/Circomlib/Comparators.lean#L46) the soundness and completeness of Circom's circuit [`IsZero`](https://github.com/Verified-zkEVM/clean/blob/62eb4edde2855c0403df9ad7e8d0c0a391958103/Clean/Circomlib/Comparators.lean#L14). This lead to [PR 265](https://github.com/Verified-zkEVM/clean/pull/265) at Clean's github.

**Technical Stack:**

- [Lean 4](https://lean-lang.org/)
- [Clean](https://github.com/Verified-zkEVM/clean/) 

**Project Goals:**

1. Prove Circom circuits sound and complete.
2. Learn about theorem proving with Clean.

**GitHub Link:**

[https://github.com/ChristianoBraga/clean](https://github.com/ChristianoBraga/clean)

**Other Links:**

None

---

### Post-Quantum Smart Account

**Contributors:**

- Flavio de Freitas Gouvea Neto - [@freitasgouvea](https://github.com/freitasgouvea)

**Project Description:**

This project implements a Smart Account (EIP-4337 Account Abstraction) that uses post-quantum cryptography (PQC) signatures for transaction authorization. Instead of verifying heavy PQC signatures directly on-chain, the verification is performed off-chain and proven through a zero-knowledge proof (ZK). The smart contract only validates the proof, ensuring that the account owner has authorized the UserOperation. This approach combines quantum resistance, efficiency, and compatibility with Ethereum infrastructure.

**Technical Stack:**

- Go (PQC key generation and signature)
- Dilithium (NIST PQC standard)
- Zero-Knowledge proof framework (TBD)
- Solidity (Smart Account contract implementation)
- Ethereum (EIP-4337 Account Abstraction)

**Project Goals:**

- Implement PQC-based signature generation in Go for UserOperations.
- Develop a ZK circuit to prove PQC signature validity without revealing computation.
- Adapt a Smart Account contract to integrate the ZK verifier.
- Demonstrate an end-to-end flow: UserOperation → PQC Signature → ZK Proof → On-chain Verification → Transaction Execution.

**GitHub Links:**

[PQ Signer](https://github.com/freitasgouvea/pq-signer-go)

---

### zkintro Portuguese Translation

**Contributors:**

- Thiago Rocha - [@thiagorochatr](https://thiagorochatr.com)

**Project Description:**
Translated the first chapter of `zkintro` into Brazilian Portuguese, preserving the original structure and formatting to improve accessibility for Portuguese-speaking readers.

**Technical Stack:**

- Markdown
- Git
- GitHub

**Project Goals:**

- Provide a high-quality PT-BR translation for zkintro's first chapter
- Maintain parity with the original and update as upstream evolves

**GitHub Link:**
[https://github.com/zkintro/zkintro/pull/4](https://github.com/zkintro/zkintro/pull/4)

**Other Links:**
https://zkintro.com/

---

### FHE VWAP Auction

**Contributors:**

- Thiago Rocha - [@thiagorochatr](https://thiagorochatr.com)

**Project Description:**
Privacy-preserving batch auction using Fully Homomorphic Encryption (FHE) on EVM. Sellers escrow Base tokens; buyers submit bids with encrypted prices. The VWAP (Volume-Weighted Average Price) is computed homomorphically on-chain and revealed via the FHEVM decryption oracle. Settlement occurs at the final public VWAP.

**Technical Stack:**

- Solidity
- Hardhat
- FHEVM 0.8.x
- @zama-fhe/relayer-sdk (frontend)
- Next.js
- Tailwind CSS
- TypeScript
- Node.js (>= 20)
- MetaMask (EIP-6963)

**Project Goals:**

- Implement an FHE-based VWAP batch auction on EVM
- Perform on-chain encrypted aggregation with single oracle decryption
- Provide a full-stack monorepo and generated ABIs for the frontend
- Support localhost and Sepolia deployments with tests and coverage
- Ship a usable dApp with MetaMask integration and network helpers

**GitHub Link:**
[https://github.com/thiagorochatr/FHEVWAP](https://github.com/thiagorochatr/FHEVWAP)

**Other Links:**
N/A
