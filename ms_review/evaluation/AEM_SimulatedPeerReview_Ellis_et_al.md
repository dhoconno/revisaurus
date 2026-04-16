# Simulated Peer Review — Applied and Environmental Microbiology

**Manuscript:** AEM-2025-XXXXX  
**Title:** Adaptation of the multiplexed CRISPR-Cas13 CARMEN RVP assay for longitudinal detection of respiratory pathogens from air samples  
**Authors:** Ellis AL, Stauss M, Barros Tiburcio P, Emmen IE, Edlefsen PT, Kosmider E, Barlow S, Goss M, Temte JL, Stachler E, McMahon K, Sabeti P, O'Connor DH, O'Connor SL  
**Journal:** Applied and Environmental Microbiology (ASM)  
**Date of Review:** April 2026  

---

# PART I: EDITORIAL DECISION LETTER

Dear Dr. O'Connor and colleagues,

**Re: AEM-2025-XXXXX — "Adaptation of the multiplexed CRISPR-Cas13 CARMEN RVP assay for longitudinal detection of respiratory pathogens from air samples"**

Thank you for submitting your manuscript to *Applied and Environmental Microbiology*. Your paper describes the optimization of the CRISPR-Cas13-based CARMEN RVP assay for detecting respiratory pathogens from air samples collected in K-12 schools, and compares the assay's performance against qRT-PCR and clinical nasal swab data from the ORCHARDS program.

I am writing to inform you that the decision on your manuscript is **Major Revision**. All four reviewers agree that the topic — adapting multiplexed CRISPR-based diagnostics for environmental air surveillance — is timely and relevant to AEM's readership. The iterative optimization approach (crRNA redesign, inhibitor removal, new influenza targets) is a strength, and the comparison with concurrent clinical surveillance data from ORCHARDS is a valuable feature. However, the reviewers have identified several significant concerns that must be addressed before the manuscript can be considered for publication.

## Editorial Assessment

The manuscript addresses a genuinely important gap: translating a high-throughput multiplexed diagnostic platform from clinical specimens to the more challenging air sample matrix. The iterative, problem-solving approach is well-documented and transparent — the authors do not hide the fact that the original CARMEN RVP performed very poorly on air samples. This honesty is commendable. However, the reviewers have converged on several critical issues that weaken the current manuscript:

1. **The concordance between CARMEN RVP (RVP_air) and qRT-PCR remains low-to-moderate at best.** Kappa scores for SARS-CoV-2 range from 0.104 to 0.372, and for influenza A are largely non-significant. All four reviewers raised this concern. The manuscript frames this as a work-in-progress, but the gap between the assay's current sensitivity and what is needed for reliable surveillance must be discussed more rigorously.

2. **The analytical validation of the assay is incomplete.** Three reviewers noted the absence of a formal limit of detection (LOD) characterization, cross-reactivity panels with near-neighbor pathogens, and inadequate reporting of assay performance metrics. These are standard requirements for any assay development paper.

3. **Critical air sampling metadata is missing.** Reviewer 1 (bioaerosol expert) emphasized that air volume sampled, sampler flow rate, and environmental conditions are not reported — making it impossible to normalize results or compare across settings.

4. **Statistical concerns.** Reviewer 3 (methods/statistics) identified issues with multiple testing correction, the presentation of kappa scores without confidence intervals, and the need for more formal quantitative comparisons between assays.

Areas of disagreement among reviewers: Reviewer 4 (CRISPR diagnostics) was somewhat more generous toward the sensitivity limitations, arguing that surveillance applications can tolerate lower per-sample sensitivity if population trends are preserved. I find this a fair point, but the manuscript must make this argument explicitly if it is to be persuasive. Reviewer 1 expressed concern that without air volume normalization, the data cannot be meaningfully interpreted; I consider this essential for revision.

## Key Issues to Address

### Essential Changes (must address for acceptance)

1. **Report air sampling metadata.** Total air volume sampled per cartridge (flow rate × sampling duration), sampler model specifications, and environmental conditions (room size or type where known) must be provided for all sampling events. Without this information, no cross-study comparisons are possible and the results are of limited utility to others in the field. (Reviewers 1, 2)

2. **Characterize the formal limit of detection.** Perform serial dilutions of target RNA in the relevant matrix (extracted air sample RNA, ideally spiked into a representative negative air sample background) and determine the LOD with replicate testing (e.g., probit analysis or hit-rate at each dilution). This must be done for at least SARS-CoV-2 and influenza A for both the qRT-PCR and RVP_air assays. (Reviewers 3, 4)

3. **Report kappa scores with 95% confidence intervals**, not just point estimates. Provide the full 2×2 contingency tables for all comparisons in the main text or supplementary materials, not just selected metrics. Discuss the implications of the low kappa values honestly. (Reviewer 3)

4. **Address multiple testing.** The manuscript acknowledges this issue but does not apply any correction. Given the number of comparisons presented, at minimum apply Benjamini-Hochberg FDR correction to the full set of p-values and present both adjusted and unadjusted values. (Reviewer 3)

5. **Provide a transparent cost analysis.** The $10–20/sample figure requires a breakdown: reagents, equipment amortization, labor, and throughput must be specified. Compare this directly with the qRT-PCR cost per sample. (Reviewers 1, 4)

6. **Discuss the practical implications of 58.8% sensitivity for SARS-CoV-2 and 7.7% for Flu A.** These are the key performance metrics for the assay, and they must be contextualized for the reader. Under what surveillance scenarios is this level of sensitivity acceptable? When is it not? This discussion is currently absent. (All reviewers)

### Strongly Recommended Changes

7. **Include field blank controls.** Were any air samplers deployed in unoccupied spaces as negative field controls? If so, report the results. If not, acknowledge this limitation and describe plans for future studies. (Reviewer 1)

8. **Show individual Ct values.** Scatter plots of Ct values for samples that are concordant vs. discordant between qRT-PCR and RVP_air would help the reader understand the sensitivity threshold at which RVP_air fails to detect positives. (Reviewers 3, 4)

9. **Update the crRNA conservation analysis.** The authors designed crRNAs against reference sequences from 2021-2022. Verify that these crRNAs match currently circulating strains (2024-2025 variants) and report the analysis. This is especially important for SARS-CoV-2, where the N gene has accumulated mutations. (Reviewers 2, 4)

10. **Clarify the substrate protocol change.** The shift from one substrate to two substrates in February 2024 could confound temporal analyses. Show whether detection rates changed around this time point, or analyze the two periods separately. (Reviewer 1)

11. **Improve figures.** Figures 3C and 4C should include confidence bands or error bars on the percentage estimates. The heatmaps would benefit from annotation of total sample numbers per time bin. (Reviewer 3)

### Suggestions (not required)

- While Reviewer 2 suggests performing sequencing on RVP_air-positive samples to confirm pathogen identity, I do not consider this essential for the current manuscript, though it would strengthen a future study.
- Reviewer 1 suggests viability testing of detected pathogens. This is beyond the scope of an assay development paper, and the authors should simply ensure they do not overstate transmission risk implications.

## Closing

Please submit your revised manuscript within **90 days**. The revised manuscript will undergo re-review by the original reviewers. Please provide a detailed point-by-point response to each reviewer comment, indicating the changes made and the page/line numbers of revisions. New or revised data should be clearly identified.

Sincerely,

*Handling Editor*  
*Applied and Environmental Microbiology*

---
---

# PART II: INDIVIDUAL REVIEWER REPORTS

---

## Reviewer 1: Bioaerosol Pathogen Detection & Air Sampling

### Summary

This paper describes the adaptation of the CRISPR-Cas13-based CARMEN RVP multiplexed assay for detecting respiratory pathogens in air samples from K-12 schools. The authors iteratively optimized the assay (adding a SARS-CoV-2 N gene target, removing PCR inhibitors, redesigning influenza crRNAs) and compared the optimized "RVP_air" and "RVP_air_flu" assays to qRT-PCR on longitudinal air samples from 15 schools in Dane County, Wisconsin, during the 2023-2024 school year. A subset of results was further compared to clinical nasal swab data from the ORCHARDS study.

### General Assessment

The study addresses a real need in environmental surveillance: cost-effective, multiplexed pathogen detection from air samples. The AerosolSense platform is widely used and the adaptation of CARMEN RVP to this sample type is of practical interest. The iterative approach to overcoming challenges (low biomass, inhibitors, suboptimal crRNA targets) is well-documented. However, the manuscript has significant gaps in reporting air sampling metadata that limit interpretability and reproducibility, which are critical for a paper in *Applied and Environmental Microbiology*. The assay's sensitivity, particularly for influenza A, remains a concern.

### Major Concerns

**1. Air volume not reported.** This is the single most important omission in the manuscript. The AerosolSense sampler operates at approximately 200 L/min, and cartridges were deployed for 3-7 days continuously. This means each cartridge sampled on the order of 860,000 to 2,000,000 liters of air, yet the total air volume is never stated. The paper reports positivity per "cartridge" without normalizing to air volume. While this may be acceptable for within-study comparisons (all samplers are the same type), it is essential metadata for cross-study comparison and for readers evaluating whether the sampling strategy was adequate. The authors must report the flow rate, sampling duration per cartridge, and total air volume sampled for each collection event. This information should be provided in a supplementary table.

**2. Absence of field blank controls.** The methods describe no-template controls and extraction blanks for the molecular assays, which is good. However, there is no mention of field blanks — cartridges deployed in the samplers but in unoccupied or known-clean spaces. Without field blanks, it is impossible to exclude the possibility that some low-level positives (particularly the ubiquitous SARS-CoV-2 signal) are due to contamination during cartridge handling, transport, or processing. The storage room control mentioned in reference 5 (Bobrovska et al.) serves this purpose, but it is absent here. At minimum, the authors should acknowledge this limitation and discuss whether any control deployments were performed.

**3. No characterization of recovery efficiency.** The paper uses a PCR inhibitor removal kit (Zymo OneStep) and demonstrates improved detection after cleaning, but no spike-and-recovery experiment is described. What fraction of target RNA is lost during the inhibitor removal step? What is the overall recovery from the AerosolSense cartridge substrate through elution, RNA extraction, and inhibitor removal? Even a rough estimate would help contextualize the sensitivity data. The finding that only 58.8% of qRT-PCR SARS-CoV-2 positives are detected by RVP_air could partly reflect RNA losses during the additional cleanup step.

**4. Protocol change confound.** The RNA extraction protocol changed in February 2024 from one substrate to two substrates per cartridge. This effectively doubled the input material for subsequent samples. The temporal analyses in Figures 2-4 span this transition. The authors should demonstrate that this protocol change did not systematically bias detection rates by comparing positivity rates before and after the change, or by analyzing the two time periods separately. At minimum, this must be noted as a potential confound.

**5. Sampler placement and environmental context.** The paper states that samplers were in "high-traffic areas" of 15 schools, but provides no further detail. The location within a school (cafeteria, hallway, classroom, nurse's office) significantly affects what is captured. Were all samplers in comparable locations? Was the sampler inlet height the same across schools? Were any rooms mechanically ventilated vs. naturally ventilated? These variables affect pathogen concentration in air and should be described, even if briefly.

### Minor Concerns

1. The Importance section claims "cost-effective alternative to individual testing" but the cost comparison is not rigorously presented. The $10-20/sample estimate is mentioned once in the introduction. What does this include? How does it compare to the qRT-PCR assay cost per sample, including labor?

2. The term "low biomass" is used several times but never quantified. What are typical RNA yields from air sample cartridges? Reporting nanograms of total RNA per cartridge or RNAseP Ct values across the dataset would help readers understand the challenge.

3. Figure 1D: The heatmap labels for "uncleaned" appear twice in the figure legend description ("uncleaned (top heat map) and uncleaned (bottom heat map)") — this appears to be a typo; the second should be "cleaned."

4. Were the 15 schools all in the same school district, or from multiple districts? The seven schools used for RVP_air testing are described as being from the Oregon school district, but the relationship to the other eight schools is unclear.

5. The sampling period of 3-7 days is quite variable. Was any analysis performed to determine whether longer sampling periods improved or reduced detection sensitivity (e.g., due to RNA degradation on the cartridge)?

### Recommendation to Editor (Confidential)

**Major Revision.** The scientific question is relevant and the approach has merit, but the missing air sampling metadata and absence of field controls are significant deficiencies for a paper in AEM. The recovery efficiency characterization is also important. I believe these issues can be addressed in revision. The assay's moderate sensitivity is a limitation but is honestly acknowledged, and the comparison to ORCHARDS data adds value. With the requested improvements, this could be a solid contribution to the environmental surveillance literature.

---

## Reviewer 2: Viral Genomics & Molecular Epidemiology

### Summary

Ellis et al. describe the optimization of the CARMEN RVP CRISPR-Cas13 multiplexed assay for application to air samples collected from K-12 schools, with comparison to qRT-PCR and clinical nasal swab surveillance data. Key modifications include the addition of a SARS-CoV-2 nucleocapsid target, removal of PCR inhibitors from extracted air RNA, and design of new influenza A M-gene crRNAs. The authors report improved but still imperfect concordance with qRT-PCR, and demonstrate that temporal patterns of pathogen detection in air mirror clinical detections.

### General Assessment

This is a well-framed methods development paper that addresses a genuine challenge in environmental surveillance — the need for affordable, multiplexed pathogen detection from low-biomass environmental samples. The work is relevant to AEM's scope and the integration with the ORCHARDS clinical surveillance program is a significant strength that many air sampling studies lack. However, the paper would benefit from more rigorous assay validation and a more forthright discussion of when the RVP_air assay's sensitivity is and is not adequate.

### Major Concerns

**1. crRNA conservation and future-proofing.** The crRNAs for SARS-CoV-2 and influenza were designed using reference sequences from 2020-2022. SARS-CoV-2 has evolved considerably since then, with mutations accumulating across the genome including the N gene. The authors should perform an in silico analysis of crRNA binding site conservation against currently circulating lineages (XEC, LP.8.1, and derivatives as of 2025) and report the results. If mismatches are found, this limits the assay's long-term utility and should be discussed. Similarly, the influenza M gene crRNAs should be checked against 2023-2024 and 2024-2025 circulating strains. The ADAPT tool used for design can presumably facilitate this analysis.

**2. No genomic confirmation of detections.** The CARMEN RVP assay detects pathogens based on crRNA-guided fluorescence, but there is no independent confirmation that positive signals represent the expected pathogen. For clinical samples, this is less of a concern because the prior probability of respiratory virus presence is high. For environmental air samples, the risk of non-specific signal or artifact is greater. Were any RVP_air-positive samples subjected to confirmatory testing by an orthogonal method (e.g., sequencing, alternate qRT-PCR target)? If not, this should be acknowledged as a limitation.

**3. Timeliness and epidemiological insight.** The data are from the 2023-2024 respiratory season. While the methods development aspect is still relevant, the surveillance data are now over a year old. The paper should make clear that the primary contribution is methodological, not epidemiological. The surveillance findings (SARS-CoV-2 detected year-round, Flu A seasonal) are confirmatory of well-established patterns and should be framed as validation rather than novel insight.

**4. Incomplete comparison with ORCHARDS.** The comparison with nasal swab data is interesting but limited by the different assay panels, different sampling populations (all students vs. only symptomatic volunteers), and the ecological nature of the comparison (school-level, not individual-level). The paper discusses some of these limitations, but the interpretation of the lag/lead analysis should be more cautious. With a significance threshold of p ≤ 0.05 and multiple pathogens tested across multiple time shifts (-3 to +3), some significant correlations are expected by chance. The authors acknowledge this but do not adjust for it.

### Minor Concerns

1. The paper does not mention data deposition. Are the qRT-PCR Ct values and RVP_air fluorescence data deposited in a public repository? For an assay methods paper, making the raw data available would greatly enhance reproducibility and allow others to apply alternative analysis approaches.

2. Table 7 lists the pathogens used for comparative analysis, but HCoV-HKU1 is absent from the comparison despite being detected in air. Why was it excluded?

3. The ORCHARDS program detects rhinovirus/enterovirus and adenovirus, which are among the most common respiratory pathogens in children. These are not in the RVP_air panel. Discussing whether the CARMEN platform could be expanded to include these targets would be useful.

4. Reference 5 (Bobrovska et al., 2025) is cited as published in *Science of the Total Environment*, but this study appears to be from some of the same collaborators. The relationship and any overlapping samples should be clarified.

5. The discussion of air sampling vs. wastewater surveillance (page 16) is too general and could be shortened. The comparison would be more impactful if supported by data from concurrent wastewater surveillance in Dane County, if available.

### Recommendation to Editor (Confidential)

**Major Revision.** The core contribution — adapting CARMEN RVP for air samples — is sound and relevant. The crRNA conservation analysis and formal assay validation metrics are the key gaps. The ORCHARDS comparison is a valuable feature but needs more cautious interpretation. I support publication after revision.

---

## Reviewer 3: Methods, Statistics & Bioinformatics

### Summary

This manuscript describes the optimization and application of a CRISPR-Cas13-based multiplexed detection assay (CARMEN RVP) for respiratory pathogen surveillance from air samples collected in schools. The paper compares assay performance against qRT-PCR using kappa concordance and Spearman correlation, and further compares air sample detections to clinical nasal swab data.

### General Assessment

The manuscript describes a technically interesting assay adaptation with reasonable potential for the field of environmental surveillance. However, there are substantial concerns regarding the statistical analysis, the completeness of the assay validation, and the clarity of the data presentation. The conclusions frequently overstate what the data support, particularly regarding the practical utility of the assay in its current form. The statistical methods need revision in several areas.

### Major Concerns

**1. Limit of detection not characterized.** This is a fundamental gap for any assay development paper. The authors compare RVP_air to qRT-PCR by testing the same samples, but they never determine the analytical LOD of either assay in the air sample matrix. Without knowing the LOD, the reader cannot distinguish between (a) the sample truly contains less target than RVP_air can detect, and (b) the sample contains enough target but some other factor (inhibition, competitive amplification) causes failure. A dilution series of known-positive material (synthetic RNA or viral RNA spiked into negative air sample extract) processed through both assays would clarify this. Probit analysis should be used to determine the 95% LOD.

**2. Kappa scores lack confidence intervals.** Throughout the paper, kappa scores are reported as point estimates without confidence intervals. For many of the comparisons, the sample sizes are small (e.g., only 2 concordant Flu A positives), meaning the confidence intervals would be extremely wide and would include zero. This must be reported honestly. The permutation test p-values help, but they do not replace confidence intervals for communicating the precision of the estimate. I recommend using the bootstrapped 95% CI for kappa.

**3. Multiple testing.** The authors commendably acknowledge the issue of multiple testing (page 28-29) and provide unadjusted p-values. However, given the number of statistical tests performed (multiple kappa scores, multiple Spearman correlations, multiple Ct thresholds, multiple target combinations, lag/lead analyses at 7 time shifts for 7 pathogens), the risk of false-positive findings is substantial. At minimum, the Benjamini-Hochberg procedure should be applied to the full set of p-values, and adjusted p-values should be reported alongside unadjusted values. Several of the borderline significant results (e.g., Flu A Spearman r=0.283, p=0.031; SARS-CoV-2 lag ts=2, r=0.280, p=0.036) would likely not survive correction.

**4. Positivity threshold analysis is ad hoc.** The paper tests multiple Ct cutoffs (35, 40) and multiple positivity criteria (both replicates positive, at least one replicate positive) and reports the combination that gives the best concordance. This is a form of optimistic bias. The authors should pre-specify the primary analysis (one threshold, one positivity criterion) and present all others as secondary/sensitivity analyses, clearly labeled as such. Alternatively, a receiver operating characteristic (ROC) curve or equivalent analysis exploring the full range of thresholds would be more informative.

**5. Bar/heatmap presentation obscures individual variation.** The primary data presentation is percentage of positive cartridges per time bin, shown as heatmaps. Individual sample-level data (Ct values, fluorescence intensities) are never shown. For an assay comparison paper, scatter plots of matched Ct values vs. RVP_air fluorescence for each sample would be far more informative. This would allow the reader to see where concordance breaks down (e.g., at what Ct threshold does RVP_air fail?). At minimum, this should be in supplementary materials.

**6. Spearman correlation on percentage data may be misleading.** The Spearman correlations in Figures 3C and 4C are computed on weekly percentage positivity from a small number of schools (5-7 per time bin). With few schools, the percentage is highly discrete (0%, 14%, 29%, 43%...), which can inflate correlation coefficients. The authors should report the number of time bins used in each correlation and consider whether the correlation is driven by a few extreme points (peak season vs. off-season). A sensitivity analysis excluding the peak and/or off-season time bins would help.

### Minor Concerns

1. Figure 1 panel labels: The legend for Figure 1D contains a typo — "uncleaned (top heat map) and uncleaned (bottom heat map)" should read "uncleaned (top) and cleaned (bottom)."

2. The exclusion of inconclusive samples (where one of two replicates is positive) is reasonable but should be reported more systematically. How many inconclusive results were there for each assay and target? Were the proportions different between RVP_air and qRT-PCR?

3. The paper states that positivity for CARMEN RVP requires average fluorescence "1.8 times higher than the fluorescence of non-template controls." How was this threshold determined? Was any formal threshold optimization performed (e.g., using ROC analysis on a training set)?

4. The moving average smoothing applied in the ORCHARDS comparison (average over three time bins) is reasonable but the window size should be justified. Different window sizes should be tested in sensitivity analysis.

5. Python version and package versions are commendably reported. Are the analysis scripts available in a public repository? If not, they should be deposited.

6. Error bars or confidence bands are absent from Figures 3C, 4C, and 5B. Given that the percentages are computed from small numbers of schools, uncertainty is high and should be displayed.

### Technical Notes

- Page 4: "98 were also positive for human control RNAseP via CARMEN RVP" — this means 9 of 107 samples lacked detectable human RNA. Were these 9 samples also negative for all pathogens? If so, they may represent sampling failures and should be discussed.
- Page 8: The statement "all correlations being significant" for SARS-CoV-2 should specify the number of tests this refers to.
- Page 26: The averaging of N1 and N2 Ct values for SARS-CoV-2 positivity is unconventional. Most laboratories require both targets to be positive, or use the lower Ct value. Averaging could mask discordant results between N1 and N2. Justify this choice.
- Supplementary Table 2 is referenced multiple times but the content is only partially described. Ensure all p-values, kappa scores, and correlation coefficients are included with appropriate precision.

### Recommendation to Editor (Confidential)

**Major Revision.** The statistical issues are fixable but require substantial effort. The LOD characterization is the most important addition. If the authors address the statistical concerns and the LOD, the paper could be a useful contribution. However, if the formal LOD reveals that RVP_air is substantially less sensitive than qRT-PCR in the air sample matrix, the authors will need to recalibrate their conclusions accordingly.

---

## Reviewer 4: CRISPR-Based Diagnostics & Molecular Assay Development

### Summary

This paper describes the adaptation of the CARMEN RVP multiplexed CRISPR-Cas13 detection platform — originally designed for clinical nasal swabs — for use with air samples from K-12 schools. Modifications include adding a SARS-CoV-2 nucleocapsid crRNA target, incorporating a PCR inhibitor removal step, optimizing primer concentrations and PCR cycling, and designing new influenza A M-gene crRNAs. The optimized assay (RVP_air) detected SARS-CoV-2, seasonal coronaviruses, RSV, and influenza from school air samples over one academic year.

### General Assessment

This is a practical and well-motivated methods paper. Translating the CARMEN RVP platform from clinical to environmental samples is non-trivial, and the paper documents the iterative troubleshooting required in a transparent and instructive manner. The key insight — that PCR inhibitor removal dramatically improves multiplex CRISPR-based detection from air — is valuable for the broader community working with environmental samples. The paper is appropriate for AEM.

That said, the assay validation is incomplete by the standards expected for a methods paper in this journal. Several specific concerns follow.

### Major Concerns

**1. No formal LOD determination.** The absence of a formal limit of detection is the most significant gap. The authors compare RVP_air to qRT-PCR on field samples, but without knowing each assay's LOD in the air sample matrix, the reader cannot interpret the discordant results. Is RVP_air missing positives because the targets are below its LOD? Or because of competitive inhibition in the multiplex reaction? Or because of crRNA mismatch with circulating strains? A dilution series of synthetic RNA or inactivated virus processed through the complete air sample workflow (spiked into eluted cartridge buffer → extraction → inhibitor removal → CARMEN RVP) would distinguish among these possibilities. This is a standard expectation for assay development papers.

**2. Competitive inhibition in the multiplex reaction.** The paper acknowledges that competitive inhibition between targets is a known challenge for multiplex PCR (references 25-27) and may contribute to lower sensitivity. However, no experiment directly addresses this. A simple comparison — testing a subset of samples with the SARS-CoV-2 or Flu A primers/crRNAs in a singleplex reaction vs. the full RVP_air multiplex — would quantify the sensitivity loss attributable to multiplexing. This would help distinguish between the effects of low template, inhibitors, and competitive amplification.

**3. The 1.8× NTC fluorescence threshold is not validated.** The positivity threshold for the CARMEN assay is defined as average relative fluorescence intensity 1.8 times higher than the NTC. This is described as a manual validation step applied after the CARMEN-RVP software identifies initial positive hits. How was the 1.8× multiplier determined? Was it optimized on a training set and validated on a test set, or applied uniformly? If the threshold were lowered to 1.5×, would more positives be captured (at the cost of specificity)? A threshold optimization analysis would strengthen confidence in the binary classification.

**4. Concordance for influenza A is inadequate and should be discussed more forthrightly.** Of 26 qRT-PCR influenza A positives, only 2 were detected by RVP_air (7.7%). Even after the RVP_air_flu improvements, only 2 of 13 qRT-PCR positives in the subset tested were concordant. The paper attributes this to the crRNA targeting the wrong gene segment (PB1 for H3N2 when H1N1 was circulating), which is a reasonable explanation for the initial RVP_air panel. However, even the improved M-gene crRNAs in RVP_air_flu showed poor concordance. The discussion should address whether the fundamental sensitivity of Cas13-based detection is sufficient for the low viral loads expected in air samples, or whether this particular application pushes the technology beyond its current performance envelope.

**5. Cost analysis is incomplete.** The stated $10-20/sample is a significant selling point but requires substantiation. This should include: (a) consumable costs per sample (RT-PCR reagents, 192.24 array cost amortized per sample, crRNA synthesis, inhibitor removal kit), (b) equipment requirements (Biomark X platform, thermocycler, RNA extraction instrument), (c) labor time per run, (d) batch size required to achieve the stated cost. For comparison, a single-target qRT-PCR costs approximately $3-8/sample in reagents alone. A multiplex qRT-PCR panel on the BioFire platform is approximately $20-30/sample. The CARMEN platform's value proposition must be clearly positioned against these alternatives.

### Minor Concerns

1. The crRNA for H3N2 (targeting M gene nt 453-547) had 8 mismatches relative to H1N1 and correctly showed subtype specificity. However, the "pan_FluA" crRNA (targeting M gene nt 101-189) had only 1 mismatch relative to H3N2 and detected both subtypes. This is a useful observation about Cas13 mismatch tolerance, but the authors should explicitly state the mismatch tolerance range (1 mismatch tolerated, 8 mismatches not) and cite relevant literature on Cas13 mismatch sensitivity.

2. The paper uses in vitro transcribed RNA and inactivated virus stocks as positive controls. Were these quantified by an independent method (e.g., digital PCR) to ensure accurate copy number inputs? This is important for interpreting the LOD data if it is added in revision.

3. The modified CARMEN RVP increased PCR cycles from 40 to 50. This substantial increase in amplification raises concerns about non-specific amplification and increased false-positive rates. Were false positives observed in negative controls at 50 cycles? Was 50 cycles chosen based on systematic optimization or empirically?

4. The sample sizes for some comparisons are quite small. For the inhibitor removal experiment (Figure 1D), only 33 samples were tested. For the RVP_air_flu experiment, 143 samples were used. Power analyses or sample size justifications would be helpful.

5. The paper should discuss the hands-on time and technical expertise required to run the CARMEN RVP assay. The 192.24 array preparation, crRNA panel setup, and data analysis with custom software require specialized training. Is this realistically deployable by public health laboratories?

### Recommendation to Editor (Confidential)

**Major Revision.** The core work is solid and the topic is highly relevant. The LOD characterization, competitive inhibition experiment, and cost analysis are the key gaps. I am optimistic that these can be addressed in revision. The influenza A sensitivity issue may not be fully solvable in this study, but a frank discussion of the assay's limitations relative to its intended use would be appropriate. The multiplex CRISPR-based detection of pathogens from air is a promising direction that deserves publication, provided the validation meets the field's standards.

---
---

# PART III: NEW REVIEWER PERSONA

A new reviewer persona was created for this review:

**Reviewer 4: CRISPR-Based Diagnostics & Molecular Assay Development** — profile saved as `08_reviewer_crispr_diagnostics.md`.

This reviewer was added because the manuscript's core contribution is the adaptation of a CRISPR-Cas13-based multiplexed assay platform, which requires specialist evaluation of crRNA design, assay validation methodology, multiplexed detection challenges, and diagnostic performance metrics. None of the existing reviewer personas covered this expertise area adequately.

---

# APPENDIX: JOURNAL CALIBRATION

**Journal:** Applied and Environmental Microbiology (AEM)  
**Publisher:** American Society for Microbiology (ASM)  
**Tier:** 3 (Specialty society journal; estimated 25-35% acceptance rate)  
**Scope:** Significant contributions to applied microbial research, basic microbial ecology, and genetic/molecular investigations of practical value. Publishes methods that advance the field, not merely incremental extensions of prior work.  
**Calibration notes:** AEM expects methodological rigor and transparency, particularly for methods development papers. "Applied" in the journal name signals that the assay's practical utility and deployability are relevant evaluation criteria. The manuscript's focus on cost-effective, multiplexed pathogen detection from environmental samples is squarely within AEM's scope. However, AEM expects assay papers to include standard validation metrics (LOD, specificity, concordance with reference methods) — incomplete validation is a common reason for revision at this journal.

**Reviewer panel justification:**
- **Reviewer 1 (Bioaerosol):** Essential for evaluating air sampling methodology, sampler performance, field controls, and environmental context.
- **Reviewer 2 (Viral Genomics & Mol Epi):** Evaluates the surveillance application, genomic target selection, data interpretation, and epidemiological significance.
- **Reviewer 3 (Methods & Statistics):** Assesses statistical approaches, assay comparison methodology, figure quality, and reproducibility standards.
- **Reviewer 4 (CRISPR Diagnostics):** Specialist in the core technology, evaluating crRNA design, assay validation, multiplexing challenges, and diagnostic performance.
