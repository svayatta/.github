# Svayatta Forge

**स्वायत्त** (*svāyatta*): Sanskrit for self-governed, autonomous; one who depends on no other.

Svayatta Forge builds sovereign AI tools: software you run yourself, inspect in full,
and verify without trusting anyone else's servers. The source of every tool is public.
Most are under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0);
where a tool has a different licence, its row below says so. All are built by
Charioteer Consulting Ltd.

**Website:** [svayattaforge.com](https://svayattaforge.com)

## What sovereign means here

- **You run it.** Self-hosted by default. Hosted options are conveniences, never requirements.
- **You can read it.** The full source is here. Most tools are Apache 2.0, which lets you
  use, modify, and ship them commercially.
- **You can check it.** Where a tool makes a claim, it comes with a way to verify it
  that does not depend on us.

## Tools

| Tool | What it does | Status |
|---|---|---|
| [agent-custody](https://github.com/svayatta/agent-custody) | Proof of what your AI agents did: a gateway that checks every tool call against a signed grant and a Cedar policy, issues a signed receipt either way, and logs it in a tamper-evident Merkle log anyone can verify. Website: [agent-custody.dev](https://agent-custody.dev). | Released on npm and PyPI, with a hosted log |
| [loom](https://github.com/svayatta/loom) | Runs large Mixture-of-Experts models across groups of ordinary machines, sharing verified GGUF weight ranges over gossip. One static Zig binary with an OpenAI-compatible API. | Distributed weight sharing works across real machines; untrusted peers is a design only |
| tells | Scores whether the other party on a phone, Meet, or Zoom call is an AI, from turn-taking and synthetic-voice evidence. | Early MVP, score not yet calibrated; source opening soon |
| indic-voice-clone | Clone your voice, accent included. Works well on Indic languages: a short sample gives an instant clone in a local web studio, and longer recordings LoRA-fine-tune the open Svara-TTS model, which covers 19 Indic languages. Runs on a 16 GB Apple-silicon laptop. Licence: PolyForm Noncommercial 1.0.0, free for personal, research and educational use; commercial use by separate licence. | Works end to end, tested in depth on northern Kannada; source opening soon |
| [inai](https://github.com/svayatta/inai) | Coordination middleware for AI agents across frameworks: DID identity without wallets, discovery by capability over a libp2p mesh, DIDComm encryption, optional x402 and MPP payments. Adapters for LangGraph, Google ADK, CrewAI, OpenAI Agents and others, plus an MCP bridge in both directions. TypeScript, Python, Rust and Zig. இணை (inai) is Tamil for "join". | Work in progress; last release 0.3.1 (March 2026), CLI on npm |

## Contact

Charioteer Consulting Ltd · partha@charioteerconsulting.com
