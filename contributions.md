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
[https://github.com/risc0/risc0/pull/3412](https://github.com/risc0/risc0/pull/3412)

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