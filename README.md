# Formal analysis of PACE and OTR key exchange

ETH Zürich *Formal Methods for Information Security* course project by **Adam Mernissi Arifi** and **Mehdi Ziazi** (Spring 2024).

We modeled successive refinements of Password-Authenticated Connection Establishment (PACE) and the Off-the-Record (OTR) authenticated key exchange in **Tamarin**. The models examine secrecy, forward secrecy, and authentication. Several intermediate versions intentionally expose attacks; the accompanying [report](report.pdf) explains the protocol changes and attack traces.

## Contents

- [`pace/`](pace/) — challenge-response through PACE, including a Diffie-Hellman key exchange and an attack on an untagged variant.
- [`otr/`](otr/) — the original OTR key exchange, an authentication attack, a proposed improvement, and a SIGMA-style exchange.
- [`report.pdf`](report.pdf) — our 26-page analysis, protocol descriptions, and attack diagrams.

Each protocol directory contains Tamarin theory files and the corresponding saved `-proof.spthy` files. The submitted models and proofs were prepared with **Tamarin 1.8.0**. Open a `.spthy` file in Tamarin to explore its lemmas and traces.
