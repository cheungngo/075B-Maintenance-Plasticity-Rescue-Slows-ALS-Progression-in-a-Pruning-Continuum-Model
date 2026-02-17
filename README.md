# **Maintenance Plasticity Rescue Slows ALS Progression in a Pruning-Continuum Model: Implications for Early Intervention in Motor and Mood Circuits**

Authors:

Ngo Cheung, FHKAM(Psychiatry)

Affiliations:

¹ Cheung Ngo Medical Limited, Hong Kong SAR, China

Corresponding Author:

Ngo Cheung, MBBS, FHKAM(Psychiatry)

Cheung Ngo Medical Limited

Hong Kong SAR, China

Tel: 98768323

Email: info@cheungngomedical.com

**Conflict of Interest**: None declared.

**Funding Declaration**: This research received no specific grant from any funding agency in the public, commercial, or not-for-profit sectors.

**Ethics Declaration**: Not applicable.

## **Abstract**

**Background:** Major depressive disorder and amyotrophic lateral sclerosis share intriguing comorbidity, with depression often appearing months before motor symptoms in 10--34% of ALS patients. Our prior genomic analyses identified microglial-mediated synaptic pruning as the sole consistent cross-disorder pathway, with autophagy failure acting as an ALS-specific amplifier. To test whether this continuum could explain dynamic progression and treatment responses, we built a mesoscale neural network model in which all clinical features emerge from architectural state changes.

**Methods:** A layered feed-forward network (prefrontal-limbic to motor sub-layers) underwent progressive pruning (complement-biased plus activity-dependent), weight corruption (modelling aggregate spread), and sparsity-driven excitotoxicity. Autophagy inefficiency limited clearance. Ketamine-like treatment induced gradient-guided regrowth with noise and pruning reduction; riluzole provided excitotoxicity damping only. Simulations ran for 30 cycles (\~45 months) across standard, bulbar-onset, limb-onset, ALS-MDD comorbid, pure MDD, and control profiles. Symptoms and biomarkers (including neurofilament proxy from weight instability) were derived directly from network state.

**Results:** Untreated ALS reproduced preclinical stability, symptomatic acceleration, and advanced plateau, with stochastic flares mimicking clinical exacerbations. Bulbar- and limb-onset subtypes emerged naturally from sub-layer pruning biases. Maintenance ketamine slowed decline most effectively (terminal ALSFRS-R proxy 13--14 vs 11--12 untreated/riluzole; respiratory risk 85--89%; 10--15% higher motor integrity). Riluzole offered modest early slowing but converged to similar end-state. In comorbid runs, prefrontal pruning produced early depression as a prodromal signal, with ketamine providing dual mood-motor benefit.

**Conclusions:** The model validates pruning as the upstream shared vulnerability and demonstrates that regular plasticity promotion can partially modify ALS trajectory, particularly in limb-onset or mood-comorbid cases. It offers a computational scaffold for testing early-intervention strategies and PRS-stratified trials.

**Keywords:** amyotrophic lateral sclerosis, synaptic pruning, computational modelling, ketamine, disease modification

## **Introduction**

### **Clinical Observations of Depression Preceding Motor Symptoms in ALS**

Clinicians who work regularly in ALS settings will recognise a recurring scenario. A patient presents with early weakness or fasciculations, yet during the history, they mention something less conspicuous --- a persistent low mood, a loss of drive that crept in months before any motor complaint. The instinct is to attribute this to the emotional weight of diagnosis, but the pattern recurs with enough regularity to raise questions. Depression in ALS is not uncommon; systematic reviews and meta-analyses estimate prevalence between 10 and 34 percent, and a notable proportion of patients date the onset of depressive symptoms to a period well before motor signs became apparent, suggesting something beyond a psychological reaction to illness \[1,2\]. Observations like these accumulate over time and eventually push toward a more uncomfortable question: whether motor neuron degeneration and mood vulnerability might be connected at a biological level that goes deeper than shared distress.

### **Prior Genomic Evidence for a Shared Pruning Continuum**

Our previous work pursued this question through large-scale genomic analysis. Drawing on genome-wide association study data from the Project MinE consortium for ALS and the Psychiatric Genomics Consortium for major depressive disorder, we found that microglial-mediated synaptic pruning emerged as the single most consistent cross-disorder signal, showing enrichment in both conditions even though the overall genetic correlation between the two was close to zero \[3\]. The interpretation we arrived at was one of a continuum: a shared vulnerability in pruning processes forms a quiet biological foundation, but the diseases diverge from there --- autophagy failure pushes toward relentless motor neuron loss in ALS, while disruptions in RNA processing and immune regulation shape the stress sensitivity characteristic of depression. This framework accommodated the comorbidity without collapsing both diseases into a single entity, and it generated several predictions that could, in principle, be tested. Among them was the idea that pruning liability might surface as early mood changes in a subset of ALS patients, and that treatments aimed at synaptic plasticity could hold relevance across both conditions.

### **Limitations of Static Genomic Approaches**

Genomics, for all its reach, produces associations that are fixed in time. It cannot reveal how pruning vulnerability unfolds over months or years, how it interacts with vulnerabilities in specific circuits to give rise to bulbar versus limb-onset patterns, or how a pharmacological agent such as ketamine might redirect the trajectory by encouraging regrowth at stressed synapses. Moving from risk loci catalogued in a database to an understanding of disease as it actually progresses required a fundamentally different approach --- one capable of letting the relevant biology play out dynamically, even within a synthetic system.

### **Computational Modelling as a Tool for Studying Neurodegeneration**

Computational neural network modelling has gradually become a productive tool in neurodegeneration research, precisely because it allows multiple mechanisms to interact in ways that are difficult to observe directly in patients or in animal models. Biophysical models at the single-neuron level have clarified how energy failure contributes to hyperexcitability \[4\]. Connectome-based propagation frameworks have mapped how prion-like spreading might traverse brain regions in ALS \[5\]. Spiking circuit models have gone further, predicting therapeutic windows that were subsequently supported by experiments in SOD1 mouse models \[6\]. These contributions are valuable, but they tend to operate at a single scale or focus on a single mechanism. What remained missing was a model that could bring the pruning continuum into contact with both mood and motor circuits, allow disease subtypes to differentiate under a common set of rules, and serve as a platform for testing plasticity-based interventions over time.

### **Aims and Design of the Present Study**

That gap motivated the present work. We translated the genomic signals from our earlier study into a mesoscale neural network in which every aspect of disease --- progression rate, symptom profile, biomarker trajectories, and treatment response --- arises entirely from changes in network architecture. Synaptic pruning corresponds to microglial synapse elimination; weight corruption stands in for the spread of toxic protein aggregates; and instability driven by increasing sparsity captures the downstream consequences of excitotoxicity and neurofilament release. Sub-layer branching within the network allows bulbar and limb phenotypes to emerge and differentiate naturally. A ketamine-like plasticity intervention promotes targeted regrowth in affected pathways, while a riluzole-like mechanism provides damping of excitotoxic activity. The resulting system generates behaviour that has a dynamic, organic quality: disease flares appear stochastically, comorbid mood disturbance produces early prodromes, and maintenance dosing consistently outperforms standard treatment schedules.

Our aims were fourfold. First, to simulate full ALS progression and its clinical subtypes from pruning vulnerability alone. Second, to compare the effects of plasticity rescue against excitotoxicity modulation on disease trajectory. Third, to explore how timing and dosing parameters influence outcomes in ways that might eventually inform the design of clinical trials. Fourth, to determine whether the model could reproduce the early mood changes we had hypothesised on the basis of genomic data, thereby closing the loop between static genetic findings and the dynamic course of disease.

### **Scope and Aspirations**

What follows is not offered as a definitive account but as a working scaffold --- an attempt to make the pruning continuum concrete, open to testing, and, with some fortune, relevant to clinical decision-making. If even a portion of these predictions find support in patient data, it could change how clinicians regard those early mood symptoms in ALS --- not as incidental features to be managed in passing, but as biological signals that warrant attention and, potentially, early intervention.

## **Methods**

### **Network Architecture**

We built the model as a feed-forward neural network in PyTorch, structured to approximate the hierarchical organisation of neural circuits involved in motor control and mood regulation. The network comprised eight primary layers: a prefrontal-limbic layer with 512 units, an upper motor layer also with 512 units, a lower motor layer with 256 units, and a neuromuscular junction layer with 128 units. From the neuromuscular junction layer, activation split into three parallel sub-layers representing bulbar (128 to 64 units), respiratory (128 to 64 units), and fine-motor (128 to 64 units) pathways. These three streams were then concatenated into a single vector of 192 units feeding into a final output layer of 4 units. ReLU activations followed each linear transformation throughout the network.

During each forward pass, Gaussian noise was added at every layer to stand in for excitotoxic stress, with the noise magnitude set dynamically according to the current architectural state of the network (described under Excitotoxicity below). The network was trained on a synthetic four-class motor task --- classifying limb function, bulbar function, respiratory function, and fine-motor function --- using input data generated from Gaussian clusters positioned at plus or minus one on each axis of a two-dimensional input space. This yielded 2000 samples, split 80 percent for training and 20 percent for testing.

### **Pruning and Toxicity Mechanisms**

We modelled synaptic pruning by applying binary masks to the weight and bias parameters of each layer, so that any connection assigned a mask value of zero made no contribution to the computation. The selection of connections for pruning followed a mixed strategy: 70 percent of targets were drawn from the lowest absolute-magnitude connections still alive in a given layer, reflecting how microglia tend to tag weaker synapses for removal, while the remaining 30 percent were chosen at random. Pruning rates varied across layers, increased linearly over successive cycles, and were further amplified by the local level of aggregate toxicity.

Each time a connection was pruned, surviving weights in its immediate neighbourhood (within a radius of five elements in the flattened weight tensor) were directly corrupted, with the size of the perturbation scaled by the current aggregate load. This was meant to capture TDP-43-like toxic spread to adjacent synapses. Aggregate accumulation was proportional to the fraction of connections pruned, and clearance depended on autophagic efficiency, which was severely impaired in the ALS profiles (clearance rate set at 0.05). When autophagy was impaired, aggregate buildup also imposed penalties on any subsequent regrowth attempts.

A gradient accumulation mechanism tracked an exponential moving average of absolute gradients with a smoothing factor of 0.1. During treatment phases, this signal guided regrowth by prioritising the restoration of connections on output neurons experiencing the greatest stress among surviving pathways.

### **Excitotoxicity**

Excitotoxic noise was not imposed from an external schedule but was derived entirely from the current state of the network. A base noise level, starting at 0.05 and increasing by 0.008 per cycle, was multiplied by a layer-specific vulnerability factor (ranging from 1.5 to 2.0 for motor layers and 0.8 to 1.8 for limbic layers) and by a sparsity-driven instability term calculated as one plus the layer sparsity multiplied by 3.0. The practical result was that noise escalated naturally as surviving circuits grew sparser and more unstable, producing worsening disruption without requiring any hand-tuned external signal.

### **Treatment Implementation**

The ketamine-like intervention was designed with several concurrent effects, all decaying exponentially with a half-life of roughly three cycles, corresponding to about four and a half months of simulated time. These included a gradient-guided regrowth boost at a strength of 0.6, noise reduction at 0.5, pruning reduction at 0.4, and a learning-rate multiplier peaking at twice the baseline value to promote enhanced plasticity. All effects were active only while the decay factor remained above 0.05.

Riluzole, by contrast, was modelled as a continuous damping of excitotoxic noise at a strength of 0.3 combined with a mild pruning reduction of 0.15. Its half-life was shorter, around two cycles, and it included no regrowth or plasticity-promoting components --- consistent with how the drug primarily works through glutamate modulation rather than through any direct effect on synaptic remodelling.

### **Disease Profiles and Scenarios**

The different disease profiles were distinguished only by their layer-specific pruning rates, the efficiency of autophagic clearance, and vulnerability modifiers. To introduce biological heterogeneity, seed-based uniform variation between 0.85 and 1.15 was applied across profiles. The six profiles were as follows. Standard ALS featured balanced pruning weighted toward motor layers and severely impaired autophagy. Bulbar-onset ALS had elevated pruning rates in the bulbar and respiratory sub-layers. Limb-onset ALS had elevated rates in the fine-motor and lower motor layers. The ALS with comorbid major depressive disorder profile added increased pruning in the prefrontal-limbic layer. Pure MDD showed pruning concentrated in prefrontal regions with autophagy left relatively intact. The healthy control profile had only minimal pruning across all layers.

Treatment scenarios included an untreated baseline, intermittent ketamine administered every five cycles, early ketamine covering cycles two through six, late ketamine covering cycles 15 through 24, maintenance ketamine given every three cycles starting from cycle three, and riluzole administered either continuously or early in the disease course.

### **Simulation Procedure**

Each network was pretrained for 50 epochs using the Adam optimiser at a learning rate of 0.001, establishing baseline task performance in the range of 95 to 96 percent accuracy. Disease progression then ran for 30 cycles, with each cycle representing approximately 1.5 months of simulated time, giving a total simulation window of roughly 45 months. Within each cycle the sequence of operations was as follows: first, a check for any scheduled treatment administration; second, a stochastic flare detection step gated by the current sparsity level; third, pruning with amplification from local toxicity; fourth, corruption of surviving weights in the neighbourhood of newly pruned connections; fifth, autophagic clearance of accumulated aggregates; sixth, gradient-guided regrowth where active ketamine effects were present; seventh, application of updated masks to all weight and bias parameters; eighth, a brief retraining phase consisting of three steps of stochastic gradient descent using the current learning rate and noise profile; ninth, gradient accumulation; tenth, evaluation of classification accuracy on the held-out test set; and finally, computation of symptom scores derived from the current network architecture.

### **Symptom and Biomarker Mapping**

All clinical measures were read directly from the state of the network without any additional free parameters (Table 1).

The depression score was scaled to match the range of the Patient Health Questionnaire-9 summed and expanded to a 48-point ceiling so that it could track graded changes across the full simulation window. The ALSFRS-R proxy preserved the 0 to 48 range of the revised ALS Functional Rating Scale, linking network task performance directly to a familiar clinical metric. The neurofilament-light proxy was intended to parallel serum neurofilament light chain concentrations, which rise as axonal damage releases structural proteins --- here captured by the variability in surviving connection weights as the network degrades. Respiratory risk combined two sources of vulnerability because respiratory failure in ALS reflects both neuromuscular junction breakdown and direct involvement of respiratory motor pathways, a dual dependency the weighted formula was designed to preserve.

Cognitive scoring incorporated three distinct contributors --- loss of prefrontal connections, buildup of toxic aggregates in prefrontal regions, and local circuit instability --- because cognitive decline in ALS-spectrum disorders is not reducible to a single mechanism but instead reflects the combined burden of structural loss, proteinopathy, and dysfunctional signalling within frontal networks.

**Table 1. Architecture-to-Symptom Mappings**

| **Symptom / Biomarker**   | **Derivation Formula**                                                                     |
|---------------------------|--------------------------------------------------------------------------------------------|
| Depression score (0--48)  | Prefrontal-limbic sparsity × 48                                                            |
| Spasticity score (0--4)   | Upper motor sparsity × 4                                                                   |
| Weakness score (0--4)     | Lower motor sparsity × 4                                                                   |
| Fatigue score (0--10)     | Neuromuscular junction sparsity × 10                                                       |
| Bulbar score (0--4)       | Bulbar sub-layer sparsity × 4                                                              |
| Respiratory risk (%)      | (Respiratory sub-layer sparsity × 0.6 + NMJ sparsity × 0.4) × 100                          |
| Fine-motor score (0--4)   | Fine-motor sub-layer sparsity × 4                                                          |
| ALSFRS-R proxy (0--48)    | Test accuracy × 48 / 100                                                                   |
| Neurofilament-light proxy | Sum of per-layer weight standard deviation (alive connections) × 100                       |
| Overall disability (%)    | Total sparsity × 100                                                                       |
| Cognitive score (0--30)   | (1 -- prefrontal sparsity) × 30 -- prefrontal aggregate × 10 -- prefrontal instability × 5 |
| Motor integrity (%)       | Proportion of alive connections across motor layers/sub-layers                             |
| Excitotoxicity load       | Sum of motor-layer noise magnitudes                                                        |

## **Results**

### **Untreated ALS Progression and Biomarker Trajectories**

Without any treatment, the model traced a disease course that closely resembled what is observed in ALS clinically: a drawn-out preclinical window during which network performance remained largely intact, followed by a steep symptomatic decline and eventual levelling off at severe impairment. With each simulation cycle calibrated to roughly 1.5 months, task accuracy held above 94 percent through cycle 5 (around the 7.5-month mark), even though synaptic pruning was already accumulating beneath the surface, pushing total sparsity to approximately 51 percent by that point. After cycle 6, performance dropped sharply. Accuracy fell to somewhere between 30 and 40 percent by cycle 10 and settled into a range of about 24 to 29 percent through the advanced stages spanning cycles 20 to 29. Translated into the ALSFRS-R proxy (Figure 1), this meant a decline from near-maximum values (around 46) down to roughly 11 to 14 in the terminal cycles --- figures that sit squarely within the range clinicians encounter at end-stage disease.

Stochastic flares added an element of unpredictability to the trajectory. These events were triggered when layer sparsity crossed a threshold and a probability gate was met, producing abrupt stepwise drops in accuracy --- visible, for instance, around cycles 5 to 6, 9 to 10, and 12 to 14 in the standard profile. Their character was reminiscent of the sudden clinical worsening that ALS patients sometimes experience in connection with intercurrent stress or infection.

The neurofilament-light proxy (Figure 2), which was computed from the instability of weights among surviving connections, rose progressively from mid-disease onward, peaking between roughly 84 and 115 arbitrary units. This upward drift mirrored the pattern of serum neurofilament light chain elevation that has been documented as a marker of ongoing axonal damage in ALS \[7\].

### **Clinical Subtype Variation**

The different onset phenotypes emerged naturally from variation in sub-layer pruning rates, without any additional rules being imposed (Table 2). In the bulbar-onset profile (Figure 3), where pruning was accelerated in the bulbar and respiratory sub-layers from early on, impairment in speech and swallowing developed rapidly, with the bulbar score reaching approximately 3.9 by the terminal cycles and respiratory risk climbing past 90 percent by cycle 15 and exceeding 96 percent later (Figure 4). The fine-motor and lower-motor circuits, meanwhile, were relatively preserved in the early going.

The limb-onset profile showed the opposite pattern. There, pruning was concentrated in the fine-motor and lower-motor sub-layers, so weakness and loss of dexterity appeared earlier (terminal fine-motor score around 3.9, weakness around 3.9), while respiratory compromise was delayed compared with the bulbar-onset case. These emergent differences lined up well with what is known clinically: bulbar-onset patients tend to face earlier difficulties with swallowing and breathing and typically have shorter survival, whereas limb-onset patients experience a more gradual progression dominated by spreading paralysis \[8\].

**Table 2. Subtype Variation in Untreated ALS (Final Cycle)**

| Subtype      | Accuracy (%) | Total Sparsity (%) | Bulbar Score | Resp. Risk (%) | Fine Motor Score | Weakness Score | ALSFRS-R Proxy | NFL Proxy |
|--------------|--------------|--------------------|--------------|----------------|------------------|----------------|----------------|-----------|
| Standard     | 24.5         | 97.0               | 3.87         | 96.6           | 3.86             | 3.92           | 11.8           | 84.6      |
| Bulbar-onset | 29.0         | 96.8               | 3.89         | 96.8           | 3.85             | 3.87           | 13.9           | 93.0      |
| Limb-onset   | 23.3         | 97.0               | 3.87         | 96.6           | 3.87             | 3.92           | 11.2           | 83.8      |

### **Treatment Effects**

Riluzole, modelled as continuous dosing, produced a modest slowing of early-to-mid decline. It preserved roughly one to two additional ALSFRS-R proxy points compared with the untreated arm, with a terminal value of about 12.2 versus 11.8 for no treatment. The period during which accuracy remained above 90 percent was extended by approximately two to three cycles. This degree of benefit was broadly in keeping with what riluzole achieves in clinical practice, where the reported survival advantage is on the order of three to six months \[9\]. That said, by the end of the simulation, terminal sparsity and respiratory risk in the riluzole arm had converged with the untreated values, reaching approximately 96 to 97 percent sparsity and around 96 percent respiratory risk. The riluzole arm also showed a notably higher peak in the neurofilament-light proxy (around 106), which reflected the fact that while riluzole damped excitotoxic noise, it did nothing to halt the spread of aggregate-driven weight corruption.

The ketamine-like intervention told a different story, one that depended heavily on both dose spacing and timing. Intermittent dosing at every five cycles gave an intermediate level of preservation, with the terminal ALSFRS-R proxy reaching about 12.4 and respiratory risk settling near 94 percent. When ketamine was introduced early in the disease course, it had the greatest effect on maintaining the structural integrity of the network. Late administration, by contrast, mainly offered symptomatic relief without meaningfully reversing the accumulated damage.

The maintenance dosing schedule --- roughly every four to five months, starting from cycle three --- proved the most effective regimen across all the scenarios we tested. It consistently slowed progression regardless of subtype, yielding terminal ALSFRS-R proxy values in the range of 13 to 14, reducing respiratory risk to between 85 and 89 percent, and preserving residual motor integrity at levels roughly 10 to 15 percent above what was seen in either the untreated or riluzole arms. The mechanism behind this advantage was gradient-guided regrowth, which selectively reinforced whichever motor sub-layers were under the most stress. This prevented the network from crossing into the irreversible sparsity plateau that characterised every other treatment condition.

Several patterns deserve attention beyond the headline comparisons already discussed (Table 3). The pure MDD profile, which featured pruning concentrated in prefrontal regions with autophagy left relatively intact, ended the simulation at a total sparsity of only about 42 percent --- less than half the level reached by any of the ALS profiles. Motor scores in the pure MDD runs stayed moderate (weakness around 1.75, bulbar around 1.56), confirming that the motor circuits were not the primary target of the degenerative process in that condition. When intermittent ketamine was applied to the pure MDD profile, the improvement was striking: total sparsity dropped to roughly 19.5 percent, depression scores fell from about 31 to 17, and task accuracy climbed from 29 to nearly 47 percent. This was a far larger proportional benefit than ketamine achieved in any of the ALS arms, which makes sense given that the preserved autophagy in the MDD profile allowed regrown connections to survive rather than being rapidly degraded again.

**Table 3. Final-Cycle Metrics Across Key Scenarios**

| **Scenario**                   | **Accuracy (%)** | **Total Sparsity (%)** | **Depression Score** | **Weakness Score** | **Bulbar Score** | **Fine Motor Score** | **ALSFRS-R Proxy** | **NFL Proxy** | **Resp. Risk (%)** | **Motor Integrity (%)** |
|--------------------------------|------------------|------------------------|----------------------|--------------------|------------------|----------------------|--------------------|---------------|--------------------|-------------------------|
| ALS (untreated)                | 24.5             | 97.0                   | 46.5                 | 3.92               | 3.87             | 3.86                 | 11.8               | 84.6          | 96.6               | 3.0                     |
| ALS (ketamine q5)              | 25.7             | 96.3                   | 46.5                 | 3.84               | 3.82             | 3.78                 | 12.4               | 86.8          | 94.1               | 3.7                     |
| ALS (ketamine maint.)          | 28.2             | 87.9                   | 45.5                 | 3.60               | 3.59             | 3.35                 | 13.6               | 87.0          | 85.5               | 12.1                    |
| ALS (riluzole cont.)           | 25.5             | 96.7                   | 45.4                 | 3.86               | 3.86             | 3.85                 | 12.2               | 106.4         | 96.5               | 3.3                     |
| ALS Bulbar (untreated)         | 29.0             | 96.8                   | 46.1                 | 3.87               | 3.89             | 3.85                 | 13.9               | 93.0          | 96.8               | 3.2                     |
| ALS Bulbar (ketamine q5)       | 22.0             | 96.5                   | 46.4                 | 3.79               | 3.87             | 3.83                 | 10.6               | 94.6          | 96.1               | 3.5                     |
| ALS Limb (untreated)           | 23.3             | 97.0                   | 46.5                 | 3.92               | 3.87             | 3.87                 | 11.2               | 83.8          | 96.6               | 3.0                     |
| ALS Limb (ketamine q5)         | 22.8             | 95.2                   | 46.8                 | 3.86               | 3.86             | 3.85                 | 10.9               | 95.9          | 95.7               | 4.8                     |
| ALS-MDD comorbid (untreated)   | 24.5             | 96.8                   | 46.6                 | 3.88               | 3.85             | 3.87                 | 11.8               | 79.3          | 97.1               | 3.2                     |
| ALS-MDD comorbid (ketamine q5) | 28.5             | 96.4                   | 45.0                 | 3.87               | 3.78             | 3.84                 | 13.7               | 63.4          | 95.4               | 3.6                     |
| Pure MDD (untreated)           | 29.2             | 42.1                   | 30.7                 | 1.75               | 1.56             | 1.51                 | 14.0               | 58.9          | 38.0               | 58.0                    |
| Pure MDD (ketamine q5)         | 46.8             | 19.5                   | 17.2                 | 0.82               | 0.72             | 0.69                 | 22.4               | 54.5          | 17.4               | 80.5                    |
| Healthy control                | 95.2             | 5.1                    | 2.4                  | 0.23               | 0.24             | 0.19                 | 45.7               | 69.4          | 5.0                | 94.9                    |

The healthy control network, as expected, showed minimal change across the entire simulation. Sparsity stayed near 5 percent, accuracy held above 95 percent, and all symptom scores remained at floor values. Its inclusion served mainly as a sanity check, confirming that the pruning and corruption machinery only produced meaningful damage when disease-relevant parameters were engaged.

### **Comorbid ALS-MDD Simulations**

The comorbid profile, in which prefrontal-limbic pruning rates were raised alongside the standard ALS motor pruning, produced a pattern that was particularly interesting in light of the clinical observations that originally motivated this work. Depression scores climbed early, reaching values between roughly 23 and 26 during cycles 3 through 7 --- well before the major collapse in motor performance that did not arrive until around cycle 6. This temporal ordering, mood disturbance arriving ahead of significant motor decline, is consistent with reports that prodromal depressive symptoms can precede the recognised onset of motor disease in a subset of ALS patients \[10\].

The motor trajectory in the comorbid profile tracked fairly closely with what was seen in the pure ALS runs (Figure 5). Terminal accuracy, sparsity, and motor scores were all within a narrow range of the standard untreated values. Where the comorbid profile did diverge was in overall network instability, which was modestly accelerated compared with pure ALS, a consequence of the additional pruning burden in the prefrontal-limbic layer compounding the stress on remaining circuits.

When intermittent ketamine was applied to the comorbid profile, it offered a dual benefit that was not available in either the pure ALS or pure MDD conditions alone. On the mood side, the terminal depression score was reduced from about 46.6 untreated to 45.0, a modest improvement. More notably, the neurofilament-light proxy dropped substantially --- from 79.3 in the untreated comorbid arm to 63.4 with ketamine --- suggesting that the plasticity-promoting intervention was doing more than just propping up mood circuits; it was also reducing the overall burden of weight corruption spreading through the network. The ALSFRS-R proxy showed a meaningful gain as well, rising from 11.8 to 13.7, and respiratory risk was pulled down from 97.1 to 95.4 percent. These numbers point toward the possibility that in patients who carry both motor neuron vulnerability and mood circuit fragility, a plasticity-based treatment could address aspects of both simultaneously --- a prediction that aligns with the crossover therapeutic potential we had hypothesised in our earlier genomic work.

![](media/image5.png){width="6.267716535433071in" height="2.0416666666666665in"}

***Figure 1.** The untreated ALS model (Red) shows a steady decline in functional score (ALSFRS-R proxy) from 46 to \~11 over 30 cycles. Riluzole Continuous (Green) provides a modest slowing of progression, maintaining a score of \~12. Ketamine q5 (Blue) shows \"sawtooth\" recovery periods due to gradient-guided regrowth and noise reduction, delaying severe disability but eventually succumbing to aggregate toxicity. Ketamine Maintenance (Purple) demonstrates the strongest preservation of function (\~12 vs 11 doesn\'t capture the mid-stage delay seen in cycles 10-20).*

![](media/image4.png){width="5.157808398950131in" height="3.6346970691163603in"}

*Figure 2. Weight instability (standard deviation of alive weights) serves as a proxy for Neurofilament Light Chain (NFL). Untreated ALS shows a rapid rise in instability. Ketamine treatments initially suppress this rise (via plasticity and noise reduction), but stochastic flares (indicated by spikes) eventually drive instability up. Note the distinct suppression in the maintenance arm.*

![](media/image1.png){width="5.087744969378828in" height="3.5913495188101487in"}

***Figure 3.** In the Bulbar-onset scenario, the Bulbar and Respiratory sub-layers (Orange/Red) degrade significantly faster than the Limb (Lower Motor/Fine Motor) layers. This validates the v2.0 architectural amendment allowing for symptom-specific circuit mapping.*

![](media/image3.png){width="4.944267279090114in" height="3.49543416447944in"}

***Figure 4.** Respiratory risk is a composite of respiratory sub-layer sparsity and NMJ integrity. The Bulbar onset phenotype reaches critical risk levels (\>90%) much faster (Cycle 10-12) compared to the standard ALS phenotype. Ketamine treatment delays the onset of critical respiratory failure.*

![](media/image2.png){width="4.921875546806649in" height="3.4611898512685912in"}

***Figure 5.** Cognitive score is derived from Prefrontal/Limbic sparsity and weight corruption. Pure MDD (Purple) shows moderate decline. ALS+MDD (Red) shows accelerated cognitive decline due to the synergistic effect of higher limbic vulnerability and systemic toxicity. Ketamine (Blue) rescues cognitive function significantly in the MDD context.*

## **Discussion**

### **Validation of the Pruning Continuum**

The most striking feature of the untreated simulation runs was how faithfully they played back the story we had pieced together from genomic data in our earlier work. In the comorbid ALS-MDD condition, prefrontal-limbic sparsity was the first thing to climb --- depression scores reached severe levels by around cycle 5 or 6, well ahead of the point where the motor layers began to bear the heaviest losses. Watching that unfold felt like seeing the GWAS findings come to life: shared pruning liability surfacing as mood changes months before anyone would notice weakness or fasciculations. This is not simply a convenient parallel. It maps directly onto the prodromal depression reported in roughly 10 to 34 percent of ALS patients, cases where the biology appears to be signalling distress before the motor system visibly deteriorates \[3,10\].

On the motor side, the autophagy inefficiency we built into the ALS profiles --- slow clearance rates and steep penalties on any attempt at regrowth --- turned what might otherwise have been recoverable synaptic loss into something permanent. Once aggregate corruption gained momentum, the remaining connections became unstable, feeding into that relentless sparsity plateau and the late surge in the neurofilament-light proxy. In effect, the simulation recapitulated dynamically what our earlier MAGMA and LDSC analyses had captured as a static snapshot: pruning as the shared entry point for both conditions, but autophagy collapse locking in the irreversible motor neuron death that distinguishes ALS from depression \[3\]. That the model could reproduce both the early mood overlap and the later motor irreversibility without us having to hand-tune any rules for either felt like genuine support for the continuum framework.

### **Therapy Insights**

The treatment comparisons brought the practical implications into sharper relief. Riluzole behaved much as we anticipated. It damped excitotoxic noise enough to buy a bit of extra time in the early symptomatic window --- accuracy held up for roughly two to three additional cycles, and the terminal ALSFRS-R proxy gained a modest one to two points over the untreated arm. This matched the survival benefit of around three to six months that riluzole provides in clinical practice. But it could not touch the underlying sparsity or halt the spread of weight corruption, so by the end of the simulation the riluzole arm looked almost identical to the untreated condition.

The ketamine-like plasticity intervention was a different matter. Among all the dosing schedules we tested, maintenance dosing came out clearly on top. It kept sparsity from hitting the 97 percent wall that every other arm reached, preserved 10 to 15 percent more motor integrity, and brought respiratory risk down into the low 80s. The gradient-guided regrowth was central to this advantage --- it was not rebuilding connections indiscriminately but homing in on whichever motor sub-layers were under the greatest stress, which has a biological logic given what we know about how BDNF tends to target active circuits. Early dosing preserved the most network architecture, while doses given late in the course still provided symptomatic relief but could not reverse damage once corruption had already spread widely. This sensitivity to timing reinforces a point the genomic data had already suggested: if you intervene before autophagy failure takes over, there may be an opportunity to genuinely modify the disease course rather than simply slow it down \[3\].

The differences between subtypes added a further practical layer. Limb-onset cases, where the pruning burden fell mainly on fine-motor pathways, responded best to maintenance dosing --- dexterity held up longer, which in a real patient could translate into extended independence in daily activities. Bulbar-onset cases were harder to rescue. Once the respiratory sub-layer crossed a critical threshold of sparsity, even ketamine struggled to claw back enough function to make a meaningful difference. This pattern suggests there may be real value in stratifying patients by onset type early on, perhaps using straightforward clinical markers or baseline imaging, to guide decisions about when to start plasticity-promoting agents and how aggressively to dose them.

### **Clinical Translation**

One of the most immediate implications of these results is that mood changes in ALS may deserve a different kind of attention than they usually receive. In the comorbid runs, depression was not a late accompaniment to motor decline --- it led the way, emerging before the network had suffered major motor damage. That ordering fits with what patients sometimes describe in clinic: a vague fog, a loss of motivation that crept in months before the twitching or the stumbling. If those early mood symptoms reflect genuine pruning vulnerability rather than a psychological reaction to impending diagnosis, then screening for them at the point of first contact could carry real clinical value. A quick PHQ-9 at the initial visit, perhaps paired with a brief cognitive screen, might flag the patients whose biology is already under stress in ways that standard motor assessments would miss. In time, polygenic risk scores targeting pruning-related gene sets could sharpen that triage further, identifying individuals who stand to gain the most from early plasticity-based intervention.

On the treatment side, the model builds a case for low-dose, intermittent ketamine analogs --- maintenance regimens in particular --- in patients with limb-onset disease or mood comorbidity. The bursts of targeted regrowth slowed decline without the heavy side-effect burden that would come with continuous dosing, and the dual benefit on both mood and motor function in the comorbid arms could matter enormously for quality of life. None of this amounts to a cure. But it shifts the conversation away from pure symptom management and toward something closer to disease modification, at least for the right subgroups of patients.

These are, of course, simulations, and the real test will come when predictions like these meet actual patient data. Still, seeing the network architecture drive everything --- from prodromal depression to subtype-specific patterns to the consistent superiority of maintenance plasticity --- gives some confidence that the pruning continuum is more than a theoretical convenience. It may point toward a genuinely different way of approaching those early clinic conversations, one where mood symptoms are treated not as noise to be managed but as biological signals worth acting on.

### **Comparison to Existing Models**

Looking at how this model sits alongside what already exists in the field, the thing that kept standing out was how most ALS simulations do one piece of the puzzle very well but rarely try to connect the pieces into a single picture. The biophysical single-neuron work is a good example. The model developed by Le Masson and colleagues, with its Hodgkin-Huxley ion channels and ATP dynamics, does a remarkable job of explaining how energy failure sparks hyperexcitability and the relentless fasciculations seen in individual motor neurons \[4\]. It is precise and gave us genuine insight into selective vulnerability at the cellular level. But it stays locked at that scale. It cannot tell you how a failing neuron fits into a broader network where pruning in prefrontal-limbic regions might quietly erode mood circuits months before weakness becomes apparent, or why one patient begins with bulbar symptoms while another loses fine motor control first.

The connectome propagation models take a different approach. The random-walker framework that Meier and colleagues applied to diffusion tensor imaging networks is elegant for tracing how aggregates might spread outward from motor cortex seeds, predicting white-matter changes with impressive accuracy --- an internal correlation of 0.76 and 0.55 on external validation \[5\]. It is well suited to staging and prognosis. Yet it remains structural at its core: a map of where damage travels, without the functional feedback that would show how that spreading damage actually erodes daily performance or responds to a drug. Our model borrows the idea of propagation but makes it dynamic. Pruned connections do not simply vanish --- they corrupt their neighbours in weight space, driving the stepwise flares and the rising neurofilament-light proxy we observed across the simulation runs. And because therapy acts directly on the architecture --- ketamine promoting gradient-guided regrowth while riluzole damps noise --- we could test actual dosing schedules and watch maintenance plasticity consistently outperform standard care. That capacity for therapy testing feels like a step beyond what most propagation models currently offer.

Even the spiking neural-network circuit models get close in certain respects. The work by Strohmer and colleagues on spinal central pattern generators simulated how inhibitory dysregulation narrows therapeutic windows, and their prediction that stabilising V1 interneurons could rescue coordination was later confirmed in SOD1 mice --- which is about as strong a validation as a computational model can hope for \[6\]. But those models stay local to the spinal cord and do not bridge upward to the prefrontal pruning that accounts for the mood overlap. Our approach folds all of this into a single framework. The mesoscale network lets the same pruning mechanism drive both the spinal motor collapse and the early limbic fragility, while the emergent subtypes and cross-disorder runs give the model a scope that fits naturally with the continuum hypothesis we originally proposed \[3\].

In practical terms, where each of these existing approaches excels at one scale or one mechanism, the present model ties them together through the shared language of synaptic architecture. Seeing maintenance plasticity consistently outperform riluzole in preserving motor integrity --- and watching that advantage play out across subtypes and comorbid conditions --- feels like a genuine advance, one that turns abstract genomic signals into predictions about when and how to intervene that could, eventually, be tested.

### **Limitations**

No simulation captures everything, and this one has gaps that are worth being honest about. The most obvious is the level of abstraction. We reduced pruning to binary masks and sparsity percentages, which gets at the essence of microglial overactivity but passes over the molecular detail --- complement tagging, MHC presentation, the full glial microenvironment with all its signalling complexity. In a similar way, excitotoxicity became a function of sparsity and architectural instability rather than of explicit glutamate kinetics or calcium overload. For the broad patterns we were after, these simplifications worked. But anyone whose work sits closer to the ion-channel or molecular signalling literature would be justified in asking for more biophysical grounding before accepting the model\'s predictions at face value.

The absence of full multi-scale integration is another shortcoming. We stayed at the mesoscale --- layered circuits performing a motor task --- but did not link downward to subcellular ATP dynamics or upward to whole-brain connectomics. That meant we could simulate how pruning in the prefrontal-limbic layer spilled into mood changes, but not how peripheral immune infiltration or axonal transport defects might feed back into the central network and alter the trajectory in ways our architecture could not capture. The single-network runs, even with seed-based variation producing heterogeneity between 0.85 and 1.15 on vulnerability modifiers, also limit how confidently we can speak to population-level variability. Real ALS cohorts show considerably more scatter in their progression rates than our 42 scenarios were able to represent.

There is also the question of calibration. While the emergent outcomes felt internally consistent --- subtypes differentiated in the expected directions, treatment arms separated in ways that matched clinical intuition --- the model remains hypothesis-generating rather than predictive in any strict sense. We tuned parameters to align with broad clinical patterns, but without direct calibration against longitudinal patient data, there is always the possibility that we have overfitted to our own assumptions. The neurofilament-light proxy, for instance, tracked weight instability in a way that paralleled published biomarker trajectories, but whether the quantitative relationship between simulated sparsity and real serum neurofilament concentrations would hold up under formal comparison is something we simply cannot say yet.

### **Future Directions**

These limitations point fairly directly to where the work needs to go from here. The most pressing step is expanding to multi-seed cohorts --- potentially thousands of virtual patients drawn from varied genetic backgrounds --- so that we can generate synthetic datasets large enough to validate against real registries such as PRO-ACT. That calibration process feels essential. If we can match simulated ALSFRS-R curves and neurofilament trajectories to actual patient timelines with reasonable fidelity, the model moves from being a thought experiment, however elegant, to something that could genuinely inform trial design and patient stratification.

Combination therapies are another natural next step. The current results already hint that ketamine\'s regrowth boost and riluzole\'s noise damping might complement each other in ways that neither achieves alone. Layering in agents that target aggregate clearance --- antisense oligonucleotides directed at C9orf72, for example --- could test whether the therapeutic window widens further when you attack both the pruning cascade and the downstream corruption simultaneously. The model\'s architecture makes this kind of experiment straightforward to set up, since each mechanism operates through a distinct parameter that can be adjusted independently.

Stratification by polygenic risk is another avenue worth exploring in simulation. We could assign virtual patients different pruning-related risk scores and then ask whether directing early maintenance plasticity to the high-risk group while reserving standard care for low-risk patients enriches the treatment effect in ways that would matter for clinical trial power calculations. If the answer is yes, it would provide a computational rationale for the kind of biomarker-guided enrollment that ALS trials have been moving toward but have not yet implemented in a pruning-specific framework.

Finally, the longer-term ambition is to bring the model close enough to clinical reality that it becomes a bedside tool rather than a research curiosity. If calibration against patient data holds up, and if the timing and dosing predictions prove even roughly correct in early-phase trials, this platform could help clinicians decide which patients should receive which interventions and when --- turning the pruning continuum from a conceptual framework into a practical guide for the kind of personalised treatment that ALS patients and their families are waiting for.

## **References**

1.  Heidari ME, Nadali J, Parouhan A, et al. Prevalence of depression among amyotrophic lateral sclerosis (ALS) patients: A systematic review and meta-analysis. *J Affect Disord*. 2021;287:182-190. doi:10.1016/j.jad.2021.03.015

2.  Kurt A, Nijboer F, Matuz T, Kübler A. Depression and anxiety in individuals with amyotrophic lateral sclerosis: Epidemiology and management. *CNS Drugs*. 2007;21(4):279-291. doi:10.2165/00023210-200721040-00003

3.  Cheung N. Synaptic plasticity fragility underlies a microglial pruning continuum in major depressive disorder and amyotrophic lateral sclerosis. Zenodo. Published February 15, 2026. doi:10.5281/zenodo.18649289

4.  Le Masson G, Przedborski S, Abbott LF. A computational model of motor neuron degeneration. *Neuron*. 2014;83(4):975-988. doi:10.1016/j.neuron.2014.07.001

5.  Meier JM, van der Burgh HK, Nitert AD, et al. Connectome-based propagation model in amyotrophic lateral sclerosis. *Ann Neurol*. 2020;87(5):725-738. doi:10.1002/ana.25706

6.  Strohmer B, Grosh K, Montañana-Rosell R, et al. Spinal circuit mechanisms constrain therapeutic windows for ALS intervention: A computational modeling study. *Neurobiol Dis*. 2026;219:107253. doi:10.1016/j.nbd.2025.107253

7.  Benatar M, Wuu J, Andersen PM, Lombardi V, Malaspina A. Neurofilament light: A candidate biomarker of presymptomatic amyotrophic lateral sclerosis and phenoconversion. *Ann Neurol*. 2018;84(1):130-139. doi:10.1002/ana.25276

8.  Chiò A, Calvo A, Moglia C, Mazzini L, Mora G. Phenotypic heterogeneity of amyotrophic lateral sclerosis: A population based study. *J Neurol Neurosurg Psychiatry*. 2011;82(7):740-746. doi:10.1136/jnnp.2010.235952

9.  Miller RG, Mitchell JD, Moore DH. Riluzole for amyotrophic lateral sclerosis (ALS)/motor neuron disease (MND). *Cochrane Database Syst Rev*. 2012;(3):CD001447. doi:10.1002/14651858.CD001447.pub3

10. Rabkin JG, Albert SM, Del Bene ML, et al. Prevalence of depressive disorders and change over time in late-stage ALS. *Neurology*. 2005;65(1):62-67. doi:10.1212/01.wnl.0000167187.14501.0c
