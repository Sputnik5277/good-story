# Good-Story Skill Adapter: Mining Engineering Domain

**Last updated**: 2026-06-04  
**Source data**: 11 published papers (EFA journal 6 + TAFM journal 5)  
**Domain**: Rock/coal mechanics, water infiltration, cyclic loading, failure mechanisms

---

## 1. Verified Narrative Arc

All 11 analyzed papers follow this exact six-stage structure:

### Stage 1: Field Belief
- **Domain fact**: Rock and coal degrade under water infiltration or cyclic loading
- **Status**: Established, widely known in the field
- **Implication**: Papers skip detailed background on *whether* degradation happens

### Stage 2: Gap (Knowledge Gap)
Papers identify specific gaps in understanding:
- Composite materials behavior (coal-concrete, loess-mudstone)
- Combined effects (water + mechanical loading simultaneously)
- Multi-scale phenomena (macro-level failure vs. micro-level damage evolution)
- Real material heterogeneity (natural coal seams, layered geological strata)

**Pattern**: Gap is always more specific than "we don't know X"; it's "we don't know X *under these specific combined conditions*"

### Stage 3: Approach
**Methodology constant across all 11 papers**:
1. Controlled laboratory experiments
2. Multiple test conditions (e.g., 0%, 50%, 100% saturation; or different loading cycles)
3. Real-time monitoring throughout tests
4. Reproducible specimen preparation

### Stage 4: Evidence (Multi-modal Data Fusion)
**Evidence hierarchy (implicit in all papers)**:

| Level | Evidence type | Role | Typical count |
|-------|---------------|------|---------------|
| Primary | Mechanical (stress-strain) | Loading path authority | 1 type |
| Secondary | AE (acoustic emission) | Crack activity monitoring | Often paired with primary |
| Tertiary | Visual (DIC, SEM, CT) | Failure morphology | 2-3 types |

**Key pattern**: Never use mechanism claims from single evidence type. Always triangulate:
- Example ✓: "Stress curve shows inflection → AE indicates crack initiation → SEM confirms crack morphology"
- Example ✗: "AE indicates crack initiation" (without stress curve support)

**Evidence prevalence in 11 papers**:
- AE (acoustic emission): 9/11 papers (82%)
- DIC (digital image correlation): 8/11 papers (73%)
- Microscopy (visual, SEM): 6/11 papers (55%)
- SEM (scanning electron microscopy): 5/11 papers (45%)
- CT scanning: 1/11 papers (9%)

### Stage 5: Claim
**What papers claim**:
- Quantitative parameter relationships (e.g., "porosity decreases 8% with saturation")
- Mechanism descriptions (e.g., "cracks concentrate at phase boundaries")
- Failure pattern categories (e.g., "shear vs. tensile failure modes")

**What papers NEVER claim**:
- Predictive models with error bounds
- Engineering specifications (e.g., "safe water depth limit")
- Operational guidance (e.g., "grouting prevents failure")
- Across-scale extrapolation (e.g., "lab findings apply to field tunnels")

### Stage 6: Consequence
**Conclusion strength distribution** (verified across 11 papers):
- **Engineering application** (7/11): Stop at suggesting practical relevance
- **Mechanistic explanation** (3/11): Stop at explaining *why* it fails
- **Quantitative relationships** (1/11): Stop at parameter relationships only

**Critical caveat**: Even papers labeled "Engineering application" do NOT prescribe actions.

Example ✓: "Water infiltration significantly reduces strength, suggesting the need for improved drainage design"  
Example ✗: "Drainage holes should be spaced 2m apart"

---

## 2. Claim Verb Standards

**Universal pattern**: All 11 papers use a single cautious verb: **"indicates"**

### Verb Strength Ranking
```
WEAKEST ← suggests → indicates → demonstrates → proves → STRONGEST
         correlation    mechanism     clear       proof
                      description     quantitative
```

### Implementation Rules

| Claim type | Verb | Example |
|-----------|------|---------|
| Correlation without mechanism | suggests | "High saturation suggests increased porosity" |
| Mechanism from multi-modal data | indicates | "AE indicates crack initiation; stress curve confirms inflection point" |
| Clear quantitative evidence | demonstrates | "Strength decreases 12±2% per saturation increment" |
| Proof (rare in domain) | proves | Avoid unless mathematical proof or unambiguous threshold |

### Why Domain Uses Cautious Verbs
1. **Material heterogeneity**: Natural samples show variability → can't claim universality
2. **Scale gap**: Lab samples (cm) vs. field (m) → extrapolation uncertain
3. **Mechanism complexity**: Multi-physics coupling (hydro-mechanical) → single explanations incomplete
4. **Threshold effects**: Failure is often abrupt; gradual transitions are approximations

---

## 3. Evidence Validation Rules

### Multi-Modal Requirement
**Rule**: Do not accept mechanism claims from a single evidence type.

**Minimum threshold**: 2 independent evidence types
- **Example ✓**: Stress-strain + AE (mechanical + acoustic)
- **Example ✓**: DIC + SEM (displacement field + morphology)
- **Example ✗**: AE alone ("AE indicates failure" without mechanical support)

### Evidence Licensing Pattern
In 11 papers, claims follow this licensing structure:

```
Mechanical data (stress-strain) 
    ↓ (provides baseline)
    → Acoustic/displacement data (AE, DIC) 
        ↓ (refines understanding)
        → Visual data (SEM, CT)
            ↓ (confirms failure morphology)
            → Final claim about mechanism
```

**Translation**: The *mechanical* evidence licenses *acoustic* claims. The *acoustic* evidence licenses *visual* interpretations. Never invert this order.

---

## 4. Consequence / Boundary Rules

### The Engineering Gap
All 11 papers exhibit a consistent boundary: they describe material behavior but avoid engineering prescriptions.

| Boundary level | Papers | Example | Example of crossing (✗ avoided) |
|--------|--------|---------|--------------------------------|
| Mechanism (cause-effect) | 3 | "Crack initiates at phase boundary due to stress concentration" | — |
| Quantitative (parameter relationships) | 4 | "Strength = f(saturation, loading rate)" | Claiming specific f() form without validation |
| Engineering (design implication) | 7 | "Results suggest improved drainage prevents damage" | "Design drainage with 2m spacing" |

**Why papers stop before prescription**:
1. Don't know whether lab conditions = field conditions
2. Multiple solutions exist for same problem (different materials, geometries)
3. Engineering decisions require economic/safety factors beyond mechanics

### Consequence Language Patterns
**Allowed softening language** (in 11 papers):
- "may lead to"
- "could result in"
- "suggests the need for"
- "implies potential for"
- "indicates importance of"

**Avoided strong language**:
- "will cause"
- "requires" (as obligation)
- "must be" (prescriptive)

---

## 5. Turning Point / Key Finding Pattern

### What Makes a Finding Surprising?
In 11 papers, "key findings" share this pattern: **deviation from single-mechanism assumption**

#### Example turning points:
1. **Non-linearity** (expected linear → observed plateau)
   - Expected: Strength drops monotonically with saturation
   - Actual: Sharp drop initially, then plateau at full saturation
   - Implication: Mechanism changes with degree of saturation

2. **Localization** (expected uniform → observed concentrated)
   - Expected: Failure occurs throughout sample
   - Actual: Failure concentrates at phase boundaries / weak planes
   - Implication: Heterogeneity is primary failure driver

3. **Temporal mismatch** (expected synchronized → observed staggered)
   - Expected: Acoustic/displacement/visual signals coincide
   - Actual: Acoustic precedes visible damage by significant time
   - Implication: Damage occurs at scales below visual detection

4. **Composite effects** (expected additive → observed interactive)
   - Expected: Effect(A) + Effect(B) = Combined effect
   - Actual: Interaction term dominates
   - Implication: Mechanisms not independent

### Why Turning Points Matter for Good-Story
The turning point is where the **single-mechanism model fails**.

This failure of simplicity **legitimates** the multi-modal evidence approach:
- If behavior were simple → one evidence type would suffice
- Because behavior is complex → multi-modal triangulation is necessary
- This makes the claim stronger, not weaker (≠ "we're confused")

---

## 6. Domain Context Constraints

### Subject Matter
All 11 papers concern:
- **Material**: Rock (sandstone, mudstone, coal) or composite (coal-concrete, loess-mudstone)
- **Stressor**: Water infiltration OR cyclic mechanical loading (or both)
- **Scale**: Laboratory (cm-scale samples)
- **Outcome**: Failure (crack propagation, strength loss, instability)

### Allowable Claims
- ✓ Mechanism at lab scale (cm-level)
- ✓ Parameter relationships (for tested conditions)
- ✓ Failure pattern categories
- ✓ Safety-critical observations (e.g., "early AE warning precedes visible failure")

### Not Allowable
- ✗ Direct field prediction (lab ≠ field)
- ✗ Design specifications
- ✗ Cross-material generalization (coal ≠ sandstone)
- ✗ Cross-stressor generalization (saturation ≠ cyclic loading dynamics)

---

## 7. Implementation Checklist for Mining Engineering Papers

When evaluating or writing a good-story claim in this domain:

- [ ] **Gap identification**: Is it specific to composite/complex/coupled scenario (not just "we don't know X")?
- [ ] **Evidence count**: Are ≥2 independent evidence types used?
- [ ] **Evidence order**: Is mechanical evidence primary, supporting acoustic/visual claims?
- [ ] **Claim verb**: Is verb "indicates" / "suggests" / "demonstrates" (not "proves")?
- [ ] **Consequence boundary**: Does claim stop at mechanism/quantitative (not prescriptive)?
- [ ] **Turning point**: Is there an explicit deviation from single-mechanism expectation?
- [ ] **Scale declared**: Is paper explicit about lab-scale limitation?
- [ ] **Softening language**: Are conditional words ("may", "could") used for implications?

---

## 8. Failure Modes (What NOT to Do)

### Red Flag 1: Strong Verbs Without Multi-Modal Support
❌ "AE demonstrates crack initiation at 40% stress" (no stress-strain confirmation)  
✓ "Stress curve shows inflection at 40% stress; concurrent AE indicates crack initiation"

### Red Flag 2: Skipping the Mechanism Explanation
❌ "Higher saturation leads to weaker rock" (why?)  
✓ "Higher saturation fills pores → increases pore pressure → reduces effective stress → explains lower strength"

### Red Flag 3: Blurring Lab ↔ Field Boundaries
❌ "This will prevent tunnel failure in loess strata"  
✓ "Results suggest improved understanding of loess degradation, which may inform tunnel design"

### Red Flag 4: Single Evidence Type Claims
❌ "SEM shows crack propagation" (observation of one sample)  
✓ "SEM shows crack propagation; consistent with AE temporal sequence and stress curve bifurcation"

### Red Flag 5: Missing the Turning Point
❌ "Results confirm existing knowledge that water reduces strength"  
✓ "Unexpectedly, strength reduction shows non-linear saturation dependence, with plateau at 80% saturation, suggesting a transition in failure mechanism"

---

## 9. Footnotes for Skill Calibration

### Why This Domain Is Demanding
1. **Material complexity**: Natural heterogeneity → claims must be hedged
2. **Scale gap**: Lab→field extrapolation always uncertain
3. **Multi-physics**: Water + mechanics are coupled, not independent
4. **Engineering stakes**: Safety-critical claims require extra care

### Why Multi-Modal Evidence Is Essential
Single evidence type (e.g., only AE) cannot distinguish:
- Real damage vs. sensor noise
- Damage location vs. damage mechanism
- Permanent damage vs. elastic deformation

Multi-modal approach resolves these ambiguities.

### Why Turning Points Matter
Turning points show that **complexity is real** (not just noise). This makes:
- The evidence more credible (not cherry-picked)
- The gap more legitimate (not just authors seeking to publish)
- The claim more robust (mechanism-based, not correlation-based)

---

## References (Source Papers)

1. Ding et al. (2026) - Tunnel lining failure, EFA
2. Li et al. (2026) - Water saturation, EFA
3. Xing et al. (2025) - Micro-macro fracture, EFA
4. Xu et al. (2026) - Coal-concrete composite, EFA
5. Zhou et al. (2025) - Crack evolution, EFA
6. Zhu et al. (2026) - Dynamic/static load, EFA
7. Lyu et al. (2026) - Dry-wet cycles, TAFM
8. Shen et al. (2026) - Macro-micro deterioration, TAFM
9. Shen et al. (2026) - In-situ mine water, TAFM
10. Wang et al. (2026) - Post-peak cyclic loads, TAFM
11. Zhou et al. (2026) - Brazilian splitting, TAFM

---

**Next steps**: Integrate this adapter into good-story skill's mining engineering branch. Test against papers in D:\00科研\omp\语料库.
