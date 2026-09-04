# A candidate therapy for a homozygous LIPK + LIPN deletion

**Status: research proposal. Not a treatment, not medical advice, never tested in a human.**
Prepared from public genetic and clinical literature. The patient's actual genetic report has
not been reviewed. Every step below requires a treating physician and an institutional
research team.

---

## 1. The problem, stated precisely

A boy (referred to here as the patient) in Mosul, Iraq, reportedly carries a deletion on
chromosome 10 that removes two genes entirely: **LIPK** and **LIPN**. Both sit in the
epidermal lipase cluster at **10q23.31**.

| Gene | Protein | Where it works | Known disease |
|---|---|---|---|
| LIPN | Lipase family member N | Granular layer keratinocytes, upregulated during differentiation | Autosomal recessive congenital ichthyosis type 8 (ARCI8), OMIM 613943 |
| LIPK | Lipase family member K | Epidermis only, final step of keratinocyte differentiation | None described in humans |

Both are secreted alpha/beta hydrolase lipases with intact catalytic triads. Both are
expressed almost exclusively in skin. Losing them means the outermost skin layers cannot
process the lipids that form the water barrier. The clinical result is severe
ichthyosis: thick adherent scale, everted eyelids and lips, hair loss, fissuring,
infection, water and heat loss, and pain.

**Why this case is unusual.** Published ARCI8 comes from point mutations in LIPN.
A complete deletion of both LIPN and LIPK together has not been reported. There is no
patient population, no natural history data, and no company with a program.

### 1.1 Three things to verify before anything else

These change the entire plan and can be read off the existing sequencing data today.

1. **Is the deletion homozygous?** ARCI8 is recessive. A therapy design assumes both
   copies are gone. If one intact copy remains, the deletion is not the explanation and
   the diagnosis is wrong.
2. **Does the deletion extend to LIPA?** Lysosomal acid lipase sits in the same band.
   Losing it causes Wolman disease, which affects liver, spleen, and adrenal glands, and
   which has an approved enzyme replacement therapy (sebelipase alfa). If LIPA is
   involved, that is an urgent, separately treatable condition.
3. **Does the deletion extend to PTEN?** The PTEN tumour suppressor lies in the same
   cytoband. Loss of one copy causes a cancer predisposition syndrome requiring lifelong
   surveillance. This must be excluded explicitly.

Also record whether LIPJ and LIPM, the other two cluster members, are inside the deleted
segment, and record the exact breakpoint coordinates. The breakpoints determine the size
of the gene cassette any therapy has to restore.

---

## 2. The design logic

The defect has a shape that is unusually favourable for treatment:

- The missing proteins are **small** (roughly 400 amino acids, about 1.2 kb of coding
  sequence each). Both fit easily into any gene delivery vector.
- They are **secreted enzymes**. A corrected cell can supply its neighbours. Complete
  correction of every cell is not required.
- The target tissue is the **outside of the body**. It can be dosed topically, watched
  directly, biopsied, and stopped. This removes most of the risk that makes gene therapy
  for internal organs dangerous.
- The disease is **not degenerative in the nervous system**. Restoring barrier function
  should restore the skin, because skin renews itself continuously.

The unfavourable part is equally clear. Epidermis sheds. Any therapy that does not reach
the basal stem cells has to be reapplied forever.

That single fact splits the plan into two tracks: **a control track** that can start within
months, and **a cure track** that targets stem cells and takes years.

---

## 3. Candidate A: bespoke topical gene therapy (the primary cure candidate)

**Working name: HSV1-LIPN/LIPK topical gel.**

### 3.1 Why this vector

Beremagene geperpavec (Vyjuvek) is an approved medicine. It is a replication-defective
herpes simplex virus type 1 engineered to carry a working copy of a gene, formulated as a
gel, and wiped onto the skin weekly. It treats dystrophic epidermolysis bullosa by
delivering collagen VII. The same platform, with a different gene, is in trials as KB105
for TGM1-deficient ichthyosis, where repeat topical dosing was well tolerated with no
immune response and restored enzyme activity in treated skin.

That is the exact precedent needed here. A topical HSV-1 skin vector delivering a missing
enzyme to ichthyotic skin already has human safety data. What is missing is the payload.

Its properties fit this case:

- **Capacity above 30 kb.** LIPN and LIPK together need under 3 kb of coding sequence.
  Both genes fit in one vector with room for full regulatory elements. Adeno-associated
  virus, capped near 4.7 kb, would be tighter and does not have topical skin precedent.
- **Non-integrating and episomal.** No insertional mutagenesis risk, which matters
  enormously in a child.
- **Transduces dividing and non-dividing cells**, including keratinocytes.
- **Topical, redosable, and stoppable.** If it does not work, you wash it off and stop.

### 3.2 Cassette design

Because capacity is not limiting, use **two independent expression units in one vector**
rather than a bicistronic construct. A self-cleaving peptide such as P2A would leave a
residual tag on a secreted enzyme, which is an unnecessary risk when there is room to
avoid it.

```
[ ITR/backbone ]--[ IVL or KRT1 promoter ]--[ LIPN CDS + native signal peptide ]--[ polyA ]
                --[ IVL or KRT1 promoter ]--[ LIPK CDS + native signal peptide ]--[ polyA ]--[ backbone ]
```

**Promoter choice is the main design decision.** Two options:

- *Differentiation-layer promoters* (involucrin, keratin 1). These switch the enzymes on
  only in the granular layer, which is where both genes are normally expressed. This is
  the physiologically correct choice and avoids lipase activity in the wrong compartment.
- *Constitutive promoters* (CMV, EF1a). Stronger and more reliable, but a secreted lipase
  expressed in basal cells could degrade lipids where they are still needed.

**Recommendation: build both, test side by side in the patient's own skin model.** The
cost of building a second construct is trivial next to the cost of guessing wrong.

Keep the **native signal peptides**. Both proteins are naturally secreted, and the native
sequence is the best-validated route to correct trafficking.

### 3.3 Honest limitation

HSV-1 vectors are episomal. Transduced cells shed within weeks. This produces
**control, not cure**: a weekly gel, for life, on the affected areas. That is exactly how
Vyjuvek is used. For a child in this condition, weekly topical treatment that restores
barrier function would still be transformative.

The durable version of this is Candidate E.

---

## 4. Candidate B: lipidomics-guided lipid replacement (the fastest path to benefit)

This is the cheapest, fastest, and most underrated idea in this document, and it can start
now.

**The insight:** nobody has ever biochemically characterised what LIPN and LIPK actually
cleave. The literature says they are epidermal lipases active in terminal differentiation
and stops there. This patient is, unfortunately, the definitive experiment.

**The protocol:**

1. Take tape strips and scale samples from his skin. This is painless and needs no biopsy.
2. Run comparative lipidomics against age-matched controls and against patients with other
   ichthyosis subtypes.
3. Two signals will appear: a lipid species that **accumulates** because nothing cleaves it,
   and a downstream product that is **absent** because it is never generated.

**Why this matters clinically.** If the missing product is a known lipid that can be
synthesised, you formulate it into an ointment and apply it directly. You are bypassing the
missing enzyme rather than replacing it. Ceramide and cholesterol mixtures already have
evidence in ichthyosis, and this would be a version tailored to his specific deficit rather
than a generic barrier cream.

**Why it is fast.** A custom compounded topical lipid is not a gene therapy. The regulatory
burden is a fraction of Candidate A. Realistic timeline is months, not years.

**Why it matters scientifically.** This experiment also defines the biomarker that every
other candidate is measured against. Without it, you cannot tell whether a gene therapy is
working except by looking at the skin. Do this first regardless of which therapy is chosen.

---

## 5. Candidate C: topical recombinant enzyme replacement

Manufacture recombinant human LIPN and LIPK protein, formulate them in a penetrating lipid
vehicle, and apply topically.

**In favour:** enzyme replacement is a mature, well-understood modality. Both proteins are
naturally secreted and extracellular, so they do not need to get inside cells. Their site of
action is the upper epidermis, which is the part closest to the surface.

**Against:** the stratum corneum blocks molecules above roughly 500 daltons, and these are
45 kilodalton proteins. Delivery is the whole problem. Mitigations worth testing include
microneedle arrays, application to already-fissured skin where the barrier is absent, and
penetration-enhancing vehicles.

**Verdict: a serious backup, not the lead.** Test it in the patient's skin model in parallel
because it is far simpler to manufacture than a viral vector. If it works, it is the safest
option in this document.

---

## 6. Candidate D: topical mRNA in lipid nanoparticles

Deliver LIPN and LIPK messenger RNA in nanoparticles, so his own keratinocytes make the
enzymes.

Engineered vectors delivered functional mRNA to keratinocytes and produced protein
throughout reconstructed epidermis after topical application in 2026 work. Ionizable
nanoparticles have achieved sustained protein restoration in patient-derived keratinocytes.

**In favour:** no virus, no DNA, no integration risk. Manufacturing is fast and the field is
moving quickly.

**Against:** stratum corneum penetration remains the acknowledged unsolved problem, and
transfection is patchy. Expression is transient, so dosing would be frequent.

**Verdict: watch, and revisit in two to three years.** Not the lead today.

**A note on why gene editing is excluded.** The newest ichthyosis work uses base editing to
correct point mutations. That approach is unavailable here. You cannot edit a gene that has
been deleted. Only gene addition works for this patient, which is why every viable candidate
above delivers a whole new copy.

---

## 7. Candidate E: ex vivo corrected epidermal stem cell grafts (the only durable cure)

This is the one approach that could produce a permanent result rather than lifelong therapy.

**The precedent is real and it worked.** In 2015 in Bochum, a boy with junctional
epidermolysis bullosa who had lost most of his skin received grafts of his own epidermal
stem cells, corrected in the laboratory with a working copy of his missing gene and grown
into sheets. Roughly eighty percent of his body surface was replaced. The corrected skin
was still functioning years later, because the therapy reached the long-lived stem cells
that regenerate the epidermis.

**Applied here:**

1. Biopsy healthy-appearing skin, isolate his keratinocyte stem cells.
2. Transduce them with a LIPN plus LIPK cassette, using an integrating vector so the
   correction is inherited by every daughter cell.
3. Expand into epidermal sheets.
4. Graft, staged over multiple surgeries, prioritising the areas causing the most harm:
   eyelids to save his corneas, hands, and the largest painful surfaces.

**The hard parts, stated plainly:**

- Integrating vectors carry insertional mutagenesis risk. This is the trade for permanence.
- Ichthyotic skin is intact, not denuded. Grafting requires removing existing skin first,
  which is major surgery and is far harder to justify than in a blistering disease where the
  skin is already gone.
- It is a multi-year program at a specialist centre with cell manufacturing capability.

**Verdict: the real cure, and the highest cost and risk.** Reasonable to stage: prove the
construct works in Candidate A first, then consider grafting for the highest-impact areas.

---

## 8. Validation plan

No candidate goes near the patient before it works in a model built from his own cells.

**Step 1. Genetics, weeks.** Whole genome sequencing. Confirm homozygosity, map exact
breakpoints, exclude LIPA and PTEN involvement, record LIPJ and LIPM status.

**Step 2. Lipidomics, one to three months.** Tape strips and scale, compared against
controls. Defines the biochemical deficit and the efficacy biomarker. Candidate B may fall
out of this step directly.

**Step 3. Patient-derived skin model, three to six months.** A single small biopsy yields
keratinocytes, which are grown into a three-dimensional organotypic skin equivalent at an
air-liquid interface. This is the workhorse of the whole program. It should reproduce his
barrier defect in a dish. Every candidate is then tested against it.

Read-outs: enzyme activity, transepidermal water loss, dye penetration, lipid profile
restoration to the Step 2 biomarker, and histology of the cornified layer.

**Step 4. Head-to-head screen, six to twelve months.** Both promoter variants of Candidate A,
plus Candidates B and C, in his own skin model. This is where the lead is chosen on data
rather than argument.

**Step 5. Animal work, twelve to eighteen months, in parallel.** Graft his corrected
keratinocytes onto immunodeficient mice to test durability and safety in living skin. A
Lipn/Lipk double knockout mouse would be informative but is a long build; the xenograft
route is faster and uses his actual cells.

**Step 6. Manufacturing and toxicology.** Good manufacturing practice production, biodistribution,
and shedding studies. Usually the rate-limiting step for a bespoke therapy.

**Step 7. Treat, under a single-patient protocol.** Start with a small test patch. Escalate
by area only after the patch is assessed.

---

## 9. Regulatory route

A therapy for one patient cannot run a randomised trial. There are now pathways built for
exactly this.

- **The FDA plausible mechanism pathway.** Draft guidance issued February 2026, designed for
  personalised N-of-1 therapies where conventional trials are impossible. Its criteria are a
  near-exact description of this case: an identified disease-causing abnormality, a therapy
  addressing the root cause, natural history data, and confirmation of target engagement.
  The comment period has closed and the pathway is the most promising route.
- **Single-patient expanded access, the traditional route.** Slower, well established.
- **European hospital exemption** for advanced therapy medicinal products prepared for a
  single patient in one member state.
- **Qatar.** Sidra Medicine opened a Gene Therapy Center for paediatric rare disease in 2025
  and has treated children from Iraq. Its existing programs are muscle and blood diseases
  rather than skin, so the realistic role is as treating and coordinating centre partnered
  with a skin gene therapy group.

**Designations worth filing early:** orphan drug and rare paediatric disease. KB105 obtained
both for a comparable ichthyosis indication.

---

## 10. Who has to be contacted

The science does not lack feasibility. It lacks a sponsor. These are the groups closest to
having the pieces already built.

| Who | What they have | Ask |
|---|---|---|
| Krystal Biotech | The approved topical HSV-1 skin platform, plus KB105, a topical gene therapy for TGM1 ichthyosis | Would they build a LIPN/LIPK payload on their existing vector |
| Northwestern University ichthyosis program (Amy Paller) | The leading clinical ichthyosis research program, running drug repurposing trials | Take the case, build the skin model |
| FIRST, Foundation for Ichthyosis and Related Skin Types | Tele-Ichthyosis, a free platform for remote consultation with world ichthyosis experts, and a physician referral service | Submit the case for expert review immediately |
| Sidra Medicine, Qatar | Gene Therapy Center, regional genomics, treats Iraqi patients | Treating centre, coordination, sequencing confirmation |
| Israeli/Bochum epidermal stem cell graft groups | The only teams that have replaced a child's epidermis with corrected stem cells | Feasibility opinion on Candidate E |

The single most valuable asset in this whole plan is the case itself. A confirmed homozygous
deletion of two epidermal lipases is a first-in-world finding that answers open questions
about what these enzymes do. That is a publication and a research program, which is exactly
the leverage needed to get a sponsor to build a therapy that has no commercial market.

---

## 11. What to do while all of this is pending

None of the above should delay treatment that works today.

- **Oral acitretin** is the most effective available medicine for lamellar-type ichthyosis
  and improves scale, ectropion, and eclabium in published series of severely affected
  children. Requires liver and lipid monitoring.
- **Intensive barrier care:** long baths, gentle mechanical descaling, thick emollients with
  urea or lactic acid, and ceramide-cholesterol preparations.
- **Ophthalmology** for the everted eyelids, to protect his corneas. This is sight-saving and
  urgent.
- **Infection control** and high-calorie nutrition, since damaged skin loses enormous energy.
- **Pain and sleep management.**

Expected benefit from this alone, within months, is substantial. It is not a cure and it does
not need to wait for one.

---

## 12. Summary

| Candidate | Mechanism | Durability | Time to patient | Risk | Verdict |
|---|---|---|---|---|---|
| A. Topical HSV-1 LIPN/LIPK gel | Delivers both genes to skin cells | Weekly, lifelong | 3 to 5 years | Moderate | **Lead** |
| B. Lipidomics-guided lipid cream | Supplies the missing lipid product | Daily, lifelong | 3 to 12 months | Low | **Start now** |
| C. Topical recombinant enzyme | Supplies the enzymes directly | Frequent | 2 to 4 years | Low | Backup |
| D. Topical mRNA nanoparticles | Cells make the enzymes transiently | Frequent | 3 to 6 years | Moderate | Revisit later |
| E. Corrected stem cell grafts | Permanently corrects skin stem cells | Permanent | 5 to 10 years | High | The actual cure |

**The honest bottom line.** A cure for this deletion does not exist and cannot be conjured.
But every component needed to build one already exists and is already approved in humans for
a different gene: a topical skin gene therapy platform, a proven precedent for replacing a
child's epidermis with corrected stem cells, and a regulatory pathway written for
single-patient therapies. Nobody has assembled them for this gene because until now there
was no patient. The blocker is not science. It is finding an institution willing to build
it, and that begins with the three verification questions in section 1.1 and one submission
to an expert review platform.
