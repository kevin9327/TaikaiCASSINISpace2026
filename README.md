# TAIKAI × EUSPA — `12th CASSINI Hackathon: Space for Peace and Resilience` Submission Package (`€9,000 EUR` Cash Pool)

![Banner](banner.png)

## 1. Competition Overview & Live Cash Verification
- **Hackathon:** 12th CASSINI Hackathon — `"Space for Peace and Resilience"`
- **Organizer:** European Union Agency for the Space Programme (**EUSPA**) / European Commission (**DEFIS**)
- **Official Portal:** `https://taikai.network/en/cassini/hackathons/space-for-peace-and-resilience`
- **Cash Prize Pool:** **`€9,000 EUR` Central European Cash Pool (`€5,000` 1st, `€3,000` 2nd, `€1,000` 3rd)** + Local Hub Prizes across 10 European hubs
- **Timeline:**
  - Registration & Matchmaking Open Now (Deadline: **November 20, 2026 @ 05:00 UTC**)
  - Hackathon & Project Submission: **November 27 – 29, 2026**
  - European Demo Day & Jury Awards: **December 2, 2026**

---

## 2. Unifying All 3 Mandatory EU Space Programme Assets Across All 3 Challenges
`EuroShield-Space` ([`cassini_space_resilience_engine.py`](cassini_space_resilience_engine.py)) integrates **Copernicus**, **Galileo / EGNOS**, and **IRIS²** across all three official CASSINI tracks:

1. **Challenge 1 — Cybersecurity for Space-Based Strategic Enablers (`CASSINI-CH1`):**
   - Implements **Galileo OSNMA (Open Service Navigation Message Authentication)** TESLA one-way key-chain validation (`SHA-256(K_i || salt) == K_{i-1}`) and HMAC navigation tag verification alongside a 5-channel pseudorange innovation residual gate (`|r_i| / \sigma > 5.0`), isolating a `+485.0 m` GNSS spoofing/meaconing attack on `PRN E24`.
2. **Challenge 2 — Space-Enabled Crisis Response & Civil Resilience (`CASSINI-CH2`):**
   - Fuses **Copernicus Sentinel-1 C-Band SAR (`VV <= -16.5 dB` specular water mask)** with **Sentinel-2 (`NDWI >= 0.25`)** to detect flooded bridge corridors through cloud cover and re-routes emergency civil convoys via Dijkstra shortest safe-time pathing (`Depot_Alpha -> Ridge_Pass -> Hospital_Central`, `34.0 min` ETA).
3. **Challenge 3 — Countering Transnational Crime & Maritime Threats (`CASSINI-CH3`):**
   - Runs a **2-Parameter CFAR (`Constant False Alarm Rate`, $\tau = 6.0\sigma$) Ship Detector** over Sentinel-1 maritime SAR swaths, cross-correlates metallic radar targets (`Z = 11.69\sigma`, `11.25\sigma`) against AIS transponder blackouts to flag illicit dark vessels (`SAR-M02`, `SAR-M04`), and dispatches an **IRIS²** SHA-256 authenticated alert payload.

---

## 3. Package Files & Deterministic Verification (`exit code 0`)
- [`cassini_space_resilience_engine.py`](cassini_space_resilience_engine.py) — Full multi-challenge Galileo OSNMA + Copernicus SAR + IRIS² engine (`exit code 0`).
- [`cassini_space_verification_report.json`](cassini_space_verification_report.json) — Machine-verifiable JSON report (`SHA-256: 3d75a7b3daa8411506612ab6715779f2617a835bccfcc19025b3751bcc928b8e`).
- [`index.html`](index.html) — Interactive Orbital SAR & Galileo OSNMA Command Center.
- [`banner.png`](banner.png) — `1200x630` competition banner.

```bash
python TaikaiCASSINISpace2026/cassini_space_resilience_engine.py
```
