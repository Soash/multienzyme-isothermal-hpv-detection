# Multienzyme Isothermal Rapid Amplification-coupled Lateral Flow Assay (MIRA-LFD) for Point-of-Care High-Risk HPV Detection

**Author:** Md Abu Sadat Soash  
**Supervisor:** Prof. Dr. Gokul Chandra Biswas  
*Department of Genetic Engineering and Biotechnology, Shahjalal University of Science and Technology, Sylhet-3114, Bangladesh*

[![Status: Unpublished Research](https://img.shields.io/badge/Status-Unpublished%20Research-orange.svg)](#confidentiality--publication-notice)
[![Platform: MIRA--LFD](https://img.shields.io/badge/Platform-MIRA--LFD-blue.svg)](#assay-architecture--principle)
[![Targets: HPV--16%20%7C%20HPV--18](https://img.shields.io/badge/Targets-HPV--16%20%7C%20HPV--18-brightgreen.svg)](#assay-architecture--principle)

---

## Abstract

Cervical cancer is a leading cause of cancer death among women around the globe. HPV vaccination has not been properly introduced yet. Screening of cervical cancer incidences still relies on visual inspection with acetic acid. HPV DNA testing, recommended by the World Health Organization, remains unimplemented in developing country like Bangladesh. Quantitative PCR used in HPV DNA testing requires thermal cyclers, stable electricity, cold-chain reagents, and trained personnel. To mitigate these challenges, this study aimed to develop an equipment-free assay for the simultaneous detection of the E6 oncogene of HPV-16 and HPV-18, thereby confirming the incidence of cervical cancer-associated. 

The test or diagnosis combines the Multienzyme Isothermal Rapid Amplification (MIRA) of target biomarker with a duplex lateral flow dipstick (LFD). Genotype-specific primers and internal NFO probes were designed against synthetic E6 fragments. An initial design placed fluorescein and hapten labels directly on the primers. This produced false positives outcomes in no-template controls, caused by dual-labelled primer-dimers. The assay was redesigned around an unlabeled forward primer and an internal FAM-labelled NFO probe. Thus, false-positive results were eliminated in negative controls. 

Band intensities were quantified by image analysis across reaction temperature, incubation time, and template copy numbers. At 37 °C, which resembles body temperature, both genotypes were detected within 30 min at copy number of 1 copy/µL. However, the results are inconsistent due to Poisson Distribution effect, whereas 10 copies/µL shows intense and steady band. Interestingly at 30 °C (ambient temperature), detection were positive by visual bands; however, they were faint band on both test lines. These were too marginal for confident visual interpretation. The HPV-18 signal rose early and then plateaued. The HPV-16 signal remained low until 20 min and then rose steeply. Raising the template from 10 to 100 copies/µL increased the HPV-18 signal and slightly compromised the HPV-16 signal, indicating competition for shared reaction components. 

The platform detects both genotypes at 10 copies/µL within 30 min at body temperature without requiring a thermal cycler, power supply, and or readout instrument. It is therefore suited to cervical cancer diagnosis in clinics and community settings where laboratory infrastructure is absent. With further optimization and thorough clinical validation, the MIRA-LFD assay system has the potential to become a promising point-of-care testing platform.

---

## Assay Architecture & Principle

```
                        [ Target DNA (E6) ]
                                 │
           ┌─────────────────────┴─────────────────────┐
           ▼                                           ▼
[ Recombinase-Assisted Annealing ]             [ Probe Cleavage (Endo IV) ]
           │                                           │
           ▼                                           ▼
[ Strand-Displacing Polymerase ]               [ Dual-Label Amplicon Formed ]
           │                                           │
           └─────────────────────┬─────────────────────┘
                                 │
                                 ▼
              [ Lateral Flow Dipstick Detection (LFD) ]
              ├── Test Line 1 (T1): HPV-16 (Biotin-Streptavidin)
              ├── Test Line 2 (T2): HPV-18 (DIG-Anti-DIG)
              └── Control Line (C): Quality / Flow Verification
```

### 1. Isothermal Enzymatic Amplification (MIRA)
MIRA utilizes a three-enzyme cascade operating at near-physiological temperatures (37 °C–42 °C). A recombinase–primer nucleoprotein filament mediates strand invasion without thermal denaturation, single-stranded binding proteins (SSBs) stabilize the open displacement loop, and a strand-displacing DNA polymerase drives rapid, exponential target amplification.

<p align="center">
  <img src="results/1.3.jpg" alt="MIRA Principle" width="550" />
  <br>
  <em>Figure 1: Mechanism of Multienzyme Isothermal Rapid Amplification (MIRA).</em>
</p>

### 2. Duplex Lateral Flow Detection (LFD)
The amplification product is introduced to a paper-based lateral flow dipstick. Conjugated anti-FAM gold nanoparticles migrate across the membrane via capillary force. To prevent dual-labeled primer-dimers from yielding non-template false positives, the assay employs an internal NFO probe cleaved sequence-specifically by Endonuclease IV, ensuring that dual-label capture occurs strictly in the presence of bona fide target amplicons.

| Component | Function / Capture Target |
|:---|:---|
| **Conjugate Pad** | Anti-FAM colloidal gold nanoparticles (AuNPs) |
| **Test Line 1 (T1)** | Immobilized Streptavidin (captures Biotin-labeled HPV-16 amplicon) |
| **Test Line 2 (T2)** | Immobilized Anti-DIG antibody (captures Digoxigenin-labeled HPV-18 amplicon) |
| **Control Line (C)** | Quality control capture verifying uniform capillary migration |

<p align="center">
  <img src="results/1.4.png" alt="Lateral Flow Device" width="600" />
  <br>
  <em>Figure 2: Lateral flow assay architecture.</em>
</p>

<p align="center">
  <img src="results/1.5.png" alt="Dual-Label Detection Mechanism" width="550" />
  <br>
  <em>Figure 3: Probe-mediated dual-label lateral flow strip mechanism.</em>
</p>

---

## Study Workflow

The complete analytical and experimental progression follows a multi-phase validation pipeline:

<p align="center">
  <img src="results/2.1.png" alt="Workflow" width="550" />
  <br>
  <em>Figure 4: Schematic representation of the study workflow.</em>
</p>

1. **Target Selection & In Silico Design:** Conserved diagnostic regions within the HPV-16 and HPV-18 E6 oncogenes were mapped, modeled, and selected to avoid target-target dimerization.
2. **Architecture Optimization:** Transition from direct primer labeling to an internal probe-mediated format to suppress non-specific background signals.
3. **Parametric Optimization:** Systematically evaluated reaction temperatures (ambient ~30 °C, physiological ~37 °C, and reference ~42 °C) and reaction times (10 to 30 min).
4. **Analytical Sensitivity & Competition Profiling:** Evaluated limit of detection and duplex channel dynamics across template copy numbers.

---

## Experimental Highlights

### 1. Elimination of Primer-Dimer Artefacts
Initial direct 5'-end primer dual-labeling resulted in spurious false-positive bands on negative controls (NTC) due to inter-primer hybridization. Redesigning the reaction around an internal nfo-probe architecture completely abolished false-positive test lines while maintaining robust positive control responses.

<p align="center">
  <img src="results/3.1.png" alt="Elimination of Primer-Dimer Artefact" width="460" />
  <br>
  <em>Figure 5: Probe-mediated suppression of primer-dimer false positives in negative controls.</em>
</p>

### 2. Operational Temperature Tolerance
- **37 °C (Body Temperature):** Generates clear, visually discernible test bands for both HPV-16 and HPV-18 within 30 minutes, confirming that body-heat incubation is viable for equipment-free deployment.
- **30 °C (Ambient Condition):** Detectable yet marginal visual bands, demonstrating enzymatic activity at room temperature, though physiological warming is recommended for robust field scoring.
- **42 °C (Reference Condition):** Serves as an upper reference benchmark confirming maximum enzymatic yield.

<p align="center">
  <img src="results/3.2.png" alt="Temperature Optimization" width="520" />
  <br>
  <em>Figure 6: Influence of reaction temperature on duplex MIRA-LFD performance.</em>
</p>

### 3. Incubation Kinetics & Duplex Dynamics
- Target line development begins within 10 minutes, reaching optimal signal differentiation and balance at **30 minutes**.
- Competitive kinetics between HPV-16 and HPV-18 amplification channels reveal shared enzyme pool utilization during late exponential phases.

| Incubation Time | Analytical Sensitivity |
|:---:|:---:|
| <img src="results/3.3.png" alt="Incubation Time" width="380" /> | <img src="results/3.4.png" alt="Sensitivity" width="380" /> |
| *Figure 7: Time-dependent line development (10–30 min).* | *Figure 8: Analytical sensitivity across copy number inputs.* |

---

## Repository Structure

```text
multienzyme-isothermal-hpv-detection/
├── results/                     # Experimental figures and schematic diagrams
│   ├── 1.3.jpg                  # MIRA isothermal amplification principle
│   ├── 1.4.png                  # LFD device structure schematic
│   ├── 1.5.png                  # Probe-mediated dual-label mechanism
│   ├── 2.1.png                  # Experimental workflow
│   ├── 3.1.png                  # Primer-dimer elimination validation
│   ├── 3.2.png                  # Reaction temperature characterization
│   ├── 3.3.png                  # Incubation time series
│   └── 3.4.png                  # Analytical sensitivity and copy number analysis
├── Thesis_Revision_Final.docx   # Master thesis document
├── .gitignore                   # Git configuration
└── README.md                    # Project documentation
```

---

## Confidentiality & Publication Notice

This research contains original, currently **unpublished experimental findings and methodology**.
- All data, figures, and technical descriptions are for evaluation, review, and archival purposes within this repository.
- **Do not reproduce, distribute, or publicly cite** without explicit written authorization from the authors and research supervisors.
- For academic collaboration or inquiry regarding the manuscript and dataset, please contact the corresponding laboratory:

**Department of Genetic Engineering and Biotechnology**  
Shahjalal University of Science and Technology, Sylhet, Bangladesh


