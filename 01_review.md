# Wearable Intelligence as Perceptual Media: A Systematic Integrative Review

*Citation key:* **[ANCHOR]** = canonical/high-confidence; **[VERIFY]** = confirm year/venue before submission.

---

## 1. Executive Summary

Wearable computing has been narrated as a succession of technical achievements:
miniaturized sensors, body-worn computation, on-device machine learning, and
increasingly "smart" feedback. This framing is productive but conceptually thin.
It tells us what wearables *contain* (sensors, models, actuators) and what they
*do to data* (record, classify, predict), but it is largely silent on what they
*do to the wearer* — on how a body-coupled system changes the way a person
perceives, feels, and acts through their own body.

This review advances a different reading. **Intelligent wearables are best
understood as *perceptual media*: body-worn or body-coupled systems that mediate
how users perceive their bodies, environments, and possibilities for action.**
On this view a vibrotactile gait trainer is not primarily a "feedback device"
and a sensory-substitution belt is not primarily a "classifier with actuators";
both are media through which perception is *reorganized*. The argument
synthesizes four traditions that rarely meet: (i) wearable/ubiquitous computing
and wearable AI; (ii) the phenomenology and media theory of technological
mediation (McLuhan, Merleau-Ponty, Polanyi, Ihde); (iii) ecological and enactive
theories of perception-action (Gibson, Varela, Noë, O'Regan); and (iv) the
empirical literatures of augmented feedback, biofeedback, sensory substitution,
rehabilitation, haptics, smart textiles, and AR/XR.

From this synthesis I develop three contributions:

1. **A mechanism — *perception-in-the-loop*.** A cyclic coupling in which
   wearable sensing, computational inference, and adaptive feedback continuously
   reshape the wearer's embodied perception *and* action, which in turn change
   what is sensed. This is distinguished from human-in-the-loop (which centers
   human *supervision/cognition*) and from closed-loop biofeedback (which centers
   *signal regulation*) by locating the intervention in **perception** — the
   wearer's lived sense of their body and environment — not merely in data or
   decisions.

2. **An analytical tool — the *Loop-Depth Taxonomy*.** Five levels (L0 Record →
   L1 Inform → L2 Correct → L3 Recalibrate → L4 Incorporate) that grade *how
   deeply a system enters the perception-action loop*, crossed with three
   orthogonal axes (who adapts, over what timescale, and at what locus —
   data/cognition/perception/body-schema). This separates "technically
   sophisticated feedback" from "deep perceptual integration," which the field
   routinely conflates.

3. **A design agenda — *Perceptual Scaffolding*.** Six principles for designing
   wearables that *build up* perceptual capacity rather than create dependency:
   scaffold-then-fade, design for awareness not only correction, keep adaptation
   legible and agency intact, respect the body schema, exploit cross-modal
   sensorimotor contingencies, design for body diversity, and — critically —
   *evaluate perceptual change, not only task accuracy*.

**Why the framing is valuable.** It reorients evaluation (from accuracy to
perceptual transformation), surfaces neglected stakes (agency, dependency, body
diversity, long-term incorporation), and unifies fragmented sub-literatures
under one analytic. It also gives HCI a vocabulary for systems — sensory
substitution, exosuits, EMS interfaces, AR rehabilitation — that are obviously
*more* than feedback devices but for which the field lacks a shared theory.

---

## 2. Search Strategy

> Full reproducible protocol (strings, databases, PRISMA flow, screening rules)
> lives in `05_search_protocol.md`. This section summarizes the logic.

**Review type.** *Systematic integrative review* (Whittemore & Knafl 2005
**[VERIFY]**; Torraco 2005 **[VERIFY]**): systematic, transparent search and
screening, but with the explicit goal of *theory building / conceptual
synthesis* across heterogeneous evidence (empirical systems, theoretical texts,
clinical studies, design artifacts) rather than effect-size aggregation. This is
the appropriate genre because the contribution is a framework, and because the
relevant evidence spans incommensurable methods (a phenomenology essay and an RCT
of a gait trainer both inform the argument but cannot be pooled).

**Databases.** ACM Digital Library, IEEE Xplore, Scopus, Web of Science;
hand-search of CHI, UIST, DIS, TEI, ISWC, UbiComp/IMWUT, PACM HCI, plus
*ToCHI*, *IJHCS*, *J. NeuroEngineering and Rehabilitation*, *IEEE Trans. Haptics*,
and key cognitive-science venues for theory anchors.

**Five keyword clusters** (A wearable computing/AI; B embodied
interaction/perception-action; C feedback/biofeedback/sensory substitution; D
rehabilitation/movement; E AR/XR perceptual interfaces) — see protocol file.

**Inclusion** (≥1 required): body-worn/body-coupled interactive system; sensing
of bodily/physiological/behavioral/environmental state; user-facing feedback
(visual/haptic/auditory/thermal/textile/robotic/AR-XR); adaptive/intelligent
response; or substantive discussion of perception, bodily awareness, action,
motor learning, or embodied experience relevant to HCI/health/rehab/
accessibility/sports/embodied interaction. **Theory texts** are admitted as a
parallel track (the "conceptual anchor" corpus) even when they describe no device.

**Exclusion / deprioritization:** pure sensor *fabrication* with no user-facing
interaction; pure algorithm *benchmarks* with no embodied loop; commercial
smartwatch marketing without research contribution; medical-device trials with no
treatment of interaction or perception; pure hardware optimization (battery,
antenna, RF) unless central to the interaction.

**Two-corpus design (recommended).** Keep a **systems corpus** (screened against
PRISMA, coded in `03_coding_scheme.csv`, classified by loop depth) and a smaller
**conceptual-anchor corpus** (theory/foundational works that ground the
framework). Report them separately so reviewers see the systematic screening
without forcing Merleau-Ponty through an inclusion checklist.

---

## 3. Key Literature Clusters

Representative anchors only; full annotations in `04_annotated_bibliography.md`.

### Cluster A — Wearable computing & intelligent wearables
Foundational definitions of wearable computing as *constant, augmenting,
context-aware* body-worn computation: Mann's wearable/"humanistic" computing and
mediated reality **[ANCHOR]**; Starner et al. on augmented reality through
wearables **[VERIFY]**; Rhodes' wearable Remembrance Agent **[VERIFY]**; Picard's
*Affective Computing* **[ANCHOR]**; situated in Weiser's ubiquitous computing
**[ANCHOR]**. *What this cluster gives the argument:* the historical baseline —
wearables defined by *what they compute*, with perception treated as an
input channel, not an output that is transformed. This is precisely the framing
the review displaces.

### Cluster B — Embodied interaction & perception-action (conceptual anchors)
Dourish, *Where the Action Is* **[ANCHOR]** (embodied interaction; Heideggerian
ready-to-hand); Klemmer et al., "How bodies matter" **[VERIFY]**; phenomenology
of incorporation — Merleau-Ponty's body schema and the blind man's cane / the
feather in the hat **[ANCHOR]**; Polanyi's *tacit dimension* (subsidiary vs.
focal awareness; tools we attend *from*) **[ANCHOR]**; Gallagher on body schema
vs. body image **[ANCHOR]**; ecological perception and affordances (Gibson)
**[ANCHOR]**; enactive/sensorimotor accounts (Varela/Thompson/Rosch; Noë;
O'Regan & Noë) **[ANCHOR]**; predictive processing / active inference (Friston;
Clark) **[ANCHOR]**; the extended mind and "natural-born cyborgs" (Clark &
Chalmers; Clark) **[ANCHOR]**. *What this gives the argument:* the theoretical
machinery for "perceptual media" and for treating perception as *plastic and
trainable*, not fixed.

### Cluster C — Feedback, biofeedback & sensory substitution
The empirical heart. Augmented-feedback motor-learning reviews (Sigrist et al.,
"Augmented visual, auditory, haptic, and multimodal feedback in motor learning")
**[ANCHOR]** and the *guidance hypothesis* (Salmoni, Schmidt & Walter; concurrent
feedback can create dependency) **[ANCHOR]**; wearable-haptics review (Shull &
Damian, "Haptic wearables as sensory replacement, sensory augmentation and
trainer") **[ANCHOR]**; tactile motor-learning suits (Lieberman & Breazeal, TIKL)
**[VERIFY]**; sensory substitution (Bach-y-Rita's tactile-vision substitution;
Bach-y-Rita & Kercel) **[ANCHOR]**, the vOICe (Meijer) **[VERIFY]**, the feelSpace
magnetic belt (Nagel et al.) **[VERIFY]**, the sensory-substitution VEST
(Novich & Eagleman) **[VERIFY]**; electrical muscle stimulation as I/O and the
agency questions it raises (Lopes & Baudisch and colleagues) **[VERIFY]**.
*What this gives the argument:* direct evidence that wearable feedback changes
*perception, proprioceptive acuity, bodily awareness, and action strategy* — not
just performance — and the cautionary evidence (dependency) that motivates
scaffolding.

### Cluster D — Rehabilitation, health & movement wearables
Real-time biofeedback for gait retraining (e.g., running-mechanics feedback;
wearable gait-retraining systems) **[VERIFY]**; soft exosuits (Harvard;
post-stroke gait) **[VERIFY]**; *human-in-the-loop optimization* of exoskeleton
assistance (Zhang et al., *Science*) **[ANCHOR]** — a key contrast case;
prosthesis embodiment and illusory-movement feedback (Marasco et al.) **[VERIFY]**;
"neurocognitive barriers to the embodiment of technology" (Makin, de Vignemont &
Faisal) **[ANCHOR]**; personal-informatics models (Li, Dey & Forlizzi;
lived-informatics, Rooksby et al.; Choe et al.) **[ANCHOR]**. *What this gives the
argument:* the L2–L4 systems, plus the embodiment/incorporation literature that
defines the deep end of the loop.

### Cluster E — AR/XR & perceptual interfaces
Sense of embodiment in VR (Kilteni, Groten & Slater; ownership/agency/
self-location) **[ANCHOR]**; rubber-hand illusion as the canonical demonstration
of malleable body ownership (Botvinick & Cohen) **[ANCHOR]**; EMS-actuated force
feedback and "affordance" overlays in MR (Lopes et al.) **[VERIFY]**; AR
movement-guidance and rehabilitation systems **[VERIFY]**. *What this gives the
argument:* the clearest cases of wearables acting as perceptual media by
*overlaying cues, redirecting attention, and rewriting felt body boundaries.*

### Cross-cutting — Somaesthetics, agency, integration
Soma design / somaesthetic interaction (Höök; Schiphorst) **[ANCHOR/VERIFY]**;
sense of agency in HCI (Limerick, Coyle & Moore; Coyle et al. "I did that!")
**[VERIFY]**; *Human-Computer Integration* (Mueller et al., "Next Steps for
Human-Computer Integration") **[VERIFY]**; postphenomenology of mediation (Ihde;
Verbeek) **[ANCHOR]**; scaffolding (Wood, Bruner & Ross; Vygotsky's ZPD)
**[ANCHOR]**.

---

## 4. Historical / Conceptual Shift

The review tells the field's history as a migration of *what we think a wearable
is for*. Each stage subsumes rather than erases the previous one.

**(i) Wearable as tool / prosthesis-of-task (≈1960s–1990s).** The wearable
extends a *task capacity*: a head-up display, a body-worn camera, a hands-free
terminal. The body is a *mounting surface*; perception is assumed stable; success
= task efficiency. (Mann; Starner; Rhodes.)

**(ii) Wearable as computation & context (≈1990s–2010s).** With ubicomp (Weiser)
and affective/context-aware computing (Picard), the wearable becomes a *sensing
and inference engine*: it measures the body and environment, classifies state,
and reports or triggers. The body becomes a *signal source*; perception is an
*input*; success = accuracy / classification performance / engagement. This is
the dominant contemporary framing — "wearable AI" as on-body machine learning —
and the one this review argues is incomplete.

**(iii) Wearable intelligence as perceptual media (emerging).** The wearable's
*output* is no longer (only) data or actions in the world but a *change in the
wearer's perception*: what they feel of their own posture, where they sense the
boundary of their body, which affordances become salient, how confidently they
move. The body is a *site of mediated perception and a partner in a loop*;
perception is the *thing being designed*; success = **perceptual recalibration,
incorporation, agency, and transfer** — not accuracy alone.

The key conceptual pivot is from **measuring the body** to **mediating
perception**. Postphenomenology names the move precisely: in Ihde's *embodiment
relation*, technology withdraws from attention and we perceive the world
*through* it (the glasses, the cane); the wearable becomes part of the perceiving
body rather than an object perceived. McLuhan's "extensions of man" supplies the
media framing — wearables extend (and amputate, and reorganize) the sensorium.
Merleau-Ponty and Polanyi supply the mechanism of *incorporation* and
*transparency*. Gibson supplies the object of perception that wearables most
distinctively reshape: **possibilities for action** (affordances). The synthesis
of these four is what "perceptual media" denotes.

---

## 5. The Perception-in-the-Loop Framework

### 5.1 The cycle

Perception-in-the-loop models the wearable + wearer as a single coupled system
turning through six phases:

```
        ┌──────────────────────────────────────────────────────────┐
        │                                                            │
        ▼                                                            │
   (1) SENSING ──► (2) INFERENCE ──► (3) FEEDBACK ──► (4) PERCEPTUAL │
   body / physio /   classify /        visual/haptic/    RECALIBRATION
   behavior / env    estimate /        audio/thermal/    (felt body,
                     predict           textile/EMS/AR    salience, affordances)
                                                            │
                                                            ▼
                                              (5) EMBODIED ACTION
                                              (posture, gait, gesture,
                                               attention, strategy, confidence)
                                                            │
                                                            ▼
                                              (6) NEW SENSING  ──┐
                                              (the world & body  │
                                               are now different)│
        └───────────────────────────────────────────────────────┘
```

Two nested loops run at different timescales:
- **Fast loop (moment-to-moment):** sensing → feedback → action → sensing. This is
  the control loop most engineering papers optimize.
- **Slow loop (developmental):** repeated cycles produce *perceptual learning* and
  *incorporation* — the cane becomes transparent, the substitution belt yields a
  "sixth sense," proprioceptive acuity changes. This slow loop is where
  "perceptual media" lives and where the field has the least evidence.

And two directions of adaptation, which must be tracked separately:
- **System→user adaptation** (the wearable changes the wearer's perception/action);
- **User→system adaptation** (the wearer learns to read, trust, and exploit the
  wearable). Genuine perception-in-the-loop requires *both*; pure
  system→user with no user learning is closer to remote control than to media.

### 5.2 How it differs from neighboring constructs

| Construct | Locus of the loop | What "closes" it | What it optimizes |
|---|---|---|---|
| **Human-in-the-loop (ML/control)** | Human *cognition/supervision* | Human label, decision, veto | Model quality, safety, control accuracy |
| **Body-in-the-loop / HIL optimization** | Body's *physiological response* (e.g., metabolic cost) | Measured bodily cost signal | Assistance parameters, efficiency |
| **Closed-loop biofeedback** | A *physiological signal* (HRV, EMG, breath) | Signal returns to target band | Self-regulation of that signal |
| **Interactive machine learning** | Human *teaching* the model | User-supplied examples/corrections | Model adapted to user |
| **Embodied interaction** | *Meaning-in-action* | (not a control loop per se) | Situated, meaningful action |
| **Active inference** | *Prediction error* | Action/perception minimizes surprise | Free-energy / prediction-error minimization |
| **Perception-in-the-loop (this work)** | The wearer's *perception* (felt body, salience, affordances) | Perception is recalibrated and re-coupled to action | **Perceptual transformation, incorporation, agency, transfer** |

**The differentiation you must make explicit:** HITL puts a *mind* in the loop to
supervise a machine; biofeedback puts a *signal* in the loop to be regulated;
active inference is a *theory of the brain*, not a design construct.
Perception-in-the-loop is a **design and analytic construct that puts the lived,
trainable perception of the wearer in the loop as the target of design.** It is
*compatible with* active inference (which explains *why* perception can be
retuned by feedback — the brain re-weights sensory precision) and *builds on* the
perception-action cycle (Fuster) and sensorimotor-contingency theory (O'Regan &
Noë, which explains *how* substitution yields genuinely new perception). Present
it as **an integrative reframing, not a discovery** — that is both honest and more
robust to reviewer pushback.

### 5.3 Is the term original / useful?
- **Useful: yes.** It names a real gap — no existing term foregrounds *perception*
  (as opposed to cognition, signal, or model) as the in-loop variable that
  wearables most distinctively reshape.
- **Original: partially.** Search shows scattered, non-canonical uses of
  "perception in the loop" in robotics/vision (where it means a perception
  *module* in an autonomy stack — a different, machine-perception sense).
  **Recommendation:** adopt the term but (a) explicitly disambiguate from the
  robotics usage, (b) anchor it to the perception-action cycle and sensorimotor
  contingencies, and (c) define it crisply as *human* perception-in-the-loop. This
  protects priority while acknowledging precedent.

---

## 6. The Loop-Depth Taxonomy

### 6.1 The five levels (refined)

The depth of a wearable = *how far into the perception-action loop it reaches*.

| Level | Name | Definition | Loop status | Exemplars |
|---|---|---|---|---|
| **L0** | **Record** | Captures data; no real-time user-facing feedback. | Open | Passive sleep/HR loggers; research IMU capture |
| **L1** | **Inform** | Reports state/data to the user for interpretation. | Open→semi (user closes it cognitively) | Step count, HR zones, activity dashboards |
| **L2** | **Correct** | Detects deviation from a target state and signals corrective feedback. | Semi-closed | Posture buzzers, gait/cadence cueing, movement coaching |
| **L3** | **Recalibrate** | *Adapts* feedback to user state/context/performance and supports *bodily awareness / perceptual recalibration*, not just error-nulling. | Closed, single-session | AR rehab cueing, adaptive balance feedback, fatigue-aware coaching, personalized haptic guidance |
| **L4** | **Incorporate** | Becomes integrated into the wearer's *long-term* perception-action system; functions as a perceptual partner/extension; new perceptual capacities emerge. | Closed, developmental | Sensory substitution (TVSS/vOICe/feelSpace/VEST), embodied prostheses, adaptive exosuits, long-horizon embodied AR |

### 6.2 The problem with a single ladder — and the fix

Your draft ladder conflates **two things that can vary independently**:
- *Feedback sophistication* (static → adaptive), and
- *Degree of bodily incorporation* (object I use → part of my perceiving body).

A system can be adaptive but never incorporated (a clever coaching app), or
non-adaptive but deeply incorporated (a simple long-worn substitution device that
becomes "transparent"). To stop reviewers collapsing the taxonomy, **report the
level *plus* three cross-cutting axes:**

1. **Who adapts?** {system→user / user→system / both}. L4 generally requires *both*.
2. **Timescale of effect:** {momentary control / single-session learning /
   developmental incorporation}.
3. **Locus of intervention:** {data → cognition → perception → body schema}. The
   shift from "perception" to "body schema" marks the L3→L4 boundary.

A paper is then coded e.g. `L3 · system+user · single-session · perception` vs.
`L4 · both · developmental · body-schema`. This makes the taxonomy *diagnostic*
rather than merely ordinal.

### 6.3 Reading rules & caveats
- **Depth ≠ virtue.** A well-designed L1 tracker may serve a user better than a
  poorly designed L4 system. The taxonomy measures *reach into perception*, not
  quality or appropriateness.
- **Code the realized loop, not the claimed one.** Many "AI wearables" claim L3
  adaptivity but evaluate only L1/L2 outcomes (accuracy, detection). Code what the
  *paper demonstrates*, and note the gap (see §8).
- **Most of the field clusters at L1–L2.** A central empirical finding to report:
  the literature is bottom-heavy; L3 is thin and mostly single-session; **L4 is
  dominated by sensory-substitution and prosthetics work that rarely cites HCI**,
  and HCI rarely cites it. The review's value is partly in *connecting* these.

---

## 7. Design Principles — Perceptual Scaffolding for Embodied Interaction

*Perceptual scaffolding* = designing wearables that **temporarily support
perception so that the wearer builds durable perceptual capacity**, then
withdrawing support — analogous to instructional scaffolding (Wood, Bruner &
Ross; Vygotsky's ZPD) but applied to *perception-action*, not concept learning.
The animating worry is the **guidance hypothesis**: feedback that is too rich,
constant, or directive produces *dependency* — performance collapses when the
wearable is removed (Salmoni, Schmidt & Walter; Sigrist et al.). Good perceptual
media make themselves progressively *unnecessary* — or, at L4, make themselves
*part of the wearer*. Either way, dependency-without-incorporation is the failure
mode.

**P1 — Scaffold, then fade.** Default to *fading* feedback as competence grows
(reduced frequency, bandwidth, or directiveness); reserve persistent feedback for
genuine substitution/augmentation (L4) where the capacity *is* the device.
Concurrent feedback aids in-session performance but can impair retention — design
for *transfer*, and measure it after removal.

**P2 — Design for bodily awareness, not only correction.** Move beyond
error-nulling (L2) toward *recalibration* (L3): help wearers *notice* their body
(proprioception, breath, tension, balance) rather than merely obey a buzzer.
Somaesthetic / soma-design methods (Höök; Schiphorst) and slow, exploratory
feedback support this; correction-only systems train compliance, not perception.

**P3 — Make adaptation legible; preserve agency.** When the system adapts
(changes thresholds, switches strategies, actuates the body via EMS/exosuit),
the wearer should be able to perceive *that* and *why* it adapted, and retain a
sense of authorship over the resulting action. EMS and strong robotic assistance
threaten the *sense of agency* (Limerick, Coyle & Moore; Lopes et al.). Provide
override, gradual handover, and signifiers of system state; measure agency
explicitly.

**P4 — Respect (and design for) the body schema.** Decide deliberately whether a
system should become *transparent* (ready-to-hand, incorporated — good for L4
extension) or *reflective* (present-at-hand — good for L3 awareness). Support
incorporation with consistent, body-coupled, low-latency, spatially congruent
feedback (the conditions under which canes, belts, and prostheses get absorbed
into the body schema). Beware "neurocognitive barriers to embodiment" (Makin et
al.): mismatched, delayed, or non-contingent feedback blocks incorporation.

**P5 — Exploit cross-modal sensorimotor contingencies.** Perception is defined by
*lawful sensorimotor coupling* (O'Regan & Noë), which is why substitution works:
a stable mapping between the wearer's movement and the feedback lets a new
"sense" emerge. Choose modality and mapping for *contingency and learnability*,
not raw bandwidth; support multiple modalities and let the wearer move to explore
the signal (active, not passive, stimulation).

**P6 — Design for body diversity and plasticity.** Bodies, sensoria, and schemas
differ (disability, aging, neurodivergence, athletic expertise). Perceptual media
must be *calibratable and re-mappable* to the individual body, and must not assume
a normate body. This is both an accessibility imperative and a scientific one
(plasticity is the resource the design exploits).

**P7 (meta-principle) — Evaluate perceptual change, not only task performance.**
The previous six fail silently if we only measure accuracy/RMSE/adherence.
Recommended perceptual-change measures: proprioceptive acuity (joint
position-matching), body-ownership/agency questionnaires and the
embodiment construct (Kilteni et al.; rubber-hand–style measures), intentional
binding for implicit agency, transfer/retention tests *after device removal*,
psychophysical thresholds for substituted modalities, and qualitative
phenomenological accounts (micro-phenomenology) of how the body "feels different."

---

## 8. Gaps in Current Literature

1. **Accuracy-centrism.** The dominant outcome is detection/classification
   performance. Whether the wearer *perceives or acts differently* is frequently
   unmeasured. (Mismatch between claimed L3 adaptivity and L1/L2 evaluation.)
2. **Under-theorized perception.** "Feedback" is treated as information delivery;
   the phenomenology of *how perception is reshaped* (incorporation,
   recalibration, affordance shift) is rarely engaged outside the
   substitution/prosthetics niche.
3. **Neglect of agency.** Increasingly *actuating* wearables (EMS, exosuits,
   strong haptics) raise authorship/control questions that are seldom measured;
   sense-of-agency instruments are underused in wearable HCI.
4. **Short-horizon, lab-bound evaluation.** The *slow loop* (developmental
   incorporation, perceptual learning) needs longitudinal, in-the-wild study;
   most evaluations are single-session. L4 claims rest on a small,
   discipline-siloed evidence base.
5. **No standard measures of perceptual change.** Without shared instruments, L3/L4
   claims aren't comparable. (P7 proposes a starter battery.)
6. **Sensing >> transformation.** Effort concentrates on *what the device can
   sense/infer*, far less on *what the wearer becomes able to perceive*. The field
   optimizes the front half of the loop (sensing/inference) and neglects the back
   half (recalibration/incorporation).
7. **Disciplinary siloing.** Sensory-substitution/prosthetics (deep L4 evidence),
   motor-learning/feedback science (the dependency cautions), HCI/soma design
   (agency, lived experience), and wearable-AI (sensing/inference) rarely cite one
   another. The review's connective work is itself a contribution.

---

## 9. Future Research Agenda

- **A1. Measurement program.** Develop and validate a *perceptual-change battery*
  for wearables (proprioceptive acuity, embodiment/agency, transfer-after-removal,
  substituted-modality psychophysics) so L3/L4 claims become comparable. *Highest
  leverage.*
- **A2. Longitudinal incorporation studies.** In-the-wild, multi-week studies of
  the *slow loop*: when do AR-rehab, exosuit, or substitution wearables become
  transparent / incorporated, and what design factors govern it (latency,
  congruence, contingency, consistency)?
- **A3. Agency-preserving actuation.** For EMS/exosuit/strong-haptic systems,
  principled handover and legibility mechanisms that maximize assistance while
  preserving the sense of agency; report agency as a first-class outcome.
- **A4. Scaffold-and-fade architectures.** Wearables that *plan their own
  obsolescence* — adaptive fading policies that promote transfer; compare against
  persistent-feedback baselines on retention, not just in-session performance.
- **A5. Perceptual media for accessibility.** Treat sensory substitution/
  augmentation as the paradigm case of perceptual media; build calibratable,
  body-diverse systems and study long-term perceptual incorporation with disabled
  co-designers (P6).
- **A6. Cross-modal mapping science for HCI.** Systematic study of which
  sensorimotor mappings are *learnable and incorporable*, importing
  sensorimotor-contingency theory into wearable feedback design (P5).
- **A7. Theory consolidation.** Position perception-in-the-loop relative to active
  inference and the perception-action cycle empirically — e.g., test whether
  feedback that the active-inference account predicts to be "precision-enhancing"
  yields measurably faster incorporation.

---

## 10. Annotated Bibliography

See `04_annotated_bibliography.md` (categorized; ~60 anchor works, each with a
one-line statement of why it matters to the argument).

---

## Refined Thesis (Section 10 of the brief)

> This review argues that wearable intelligence should be understood not merely as
> body-worn sensing or AI-enabled computation, but as **perceptual media**:
> body-coupled systems that shape how people perceive, interpret, and act through
> their bodies. Through a systematic integrative review spanning wearable
> computing, embodied interaction, augmented-feedback and sensory-substitution
> science, rehabilitation, and AR/XR, I (1) introduce **perception-in-the-loop**
> as the mechanism by which wearables function as perceptual media — a dynamic
> coupling of sensing, inference, feedback, perceptual recalibration, and embodied
> action that is distinct from human-in-the-loop supervision and closed-loop
> signal regulation; (2) develop a **loop-depth taxonomy** that grades how deeply
> systems enter the perception-action loop, from passive recording to long-term
> perceptual incorporation; and (3) propose **perceptual scaffolding** as a design
> agenda that builds durable perceptual capacity, preserves agency, and is
> evaluated by perceptual change rather than task accuracy alone.

*(Structure preserved from your draft; tightened for precision and to foreground
the three contributions and the key differentiation from HITL/biofeedback.)*
