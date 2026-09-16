# MaleCNS / FlyWire · Immune Sight

Research visualization: a **downsampled mushroom-body circuit** treats a toy neoantigen vector as an odor. Sparse Kenyon cells either recognize that pattern or they do not. Recognition (“sight”) is the only source term that opens an immune ODE against unitless tumor burden.

This is **not** FlyWire (139,255 neurons) or MaleCNS (166,700 neurons) running in the browser. It is **not** a medical device.

## Run

Open `index.html` in a browser.

1. Start is a cold tumor: antigen cloaked, immune blind, burden high.
2. Click **present antigen**. The current top-k Kenyon cells become the memory template.
3. Sight (code overlap) rises; immune activity `I` follows; burden `T` can fall.
4. **cloak antigen** hides the pattern again.
5. **antigen escape** drifts the neoantigen vector so the old template misses.

Switch atlas between MaleCNS-like 640 KC and FlyWire-like 512 KC (different claw counts and seeds only).

## Loop

```
neoantigen + vitals → PNs → random-claw KCs → APL top-k
                                    ↓
                         template overlap = sight
                                    ↓
                    dI/dt sourced by sight, not by drug
                                    ↓
                         I kills T in a logistic ODE
```

## Citations

- Dorkenwald et al., *Nature* 2024 — FlyWire whole-brain connectome
- HHMI Janelia / Cambridge Connectomics / Google Research — MaleCNS v1.0 (CC BY 4.0)
