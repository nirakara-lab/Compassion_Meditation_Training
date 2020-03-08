# The Impact of Compassion Meditation Training on Well-being and Related Variables: A Network Perspective
[![DOI](https://zenodo.org/badge/245776569.svg)](https://zenodo.org/badge/latestdoi/245776569)


We computed networks comprising associations among well-being and other psychological variables before and after a Compassion Cultivation Training (CCT). Associations between self-compassion and adaptative emotional and cognitive regulation variables became stronger following CCT. The strength and expected influence centrality values (i.e., importance and influence in the network) increased for self-compassion measures, whereas the values declined for depression, anxiety, brooding, non-judgment and non-reactivity. After CCT, self-compassion, non-attachment, decentering, and emotional reappraisal were the most important nodes connecting the different subnetworks (i.e., highest bridge centrality values). Compassion, mindfulness, and well-being were the most predictable nodes (i.e., variance explained) by other nodes in the network, whereas psychopathology-related constructs diminished in their predictability after the program. Community analysis detected five clusters of nodes (i.e., psychopathology, self-compassion, mindfulness, well-being and compassion) prior to CCT and these remained largely unchanged after CCT. These results clarify the mechanisms through which compassion meditation may produce its effects.



## Sample description
Between April and December 2017, 198 participants enrolled in a standardized 8-week CCT at a university-associated research center specializing in Mindfulness and Compassion-Based Interventions. Inclusion criteria for the CCT were as follows: 1) 18 years of age or more, and 2) not having any current serious psychological disorder or substance use.
Statistical analyses were conducted only for data from participants who completed pre-assessment and attended a minimum of 6 sessions (i.e., 75% of the program).

After applying all exclusion criteria, data from a total of 96 individuals were included in all analyses. Participants mean age was 47.78 (SD=9.80), 75% women, 93.7 % had higher education, 42.7% married, 79.2% employed, 11.5% with physical illness, 85.4% with previous meditation experience, being the meditation years average was 4.81 (SD=5.58).

## Constructs and instruments of study
### Mindfulness
-	Five-Facet Mindfulness Questionnaire-Short Form (FFMQ, 20 items [α = .87]; [71]). It  includes five component skills of of mindfulness: observing, describing, acting with awareness, non-judging of inner experience, and non-reactivity to inner experience
-	Non-Attachment Scale (NAS, 30 items [α = .93]; [72]). It measures the absence of fixation on thoughts, images, or sensory inputs, as well as an absence of internal pressure to get, hold, avoid, or change circumstances or experiences.
-	Experiences Questionnaire (EQ, 11 items [α = .89]; [73]). It assesses the ability to observe one’s thoughts and feelings in a detached manner.
-	Multidimensional assessment of interoceptive awareness (MAIA, 32 items [α = .94];  [74]). It measures interoceptive body awareness.

### Compassion
-	Self-Compassion Scale-Short Form (SCS-SF, 12 items [α = .88]; [75]). It measures three components of compassion to oneself: self-kindness, common humanity, and mindfulness.
-	Compassion Scale (CSP, 24 items [α = .86]; [76]). It assesses compassion to others, through the following components: kindness, indifference, common humanity, separation, mindfulness and disengagement.
-	Interpersonal Reactivity Index (IRI, 14 items [α = .77]; [77]). It measures empathy towards others. In this study only the Empathic Concern subscale was included.
### Psychological well-being
-	Satisfaction With Life Scale (SWLS, 5 items [α = .87]; [78]). This is a measure of global life satisfaction.
-	Life Orientation Test–Revised (LOT-R, 10 items [α = .67]; [79]). It measures dispositional optimism.
-	Pemberton Happiness Index (PHI, 11 items [α = .91]; [80]). A measure that includes both hedonic and eudaimonic components of psychological well-being.
### Psychological Distress
-	Depression Anxiety Stress Scales (DASS-21, 21 items [α = .92]; [81]). It measures symptoms of depression, anxiety and stress.
### Emotional and cognitive control
-	White Bear Supression Inventory (WBSI, 10 items [α = .89]; [82]). It measures unwanted intrusive thoughts and thought suppression.
-	Ruminative Response Style (RRS, 22 items [α = .92]; [83]). It assesses an excessive focus on causes and consequences of depressive symptoms. It includes two factors: reflection and brooding.
-	Emotion Regulation Questionnaire (ERQ, 10 items [α = .76]; [84]). It measures two emotional regulation strategies: reappraisal and suppression.
-	Attentional Control Scale (ACS, 20 items [α = .84]; [85]). It assesses perceived ability in executive control over attention.

### Dataframe

*network_pre*: 25 variables. Online assessment was completed the week before starting MBSR.
- **mindfulness** ="FFMQ_O","FFMQ_D","FFMQ_A","FFMQ_J","FFMQ_R" (5 subscales of Five-Facet Mindfulness Questionnaire-Short Form), "NAS","EQ","MAIA".
- **compassion** = "SCS_A","SCS_H","SCS_M"(3 subscales of Self-Compassion Scale-Short Form),"CSP","IRI_E" (empathy subscale of Interpersonal Reactivity Index),
- **psychologycal wellbeing** = "SWLS","LOT","PHI",
- **psychologycal distress** = "DASS_S","DASS_D","DASS_A"(3 subsclaes of Depression Anxiety Stress Scales)
- **Emotional and cognitive control** = "WBSI", "RRS_B", "RRS_R"(2 subsclale of Ruminative Response Style), "ERQ_R", "ERQ_S" (2 subscales of Emotion Regulation Questionnaire), "ACS"

*network_post*: 25 variables. Online assessment was completed during the week after the end of the MBSR.
- **mindfulness** ="FFMQ_O","FFMQ_D","FFMQ_A","FFMQ_J","FFMQ_R" (5 subscales of Five-Facet Mindfulness Questionnaire-Short Form), "NAS","EQ","MAIA".
- **compassion** = "SCS_A","SCS_H","SCS_M"(3 subscales of Self-Compassion Scale-Short Form),"CSP","IRI_E" (empathy subscale of Interpersonal Reactivity Index),
- **psychologycal wellbeing** = "SWLS","LOT","PHI",
- **psychologycal distress** = "DASS_S","DASS_D","DASS_A"(3 subsclaes of Depression Anxiety Stress Scales)
- **Emotional and cognitive control** = "WBSI", "RRS_B", "RRS_R"(2 subsclale of Ruminative Response Style), "ERQ_R", "ERQ_S" (2 subscales of Emotion Regulation Questionnaire), "ACS"

### Script of network analysis in R
*MBSR_network_analysis.R* contains the analysis done in the paper and the supplementary material.
