# Siddharth S

**Electrical & Electronics Engineering student, SSN College of Engineering, Chennai.** Working on model efficiency for constrained hardware — compression, quantisation, and deployment.

The degree is in power systems; the work isn't. Most of what's below came out of chasing a bug or a bad number until the actual cause showed up, then writing that down instead of the result that looked better.

- **Currently:** Looking for a research or applied ML internship, Jan–Jul 2027, in efficient deep learning / edge ML.
- **Reach me:** [siddharth2310241@ssn.edu.in](mailto:siddharth2310241@ssn.edu.in) · [ORCID](https://orcid.org/0009-0009-2692-0917)

---

## Research

**Battery degradation forecasting.** Benchmarked eight model families — decision trees, MLPs, LSTMs, Transformers, and physics-informed neural networks — for predicting capacity and impedance fade on the NASA PCoE Li-ion dataset. Rollout MAPE for the Transformer sat at 111% until a diagnostic pass found early stopping firing mid-schedule, while the model was still effectively teacher-forced; enforcing a minimum training budget dropped it to 6.23%, ahead of the LSTM baseline. A curriculum-trained PINN with GradNorm loss balancing recovered an activation energy in line with published LCO chemistry, and cross-dataset transfer to a second cell chemistry showed the failure mode was scale mismatch, not chemistry, once corrected for. *Under review, Journal of Energy Storage.*

**Neural image compression.** Built a low-rank factorised SIREN codec with a learned entropy model shared directly with the range coder, so estimated and realised bitrates agree. Swept quantisation step — rather than the loss weight — as the rate-control axis across 384 independently trained models on Kodak, giving valid BD-rate comparisons: −60.4% at rank 16 against a matched full-rank baseline, for a 73% parameter reduction. Done as a research internship at NIT Calicut. *Under review, IEEE Signal Processing Letters.*

**Smart irrigation.** IoT rainfall-prediction system that suppresses watering ahead of forecast rain — Arduino sensor node, ML prediction model, Go backend with MongoDB for telemetry. *Accepted, ICCCT 2026.*

## Experience

| Role | Where | What |
| --- | --- | --- |
| Research Intern | NIT Calicut, 2026 | Independent research on learned image compression, above. |
| Tech & Product Intern | Zocket Technologies, 2025 | Shipped RESTful APIs in Go/Gin for an ad-campaign management platform; secure API wrappers with dynamic header handling; prototyped a payment-gateway backend. |
| Smart Infrastructure Intern | Siemens, 2026 | Technical data sheets and PLC logic (SIMATIC S7-1200) for BMS and fire-alarm field devices. |

## Toolbox

`Python` · `Go` · `C++` · `C`
`PyTorch` · `NumPy` · `pandas` · `scikit-learn`
`quantisation` · `low-rank factorisation` · `entropy coding` · `rate–distortion optimisation`
`FastAPI` · `Flask` · `Gin` · `MongoDB`
`ESP32` · `Arduino` · `Embedded C`
