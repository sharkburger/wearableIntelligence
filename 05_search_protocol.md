# Search Protocol (Methods Section Draft)

Reproducible search strategy for the systems corpus, plus the parallel
conceptual-anchor track. Designed for ACM DL, IEEE Xplore, Scopus, Web of Science.

---

## 1. Databases & venues
- **Full-text/index databases:** ACM Digital Library, IEEE Xplore, Scopus, Web of
  Science Core Collection.
- **Targeted venue hand-search:** CHI, UIST, DIS, TEI, ISWC, UbiComp/IMWUT, PACM
  HCI, ToCHI, IJHCS; plus *J. NeuroEngineering & Rehabilitation*, *IEEE Trans.
  Haptics*, *IEEE Trans. Neural Systems & Rehab Eng.* for systems; *Behavioral &
  Brain Sciences*, *Trends in Cognitive Sciences*, *Phenomenology and the
  Cognitive Sciences* for the conceptual track.
- **Backward/forward snowballing** from the anchor set in `04_annotated_bibliography.md`.

## 2. Date window
- Systems corpus: 1995–present (post-Mann wearable-computing era).
- Conceptual anchors: no date limit (Merleau-Ponty 1945 onward).

## 3. Search strings (adapt syntax per database)

**Cluster A — wearable computing & AI**
```
("wearable comput*" OR "wearable intelligen*" OR "intelligent wearable*"
 OR "wearable AI" OR "smart wearable*" OR "body-worn comput*"
 OR "context-aware wearable*" OR "adaptive wearable*")
```

**Cluster B — embodied interaction & perception-action**
```
("embodied interaction" OR "perception-action" OR "sensorimotor"
 OR "body schema" OR "body awareness" OR "embodied cognition"
 OR "perceptual coupling" OR "perceptual learning" OR "active inference"
 OR "enactive")
```

**Cluster C — feedback / biofeedback / sensory substitution**
```
("wearable feedback" OR "biofeedback" OR "haptic feedback"
 OR "sensory substitution" OR "sensory augmentation" OR "augmented perception"
 OR "movement feedback" OR "real-time feedback")
```

**Cluster D — rehabilitation & movement**
```
("wearable rehabilitation" OR "gait retraining" OR "posture correction"
 OR "motor learning" OR "physical therapy wearable" OR "assistive wearable"
 OR "exosuit" OR "exoskeleton" OR "prosthes*") 
```

**Cluster E — AR/XR perceptual interfaces**
```
("augmented reality" OR "mixed reality" OR "smart glasses" OR "XR")
 AND (wearable OR body OR perception OR rehabilitation OR "movement guidance")
```

**Recommended combination for the systems corpus** (AND across a body-coupling
term, a feedback/perception term, and an interaction term):
```
(Cluster A OR "wearable" OR "body-worn" OR "on-body")
AND (Cluster C OR "feedback" OR "perception" OR "body awareness")
AND ("interaction" OR "user study" OR "HCI" OR "experience" OR "motor learning"
     OR "rehabilitation")
```

## 4. Inclusion criteria (≥1 required)
1. Body-worn or body-coupled **interactive** system.
2. Sensing of bodily / physiological / behavioral / environmental state.
3. User-facing feedback (visual, haptic, auditory, thermal, textile, robotic, AR/XR).
4. Adaptive or intelligent response based on user state.
5. Substantive discussion of perception, bodily awareness, action, motor learning,
   feedback, or embodied experience.
6. Relevance to HCI, health, rehab, accessibility, sports, or embodied interaction.

## 5. Exclusion / deprioritization
- Pure sensor **fabrication** with no user-facing interaction.
- Pure algorithm **benchmark** with no embodied/wearable loop.
- Commercial smartwatch **marketing** without research contribution.
- Medical-device **trials** with no treatment of interaction or perception.
- Hardware optimization (battery, antenna, RF, power) unless central to interaction.

## 6. Two-corpus rule
- **Systems corpus** → PRISMA-screened, coded in `03_coding_scheme.csv`, classified
  by loop depth (§6 of review).
- **Conceptual-anchor corpus** → purposive, theory/foundational works (exempt from
  inclusion checklist); reported separately.

## 7. Screening flow (PRISMA 2020 — fill in counts)
```
Records identified (DB n=____ ; venue hand-search n=____ ; snowball n=____)
        │  duplicates removed (n=____)
        ▼
Title/abstract screened (n=____)  ──► excluded (n=____ ; reasons logged)
        ▼
Full-text assessed (n=____)       ──► excluded (n=____ ; reasons logged)
        ▼
Included in systems corpus (n=____)   + conceptual anchors (n=____)
```

## 8. Coding & reliability
- Extract per `03_coding_scheme.csv` (basic / system / perception-in-the-loop /
  theoretical-contribution fields + loop level + 3 cross-cutting axes).
- Double-code a 15–20% sample for loop-level and locus; report agreement
  (e.g., Cohen's κ); resolve by discussion; refine level definitions if κ low —
  this *is* part of "testing whether the taxonomy works."

## 9. Notes for your filmAI/eye-tracking workflow parity
You ran prior scoping reviews (`filmAI`, `eyetrackingWild`) with explicit
include/exclude verification passes and per-domain coding. Mirror that here:
keep a running screening log, a decisions/edge-cases note, and a versioned
`03_coding_scheme.csv`. Because this is *integrative*, also keep a short
**theory-memo** file capturing how each anchor reshapes the framework as you read.
