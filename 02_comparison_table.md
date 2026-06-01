---
---

# Conceptual Comparison Table

Eleven framings of body-worn / body-coupled systems, compared across eight
attributes. Transposed (concept = row) for readability. The final column states
each framing's relation to **wearable intelligence as perceptual media**.

> **How to read this:** the first five rows are *framings of the wearable itself*
> (tool → media); the last six are *loop/interaction paradigms* it can instantiate.
> Perceptual media is the synthesis the review argues toward; perception-in-the-loop
> is its mechanism.

---

## Part 1 — Framings of the wearable

| Framing | Role of user | Role of body | Role of system | Feedback type | Intelligence type | Main eval metric | Limitations | Relation to my framework |
|---|---|---|---|---|---|---|---|---|
| **Wearable as tool** | Operator of a task aid | Mounting surface / carrier | Passive instrument; does what it's told | None / direct readout | None (mechanical) | Task efficiency, ergonomics | Perception assumed fixed; body incidental | The baseline the review *displaces*; L0–L1 |
| **Wearable as computation** | Data subject / supervisor | Signal source | Senses, stores, computes, reports | Informational (display/log) | Algorithmic processing | Throughput, latency, accuracy | Treats perception as input only | The "what it computes" framing the review critiques; L1 |
| **Wearable as AI system** | Data subject; sometimes teacher | Source of features for models | Infers/predicts/classifies state | Inference outputs, alerts | Statistical/ML inference | Model accuracy, F1, AUROC | Accuracy-centrism; perception unmeasured | Front-half-of-loop only; claims L3, evaluates L1–L2 |
| **Wearable as feedback device** | Receiver of corrective signals | Target of correction | Detects deviation, signals it | Corrective (haptic/audio/visual) | Threshold/rule or control law | Error reduction, compliance | Trains compliance, risks dependency (guidance hyp.) | L2; *precursor* to perceptual media but not yet it |
| **Wearable as perceptual media** | Perceiver-actor in a coupling | **Site of mediated perception & loop partner** | Mediates what/how the wearer perceives & can act | Adaptive, perception-shaping, multimodal | *Coupled* human+machine intelligence | **Perceptual change, incorporation, agency, transfer** | Phenomenological mediation (Ihde) | **The thesis**; spans L3–L4 |

## Part 2 — Loop / interaction paradigms

| Paradigm | Role of user | Role of body | Role of system | Feedback type | Intelligence type | Main eval metric | Limitations | Relation to my framework |
|---|---|---|---|---|---|---|---|---|
| **Human-in-the-loop** | Supervisor / labeler / decider | Largely incidental | Defers to human judgment | Human→system corrections; system→human queries | Machine learning + human oversight | Model quality, trust, safety | Centers *cognition/supervision*, not perception | Sibling construct; differs by *locus* (mind vs. perception) |
| **Body-in-the-loop / HIL optimization** | Source of optimized response | Physiological cost signal (e.g., metabolic) | Optimizes assistance to bodily response | Implicit (parameter tuning) | Optimization over bodily signal | Metabolic cost, efficiency | Optimizes *physiology*, not lived perception | Close cousin; perception-in-the-loop generalizes the *target* to perception |
| **Closed-loop biofeedback** | Self-regulator | Physiological signal (HRV/EMG/breath) | Surfaces signal; nudges toward target | Continuous signal display | Control loop (often no ML) | Signal regulation, self-control | Single-signal; regulation ≠ perceptual reorganization | A *special case* (L2–L3) within perception-in-the-loop |
| **Sensory substitution** | Active explorer of a new sense | Sensorimotor coupling substrate | Maps one modality onto another | Persistent cross-modal stream | Mapping (often minimal ML) | Psychophysics, acquired perception | Long training; narrow tasks; siloed from HCI | The **paradigm case of L4** perceptual media |
| **Embodied interaction** | Meaning-maker in situated action | Locus of meaning & skill | Affords meaningful action | Multimodal, situated | (Design stance, not an algorithm) | Meaning, appropriation, experience | Descriptive; light on *adaptive* intelligence | Theoretical *parent*; perceptual media operationalizes it for intelligent wearables |
| **Perception-in-the-loop (mine)** | Perceiver-actor whose perception is the in-loop variable | Plastic, trainable perceiving body | Couples sensing→inference→feedback to *recalibrate perception* | Adaptive, perception-shaping, cross-modal | **Coupled** human+machine; both adapt | **Perceptual transformation, incorporation, agency, transfer** | Risk of conceptual overlap; must disambiguate (see review §5.2) | The **mechanism** of perceptual media |

---

## One-paragraph differentiation (drop-in for the paper)

> Perception-in-the-loop is easily confused with four neighbors, and the
> distinction is the *locus of the loop*. **Human-in-the-loop** places a *mind* in
> the loop to supervise a machine; the in-loop variable is human judgment.
> **Body-in-the-loop optimization** places a *physiological cost* in the loop;
> the in-loop variable is bodily efficiency. **Closed-loop biofeedback** places a
> *signal* in the loop to be regulated. **Active inference** is a theory of the
> brain, not a design construct. Perception-in-the-loop places the wearer's
> *lived, trainable perception* — felt body, salience, and possibilities for
> action — in the loop as the explicit target of design. It is compatible with
> active inference (which explains why precision-weighted feedback can retune
> perception) and subsumes biofeedback and sensory substitution as special cases
> at different loop depths.
