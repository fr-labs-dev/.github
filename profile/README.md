<div align="center">

# FR LABS

**Building verifiable infrastructure for autonomous AI systems.**

[![Website](https://img.shields.io/badge/website-fr--labs--dev.github.io-00C2FF?style=flat&logo=github)](https://fr-labs-dev.github.io)
[![AXIOM](https://img.shields.io/badge/product-AXIOM%20Protocol-00C2FF?style=flat)](https://fr-labs-dev.github.io/axiom)
[![Base](https://img.shields.io/badge/deployed-Base%20Sepolia-0052FF?style=flat&logo=ethereum)](https://basescan.org)
[![npm](https://img.shields.io/badge/npm-%40frlabs%2Faxiom--sdk-CB3837?style=flat&logo=npm)](https://npmjs.com/package/@frlabs/axiom-sdk)

---

## What We Build

AXIOM Protocol is a cryptographic provenance layer that generates
immutable, independently verifiable receipts for every AI inference.

**When an AI agent acts, AXIOM proves:**

- Which exact model ran, with weights bound to a hardware identity
- On which input, using pre-execution commitments
- Producing which output, with signed receipt evidence
- In which hardware environment, using TEE attestation
- At which time, with replay-resistant integrity

---

## Repositories

| Repo | Description | Status |
|------|-------------|--------|
| [axiom](https://github.com/fr-labs-dev/axiom) | AXIOM Protocol monorepo | Active |
| [fr-labs.dev.github.io](https://github.com/fr-labs-dev/fr-labs.dev.github.io) | Company + product website | Active |

---

## Quick Start

```bash
npm install @frlabs/axiom-sdk
```

```typescript
import OpenAI from 'openai';
import { AxiomClient, wrapOpenAI } from '@frlabs/axiom-sdk';

const axiom = new AxiomClient({ apiKey: process.env.AXIOM_API_KEY! });
const openai = wrapOpenAI(new OpenAI(), axiom, { modelId: 'your-model-id' });
```

---

## Current Status

| Metric | Value |
|--------|-------|
| Tests passing | 70+ |
| Crypto packages | 8 |
| External crypto deps | 0 |
| Chains supported | Base Sepolia |
| Contract status | Deployed and verifiable |

---

*Building in public from India. Founded 2025.*

**Contact:** frlabs.startup@gmail.com

</div>
