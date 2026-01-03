# Drug–Target Interaction Maps and Metabolism Sites
## PHA 548 • Sedative–Hypnotics

This document provides:
1) Drug → target → binding site → functional consequence  
2) Key metabolism routes and “sites of metabolism” (structural liabilities)

*Note: “Sites of metabolism” are presented as high‑yield medicinal chemistry liabilities (not exhaustive atom‑by‑atom biotransformations).*

---

## A. Drug–Target Maps (Mechanism + Binding Site)

### A1. GABA_A Modulators (Benzodiazepines and Z‑drugs)

- **Target:** GABA_A receptor (pentameric ligand‑gated Cl⁻ channel)  
- **Binding site:** Benzodiazepine site at **α–γ interface** (allosteric)  
- **Functional effect:** ↑ *frequency* of GABA‑induced channel opening (requires GABA)

**Mermaid interaction map**

```mermaid
flowchart LR
  BZD[Benzodiazepines] -->|bind allosteric| BZDSite[α–γ interface (BZD site)]
  Z[Z-drugs] -->|bind allosteric| BZDSite
  BZDSite -->|PAM| GABAA[GABA_A Cl⁻ channel]
  GABAA -->|↑ frequency| Inhib[↑ neuronal inhibition]
  Inhib --> Clinical[Anxiolysis • Sedation • Hypnosis (dose & PK dependent)]



