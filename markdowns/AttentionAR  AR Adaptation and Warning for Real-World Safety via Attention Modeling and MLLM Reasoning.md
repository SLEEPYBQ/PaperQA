![](_page_0_Picture_0.jpeg)

![](_page_0_Picture_1.jpeg)

![](_page_0_Picture_2.jpeg)

Latest updates: [hps://dl.acm.org/doi/10.1145/3746059.3747674](https://dl.acm.org/doi/10.1145/3746059.3747674)

# RESEARCH-ARTICLE AentionAR: AR Adaptation and Warning for Real-World Safety via Aention Modeling and MLLM Reasoning

[YUNQIANG](https://dl.acm.org/doi/10.1145/contrib-99661391092) PEI, University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China, Chengdu, Sichuan, [China](https://dl.acm.org/doi/10.1145/institution-60005465)

[RENMING](https://dl.acm.org/doi/10.1145/contrib-99661421164) HUANG, University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China, Chengdu, [Sichuan, China](https://dl.acm.org/doi/10.1145/institution-60005465)

[MINGFENG](https://dl.acm.org/doi/10.1145/contrib-99661393364) ZHA, University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China, Chengdu, [Sichuan, China](https://dl.acm.org/doi/10.1145/institution-60005465)

[GUOQING](https://dl.acm.org/doi/10.1145/contrib-99659896958) WANG, University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China, Chengdu, [Sichuan, China](https://dl.acm.org/doi/10.1145/institution-60005465)

PENG [WANG](https://dl.acm.org/doi/10.1145/contrib-99661322751), University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China, Chengdu, Sichuan, [China](https://dl.acm.org/doi/10.1145/institution-60005465)

QIAO [KANG](https://dl.acm.org/doi/10.1145/contrib-99661715375)

[View](https://dl.acm.org/doi/10.1145/3746059.3747674) all

.

Open Access [Support](https://libraries.acm.org/acmopen) provided by:

University of Electronic Science and [Technology](https://dl.acm.org/doi/10.1145/institution-60005465) of China

Tongji [University](https://dl.acm.org/doi/10.1145/institution-60073652)

![](_page_0_Picture_15.jpeg)

![](_page_0_Picture_16.jpeg)

Published: 28 September 2025

[Citation](https://dl.acm.org/action/exportCiteProcCitation?dois=10.1145%2F3746059.3747674&targetFile=custom-bibtex&format=bibtex) in BibTeX format

UIST '25: The 38th [Annual](https://dl.acm.org/conference/uist) ACM [Symposium](https://dl.acm.org/conference/uist) on User Interface Soware and [Technology](https://dl.acm.org/conference/uist) *September 28 - October 1, 2025 Busan, Republic of Korea*

Conference Sponsors: [SIGCHI](https://dl.acm.org/sig/sigchi) [SIGGRAPH](https://dl.acm.org/sig/siggraph)

# AttentionAR: AR Adaptation and Warning for Real-World Safety via Attention Modeling and MLLM Reasoning

[Yunqiang](https://orcid.org/0000-0001-6778-4688) Pei University of Electronic Science and Technology of China Chengdu, China [yqsimonpei3940@hotmail.com](mailto:yqsimonpei3940@hotmail.com)

[Guoqing](https://orcid.org/0009-0002-9812-4548) Wang University of Electronic Science and Technology of China Chengdu, China gqwang0420@uestc.edu.cn

[Renming](https://orcid.org/0009-0009-6459-3099) Huang University of Electronic Science and Technology of China Chengdu, China [hrenming13@gmail.com](mailto:hrenming13@gmail.com)

Peng [Wang](https://orcid.org/0000-0002-5397-9115) University of Electronic Science and Technology of China Chengdu, China [p.wang6@hotmail.com](mailto:p.wang6@hotmail.com)

[Yang](https://orcid.org/0000-0002-5070-4511) Yang University of Electronic Science and Technology of China (UESTC) Chengdu, China

yang.yang@uestc.edu.cn

[Mingfeng](https://orcid.org/0000-0003-0186-2940) Zha University of Electronic Science and Technology of China Chengdu, China [zhamf1116@gmail.com](mailto:zhamf1116@gmail.com)

> Qiao [Kang](https://orcid.org/0009-0009-0669-0085) Non-affiliated Shanghai, China [qiaokang1213@gmail.com](mailto:qiaokang1213@gmail.com)

[Heng](https://orcid.org/0000-0002-2999-2088) Tao Shen Tongji University Shanghai, China UESTC Chengdu, China [shenhengtao@hotmail.com](mailto:shenhengtao@hotmail.com)

<span id="page-1-0"></span>![](_page_1_Picture_9.jpeg)

Figure 1: Overview of the AttentionAR system architecture with four modules: (A) Attention Detection, assessing user attention via EEG, IMU, and gaze data; (B) Egocentric Data Acquisition, capturing real-time visual and contextual information; (C) Hazard Reasoning, using multi-frame analysis to infer risk levels, sources, and directions; and (D) AR Adaptation & Warning, dynamically adjusting the AR interface for timely safety alerts.

Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and the full citation on the first page. Copyrights for components of this work owned by others than the author(s) must be honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists, requires prior specific permission and/or a fee. Request permissions from [permissions@acm.org](mailto:permissions@acm.org). UIST '25, Busan, Republic of Korea

#### Abstract

Augmented Reality is rapidly transforming everyday experiences, yet its deployment in dynamic, real-world settings often undermines user safety and situational awareness. Existing AR interfaces

<sup>©</sup> 2025 Copyright held by the owner/author(s). Publication rights licensed to ACM. ACM ISBN 979-8-4007-2037-6/25/09 <https://doi.org/10.1145/3746059.3747674>

typically employ static designs that fail to adapt to fluctuating environmental conditions and shifts in user attention. In this paper, we introduce AttentionAR, a proof-of-concept system whose primary contribution is the novel integration of real-time attention monitoring with contextual hazard assessment to dynamically adjust AR overlays. Our approach comprises three complementary modules: an Attention Awareness module that processes physiological and behavioral signals to distinguish between internal and external attention; a Scene Awareness module that leverages multi-frame image analysis and chain-of-thought reasoning via multimodal language models to evaluate risks; and an AR Adaptation and Warning module that modulates interface transparency and delivers timely alerts. Our user study provides initial evidence that this integrated approach can enhance situational awareness and mitigate distraction-related risks compared to static interfaces. We conclude by discussing the implications of our findings, including the challenges of model generalizability that highlight a critical need for personalization, positioning AttentionAR as a foundational step toward more robust, attention-aware safety systems.

#### CCS Concepts

• Human-centered computing → Mixed / augmented reality; Virtual reality; Interactive systems and tools.

#### Keywords

Augmented Reality, Attention Detection, Scene Awareness, Physiological and Behavioral Signals, Adaptive User Interfaces, Large Language Models.

#### ACM Reference Format:

Yunqiang Pei, Renming Huang, Mingfeng Zha, Guoqing Wang, Peng Wang, Qiao Kang, Yang Yang, and Heng Tao Shen. 2025. AttentionAR: AR Adaptation and Warning for Real-World Safety via Attention Modeling and MLLM Reasoning. In The 38th Annual ACM Symposium on User Interface Software and Technology (UIST '25), September 28–October 01, 2025, Busan, Republic of Korea. ACM, New York, NY, USA, [19](#page-19-0) pages. [https://doi.org/10.1145/3746059.](https://doi.org/10.1145/3746059.3747674) [3747674](https://doi.org/10.1145/3746059.3747674)

#### 1 Introduction

With the rapid proliferation of augmented reality (AR) technology in daily life, its applications have expanded across various domains, addressing safety concerns in gaming [\[73\]](#page-18-0), industry [\[55,](#page-17-0) [87\]](#page-18-1), and household environments [\[84\]](#page-18-2). However, AR may impair perception [\[41,](#page-17-1) [80\]](#page-18-3), divide attention, or even cause distractions [\[44\]](#page-17-2). These issues become particularly critical during everyday activities such as walking [\[73\]](#page-18-0) or climbing stairs [\[102\]](#page-19-1), where virtual information presented by AR devices can divert attention, leading to a diminished awareness of potential real-world hazards. This lack of awareness increases the risk of accidents [\[32\]](#page-17-3). Indeed, accidents stemming from reduced situational awareness (SA) due to AR immersion are on the rise [\[41\]](#page-17-1).

Situational awareness is widely recognized as a key factor in ensuring user safety, making it a crucial area for AR advancements [\[42\]](#page-17-4). Originally defined as "the perception of the elements in the environment within a volume of time and space, the comprehension of their meaning, and the projection of their status in the near future" [\[23\]](#page-17-5), SA consists of three levels: perception, comprehension, and projection [\[24\]](#page-17-6). The effectiveness of SA heavily relies on attention allocation [\[53\]](#page-17-7). Human attention is classified into internal attention (focusing on internal cognitive processes such as recalling a phone number or planning a schedule [\[40,](#page-17-8) [67\]](#page-18-4)) and external attention (focusing on spatial locations, temporal events, or sensory inputs to interact with the external world) [\[17\]](#page-17-9). Within AR environments, external attention is further divided into attention directed at AR elements and attention directed at the real world [\[13,](#page-16-0) [49,](#page-17-10) [81,](#page-18-5) [91,](#page-18-6) [92\]](#page-18-7). However, both internal attention and attention directed at AR elements can divert users' focus from the real-world environment. When users operate AR devices in complex or dynamic environments, attention shifts often lead to "look-but-fail-tosee" phenomena [\[20,](#page-17-11) [54\]](#page-17-12), where users, despite gazing at potential hazards, fail to register or interpret them correctly if their attention is preoccupied with internal thoughts [\[30\]](#page-17-13). This disruption directly impairs SA Level 1 (perception) [\[20\]](#page-17-11), significantly increasing accident risks, particularly in activitiessuch as walking or driving. Thus, a critical challenge remains: how to establish a real-time coupling mechanism between dynamic scene risk analysis and user attention interference within AR environments, enabling automated interface adaptation.

Existing studies have attempted to address AR-induced distractions from four main perspectives. 1) Environmental Perception: Traditional approaches rely on static snapshots of the environment (e.g., pothole detection [\[63\]](#page-18-8) and construction hazard avoidance [\[46\]](#page-17-14)) but lack continuoustracking ofscene dynamics. As a result, they fail to analyze the temporal attributes of hazardous objects (e.g., pedestrian or vehicle movement) and their spatial-temporal correlation with user behavior. 2) Attention Management: Previous research primarily focuses on either internal attention (e.g., suppressing AR notifications to maintain cognitive flow [\[90,](#page-18-9) [97\]](#page-18-10)) or external attention (e.g., preventing interruptions when users are immersed in AR content [\[50,](#page-17-15) [71\]](#page-18-11)), without integrating both to enable real-time AR adjustments based on dynamic user attention shifts. 3) Adaptation Triggering Mechanism: Some studies introduce AR adaptation strategies that prevent UI elements from obstructing critical safety information (e.g., emergency exit signs [\[25,](#page-17-16) [57\]](#page-17-17)). However, most rely on manual activation mechanisms [\[57\]](#page-17-17), making responses to safety hazards delayed and lacking proactive warning functionalities. 4) AR-based Warnings can enhance safety awareness, but vague or improperly designed alerts may introduce distractions in hazardous situations due to poor attention guidance [\[5,](#page-16-1) [42\]](#page-17-4).

These limitations stem from a common blind spot: the absence of a unified computational model that integrates dynamic risk prediction with evolving user attention states.

To address this gap, this study integrates spatial-temporal scene dynamics and continuous attentional states into a unified analytical framework. Unlike traditional static analyses, we propose leveraging multimodal large language models (MLLMs) to infer spatial-temporal hazard patterns from video streams (e.g., abnormal pedestrian trajectories). Additionally, physiological and behavioral signals—including electroencephalography (EEG), head movement data from inertial measurement units (IMU), and eyetracking data—are used to model dynamic attention shifts. Based on these multimodal inputs, our system autonomously adapts AR

interfaces to mitigate distractions. This "scene-user" joint perception mechanism offers a novel approach to AR safety enhancement in dynamic environments ( [Figure](#page-1-0) 1).

The contributions of this paper are as follows:

1. A Novel Integrated System for Attention-Gated Risk Assessment: We present the design and implementation of AttentionAR, a system that, to our knowledge, is the first to create a closed-loop pipeline connecting a user's real-time physiological attention state, through a large-model-based dynamic risk assessment, to a contextually-aware adaptive interface. Our primary contribution lies in the novel orchestration of these components to create a new, intelligent system capability for real-world AR safety.

2. A Spatiotemporal Hazard Inference Strategy Using Multi-Frame MLLM Reasoning: We propose and validate a prompting strategy that guides an MLLM to reason about spatio-temporal hazards in egocentric video, identifying not just objects but the source, direction, and severity of potential risks.

3. A Multimodal Attention Model and its In-the-Wild Validation: By integrating EEG, IMU, and gaze data, we construct a user attention model and demonstrate, through a real-world user study, that our integrated system significantly enhances situational awareness and safety perception.

#### 2 Related work

Existing research leverages physiological and behavioral signals, MLLMs, and AR technologies to explore attention mechanisms, analyze complex environments, and optimize safety warnings. These efforts collectively enhance situational awareness and improve safety interventions.

# 2.1 Understanding Attention through Physiological and Behavioral Signals

Monitoring physiological and behavioral signals has provided crucial insights into the neural mechanisms of attention regulation.

Attention control is largely influenced by the prefrontal cortex's default inhibitory properties [\[88\]](#page-18-12), particularly reflected in theta and alpha wave activity recorded from EEG electrodes F1 and F2 [\[90\]](#page-18-9). During focused states, event-related desynchronization (ERD) in these bands indicates reduced activity, with alpha wave ERD enhancing external attention and alpha wave synchronization (ERS) facilitating internal cognitive processes, such as mental arithmetic [\[64,](#page-18-13) [83\]](#page-18-14). This distinction helps differentiate whether a user is engaged with the external environment or internal thought processes.

To pinpoint external attention focus, multimodal approaches combining different physiological and behavioral signals improve classification accuracy and robustness. Head movement (e.g., IMUbased acceleration and angular velocity) is used to determine attentiveness via threshold-based methods, allowing for minor movements while reducing misclassification [\[51\]](#page-17-18). Meanwhile, gaze tracking identifies the user's specific point of focus. Further, integrating EEG and eye-tracking (ET) data enables real-time differentiation between internal and external attention states [\[91\]](#page-18-6).

#### 2.2 (M)LLMs in Situational Awareness

LLMs have demonstrated strong reasoning abilities in interpreting ambiguous language and assessing how complex environments influence user behavior. They have been applied to evaluate human input/output availability by detecting Situationally Induced Impairments and Disabilities(SIIDs) [\[61\]](#page-18-15) and to predict user behavior from multimodal scene data [\[52\]](#page-17-19). By incorporating advanced semantic analysis, LLM-powered systems improve the interpretation of user intent [\[96\]](#page-18-16).

However, LLMs alone face limitations in human-computer interaction, as they struggle to process complex real-world scenarios involving visual, auditory, and sensor data [\[27,](#page-17-20) [99\]](#page-18-17). To address this, MLLMs integrate multiple data streams to enhance situational awareness [\[10,](#page-16-2) [99\]](#page-18-17). Open-source frameworks like LLaVA [\[60\]](#page-18-18) exemplify this by seamlessly combining vision and language tasks.

Integrating thermal imaging data with MLLMs hasshown promise in improving safety and functionality in autonomous driving (ADS) and intelligent transportation systems (ITS) [\[6\]](#page-16-3). By leveraging MLLMs' visual and logical reasoning capabilities, these systems can detect potential hazards in complex traffic environments [\[1\]](#page-16-4). Additionally, the ability to process multiple images is crucial for Large Vision-Language Models (LVLMs) to develop a more comprehensive scene understanding [\[66\]](#page-18-19).

#### 2.3 AR Adaptation and Safety Warnings

Dynamic AR adaptation and timely safety warnings are critical for user safety in real-world applications. AUIT [\[25\]](#page-17-16) provides optimization tools for adapting UI elements to meet accessibility, visibility, and consistency requirements in XR applications. Building on this, SituationAdapt [\[57\]](#page-17-17) enhances safety by preventing UI elements from obstructing critical real-world information or causing visual distractions.

However, adaptation alone does not guarantee heightened safety awareness, particularly in high-workload environments [\[5\]](#page-16-1). While AR-based warnings can improve hazard perception [\[2,](#page-16-5) [45\]](#page-17-21), ineffective designs may cause distractions [\[78\]](#page-18-20), especially if they lack clear attention guidance [\[42\]](#page-17-4). This risk is particularly concerning in hazardous scenarios, where ambiguous warnings can inadvertently misdirect user focus [\[5\]](#page-16-1).

#### 2.4 AR in Locomotion Contexts

A substantial body of work has explored the challenges of AR usage during walking. Several studies have focused on designing AR interfaces for specific mobile contexts, such as virtual meetings [\[12\]](#page-16-6) or general text presentation in dual-task situations [\[47\]](#page-17-22), while others have investigated more fundamental aspects of interaction, such as spatial UI transition mechanisms [\[62\]](#page-18-21) and the effect of spatial reference frames on target acquisition [\[65\]](#page-18-22). Concurrently, systems have been developed to directly address safety, for instance, by detecting obstacles for smartphone users [\[43\]](#page-17-23) or specifically for "texting while walking" scenarios [\[48,](#page-17-24) [76\]](#page-18-23). This extends to research on using peripheral vision for notifications [\[14\]](#page-17-25) and even radical approaches like substituting real-world walking with dynamically generated VR experiences in systems like VRoamer [\[16\]](#page-17-26) and Dreamwalker [\[98\]](#page-18-24).

While this foundational work addresses AR usability and direct obstacle avoidance, AttentionAR's contribution is distinct. Our

UIST '25, September 28–October 01, 2025, Busan, Republic of Korea Pei, et al.

<span id="page-4-2"></span>![](_page_4_Figure_2.jpeg)

(a) Hardware setup (b) Experimental tasks for inducing internal/external attention

Figure 2: Attention Data Collection during Four Tasks. (a) Twenty-three participants wore a HoloLens 2 and a Brainco Oxyzen EEG device for data acquisition. (b) Participants completed four tasks designed to induce internal and external attention.

work addresses the cognitive layer of safety, specifically the "inattentional blindness" problem [\[93\]](#page-18-25), where a user might look at a hazard but fail to perceive it. Unlike the systems above, we close the loop between the user's internal physiological state and a deep, MLLM-based understanding of the environment, providing a safety net for moments of cognitive, rather than purely visual, distraction.

## 3 User Attention Modeling

## <span id="page-4-3"></span>3.1 Data Collection

To classify internal and external attention, we collected EEG and IMU data. The IMU recorded linear acceleration, angular velocity, and Euler angles across three orthogonal axes, capturing head posture in three-dimensional space.

Participants and Setup. Twenty-three participants (ages 21–30, five females), including four with prior AR experience, wore the HoloLens 2[1](#page-4-0) and the Brainco Oxyzen EEG device[2,](#page-4-1) which recorded data at 256 Hz (see [Figure](#page-4-2) 2a). None of the participants reported a history of neurological disorders.

Experimental Scenario and Tasks. Participants wore the HoloLens 2 and completed four tasks designed to induce internal or external attention (see [Figure](#page-4-2) 2b).

Mental Rotation Task (Task 0) [\[81\]](#page-18-5) (internal): Participants judged whether two virtual geometric 3D models were identical. The task consisted of 15 subtasks, each lasting 10 seconds.

Mental Arithmetic Task (Task 1) [\[34,](#page-17-27) [74\]](#page-18-26) (internal): Participants mentally solved multiplication problems displayed on an AR panel. The task included five subtasks, each lasting 30 seconds.

Word Counting Task (Task 2) (external): Participants read an AR-displayed English passage ( 50 words) and counted specific words (e.g., words with exactly five letters). The task included five subtasks, each lasting 30 seconds.

Cup-and-Ball Guessing Task (Task 3) (external): In a realworld setting, an experimenter continuously swapped the positions

of three paper cups, with one concealing a small ball. Participants had to track the cup containing the ball until the task ended. Given its continuous nature, this task was not divided into subtasks.

Task Duration and Data Collection. Each task lasted 2 minutes and 30 seconds, during which EEG and IMU data were recorded. A 5-second countdown preceded each task, during which no signals were recorded. Participants rested for 1–2 minutes between tasks to mitigate carry-over effects [\[7\]](#page-16-7). Within the same task, no breaks were given between subtasks, and participants had to provide an answer before moving to the next subtask. To prevent premature completion, each subtask was designed with an appropriate level of difficulty. Each participant's session lasted 40 minutes, including pre-experiment questionnaires (age, AR experience, etc.), device setup, task execution, breaks, and a post-experiment interview (answer validation, user experience feedback, etc.). In total, approximately three hours of synchronized EEG and IMU data were collected.

## 3.2 Data Preprocessing

Data Processing and Analysis. Raw physiological and behavioral data are inherently non-stationary and susceptible to motion artifacts [\[70\]](#page-18-27). Therefore, participants were instructed to move their heads naturally while avoiding excessive movements. After filtering out invalid data (for example, missing data due to device disconnection and one subject (S17) who couldn't clearly see the text on the AR elements in Task 0-2 due to vision issues), 80 valid, continuous data recordings remained (each 10s-150s long). These original recordings were then processed and segmented to create the final training dataset. The data preprocessing steps are summarized in [Figure](#page-5-0) 3(a):

1. Temporal Alignment. Timestamps within each recording were synchronized.

2. Filtering. EEG signals were band-pass filtered (0.5-45 Hz) [\[39\]](#page-17-28) into six components brain wave components (delta, theta, alpha, low beta, high beta, gamma). IMU data (9 components: three accelerometer, three gyroscope, three Euler angles) underwent moving average filtering [\[29\]](#page-17-29).

3. Data Normalization. Data were normalized acrossrecordings to account for individual differences [\[56\]](#page-17-30).

4. Downsampling. Given the 10-second sample length and the presence of redundant information in high-sampling-rate data [\[4\]](#page-16-8), EEG and IMU signals were downsampled to 1 Hz to reduce data dimensionality and computational complexity [\[19\]](#page-17-31).

5. Segmentation. From the 80 preprocessed recordings, we generated 10,807 training samples using a 10-second sliding window with a 1-second step. This resulted in 5,847 internal-attention and 4,960 external-attention samples. The chosen window size and step balanced the trade-off between capturing transient dynamics and maintaining data continuity, improving model robustness.

Results. A Mann-Whitney U test revealed significant differences (p < .001) in six brain waves and eight IMU components between internal and external attention states: 1) IMU Features: External attention (EA) exhibited higher acceleration on the y-axis (-9.08 vs. -9.57) and z-axis (1.95 vs. 0.00), as well as greater roll (rotation about the x-axis; -1.20 vs. -1.52) angles. Conversely, EA showed lower x-axis acceleration (-0.62 vs. -0.24), lower angular velocities

<span id="page-4-0"></span>[<sup>1</sup>https://www.microsoft.com/en-us/hololens/buy](https://1https://www.microsoft.com/en-us/hololens/buy)

<span id="page-4-1"></span><sup>2</sup>https://brainco.tech/#/product/oxyzen

AttentionAR: Attention-Gated MLLM Reasoning for AR Safety UIST '25, September 28–October 01, 2025, Busan, Republic of Korea

<span id="page-5-0"></span>![](_page_5_Figure_2.jpeg)

Figure 3: Attention Modeling Process. (a) Data preprocessing, (b) attention model training and prediction.

(as measured by the gyroscope) around the x-axis (-0.09 vs. -0.01) and y-axis (-0.11 vs. 0.05), and lower pitch (rotation about the yaxis; -0.15 vs. -0.12) and yaw (rotation about the z-axis) angle (- 0.33 vs. -0.12) (note: yaw, pitch, and roll are computed from the headband's IMU Euler angles). No significant difference was found in z-axis angular velocity. These findings suggest that external attention involves more pronounced motion responses, except for z-axis angular velocity, which may contribute less to attention classification. 2) EEG Features: EA exhibited lower power in all six brain wave bands: delta (17.50 vs. 93.90), theta (8.26 vs. 37.5), alpha (5.01 vs. 21.30), low beta (4.24 vs. 22.8), high beta (4.54 vs. 19.90), and gamma (3.90 vs. 19.70). This suggests reduced deep cognitive processing (e.g., memory, reasoning, high-frequency information integration) during EA compared to IA, aligning with previous findings [\[64\]](#page-18-13).

Findings. Our analysis reveals that internal attention and external attention exhibit distinctly different signal distributions across most dimensions, underscoring marked differences in the underlying physiological and motor responses. In external attention, EEG power across all frequency bands—including delta, theta, alpha, low beta, high beta, and gamma—is notably lower than that of internal attention. This decreased power suggests a reduction in deep cognitive processing functions such as memory, reasoning, and high-frequency information integration, in line with previous findings [\[64\]](#page-18-13). Meanwhile, the IMU data show that external attention produces stronger motor responses in some respects; for instance, subjects demonstrate higher acceleration on the y and z axes and greater roll (rotation about the x-axis) compared to internal attention. At the same time, measures such as acceleration on the x-axis, certain angular velocities (around the x and y axes), and the pitch and yaw angles display lower values. These differences imply that subjects adopt different movement strategies when processing external stimuli, resulting in more variable and diverse signal distributions.

Using all 15 dimensions for model training rather than selecting only those features that are individually significant has clear advantages. This comprehensive approach captures the full range of feature interactions that could reveal subtle patterns not apparent when features are considered in isolation [\[59\]](#page-18-28). It also minimizes the impact of noise from any single dimension, thereby reducing the risk of overfitting [\[59\]](#page-18-28) and facilitating the development of a

more robust and interpretable multimodal classifier. Overall, these findings provide important insights into how internal and external attention states are manifested in neural and motor signals, and they lay a solid theoretical foundation for further advancements in multimodal data integration and attention classification.

#### 3.3 Attention Modeling

We modeled attention using imbalanced learning algorithms [\[35\]](#page-17-32), long short-term memory (LSTM) networks[\[36\]](#page-17-33), and cross-attention mechanisms [\[89\]](#page-18-29) with physiological signals.

Feature Extraction (see [Figure](#page-5-0) 3b). We designed two Bidirectional LSTMs (BiLSTM) [\[103\]](#page-19-2): One for EEG data [\[3\]](#page-16-9), which processes six brain wave features per time step over a 10-second window. One for IMU data [\[26\]](#page-17-34), which processes nine components to capture sequential dependencies and generate hidden states.

Cross-Attention Mechanism (see [Figure](#page-5-0) 3b). We employed a bidirectional cross-attention mechanism [\[100\]](#page-18-30) to enhance EEG-IMU information fusion.

$$
Attn(E, I_i) = \sum_{i=1}^{N} softmax\left(\frac{E, W_Q, (I_i, W_K)^T}{\sqrt{d}}\right)I_i, W_V
$$
 (1)

where represents EEG samples (queries), represents IMU samples(keys and values), and ,, are learnable projection matrices.

Fusion and Classification. Cross-attention outputs were meanpooled, concatenated into a single representation, and processed through a fully connected layer with ReLU, dropout, and layer normalization.

Training Configuration. The model was implemented in Py-Torch (learning rate = 1e-4, batch size = 64, seed = 5000) using the Adam optimizer (weight decay = 1e-4). The dataset was partitioned into 80% for training and 20% for testing. Within the 80% training partition, we utilized early stopping (patience=20), which concluded at epoch 165, to prevent overfitting.

Result. Our method, which wasinspired by [\[37\]](#page-17-35), achieved 94.36% accuracy and 93.79% F1-score for user attention classification, outperforming both ablation setups: the cross-attention-only variant reached 92.69% accuracy and 92.04% F1-score, and the LSTM-only

<span id="page-6-0"></span>Table 1: Performance Comparison of Ablation Experiments and Existing Methods

| Method                           | Accuracy | F1 Score |  |  |  |  |  |  |
|----------------------------------|----------|----------|--|--|--|--|--|--|
| Comparison with Existing Methods |          |          |  |  |  |  |  |  |
| LSTM + Cross-Attention (Ours)    | 0.9436   | 0.9379   |  |  |  |  |  |  |
| SVM (RBF Kernel) [22]            | 0.8113   | 0.7524   |  |  |  |  |  |  |
| LDA [90]                         | 0.7382   | 0.6515   |  |  |  |  |  |  |
| Logistic Regression [22]         | 0.7179   | 0.6494   |  |  |  |  |  |  |
| Ablation Experiment              |          |          |  |  |  |  |  |  |
| Cross-Attention only             | 0.9269   | 0.9204   |  |  |  |  |  |  |
| LSTM only                        | 0.9260   | 0.9172   |  |  |  |  |  |  |

variant obtained 92.60% accuracy and 91.72% F1-score. These improvements suggest that the combination of LSTM with crossattention effectively captures temporal and contextual relationships in the data. In contrast, traditional machine learning methods tailored for user attention classification—such as Linear Discriminant Analysis (LDA) [\[90\]](#page-18-9) (73.82% accuracy, 65.15% F1-score), a linear logistic regression model [\[22\]](#page-17-36) (71.79% accuracy, 64.94% F1 score), and a non-linear SVM with RBF kernel [\[22\]](#page-17-36) (81.13% accuracy, 75.24% F1-score)—demonstrate a notable performance gap. [Table](#page-6-0) 1 presents these accuracy and F1-score data. We also employed 5-fold cross-validation ( [Table](#page-7-0) 2) to assess generalization. Additionally, with device latencies of approximately 200 ms, our framework is well-suited for real-time processing.

## 3.4 Cross-Validation Data Distribution Analysis

In this section, we analyze and visualize the data distributions from two cross-validation strategies—Leave-One-Subject-Out (LOSO CV) and Leave-One-Task-Out (LOTO CV). By visualizing these distributions (in [Figure](#page-6-1) 4 and [Figure](#page-7-1) 5), we can observe commonalities and differences among subjects and tasks, as well as reveal how neural and motion signals change under different attention states. In each subplot, the horizontal axis shows a 10-second time sequence (sampled at 1 Hz) and the vertical axis represents the normalized data values. The mean curve and its surrounding standard deviation band together display the overall trend and the variability at each time point, providing a comprehensive view of the data structure and inter-feature interactions.

3.4.1 Subject-Level Consistency. In LOSO CV, we examine the common patterns and individual differences among subjects. [Figure](#page-6-1) 4 shows that most subjects' 15 features follow similar mean trends with only minor fluctuations over time, indicating high consistency across the group. However, some low-performing subjects (e.g., S1 and S10 as shown in [Table](#page-7-0) 2, with lower accuracy and F1 scores) deviate significantly in key features—especially in the yaw component of head Euler angles. Their signal distributions resemble a "blind guess" pattern [\[85\]](#page-18-31), suggesting these subjects differ notably in movement habits, recording noise, or physiological state. This deviation may prevent the model from effectively extracting features, thereby affecting prediction performance. This finding indicates

<span id="page-6-1"></span>![](_page_6_Figure_7.jpeg)

Figure 4: Subject-level normalized time series distributions (mean ± standard deviation) across 15 dimensions. This figure visually explains why the model struggles with certain individuals. Low-performing subjects (e.g., S1, S10, highlighted in red) exhibit signal distributions, particularly in the head's yaw component, that are distinctly different from the majority of other subjects (grey lines), demonstrating that poor performance is linked to observable individual differences.

that personalization is not merely an enhancement but a prerequisite for deploying such attention-aware systems effectively and equitably across a diverse user base. We should also state clearly that this variability represents a significant performance limitation of the current generalized model, as its reliability on an arbitrary new user cannot be guaranteed without such personalization.

#### 3.4.2 Task-Level Patterns. Task Correlation and Variability. In LOTO CV, we compare the data distributions of four tasks (see [Fig](#page-7-1)[ure](#page-7-1) 5):

Task 0: Internal Attention (Mental Rotation) and Task 1: Internal Attention (Mental Arithmetic) show relatively concentrated signal distributions and high accuracy (approximately 94.63% and 94.99%, respectively). Their F1 scores are 0 because both tasks contain no positive samples (all represent internal attention), so the model only needs to assign one class.

In contrast, Task 2: External Attention (Word Counting—AR UI) and Task 3: External Attention (Cup Guessing—Real World) exhibit

<span id="page-7-1"></span>![](_page_7_Figure_1.jpeg)

Figure 5: Task-level normalized time series distributions (mean ± standard deviation) across 15 dimensions. This figure validates our feature selection by showing that our chosen features contain meaningful, separable information. The clear visual separation in signal distributions between internal attention tasks (Tasks 0/1, red lines) and external attention tasks (Tasks 2/3, blue/green lines) confirms that the features are effective at capturing the high-level states we aim to model.

considerably greater dispersion in some dimensions (e.g., EEG theta and alpha bands, acceleration on the y and z axes, angular velocity on the y axis, and yaw and roll in Euler angles). Their accuracy (approximately 5.60% and 29.47%) and F1 scores (approximately 10.61% and 45.53%) are much lower. This suggests that the external attention tasks trigger EEG and IMU signals that are much more heterogeneous. Moreover, differences between Task 2 and Task 3 in certain movement and posture features (such as yaw) imply that subjects display more varied head movements when observing different external targets.

In summary, the cross-validation analyses presented in these visualizations serve to establish three distinct but related points. First, the Leave-One-Subject-Out results ( [Table](#page-7-0) 2) demonstrate that a generalized attention model is feasible but sensitive to individual differences. While the model performs well on many users, its performance drops for specific individuals (e.g., S1, S10), providing a data-driven motivation for future work on personalization. Second, [Figure](#page-6-1) 4 visually explains this phenomenon, showing that poor model performance correlates with subjects' atypical signal

AttentionAR: Attention-Gated MLLM Reasoning for AR Safety UIST '25, September 28–October 01, 2025, Busan, Republic of Korea

<span id="page-7-0"></span>Table 2: Performance of Cross-Validation Strategies

| Validation Strategy                    | Accuracy | F1 Score |  |  |  |  |  |  |
|----------------------------------------|----------|----------|--|--|--|--|--|--|
| 5-Fold Cross-Validation                |          |          |  |  |  |  |  |  |
| Fold 1                                 | 0.9514   | 0.9461   |  |  |  |  |  |  |
| Fold 2                                 | 0.9422   | 0.9355   |  |  |  |  |  |  |
| Fold 3                                 | 0.9075   | 0.8968   |  |  |  |  |  |  |
| Fold 4                                 | 0.9144   | 0.9063   |  |  |  |  |  |  |
| Fold 5                                 | 0.9479   | 0.9426   |  |  |  |  |  |  |
| Leave-One-Subject-Out Cross-Validation |          |          |  |  |  |  |  |  |
| Subject 0                              | 0.7199   | 0.6108   |  |  |  |  |  |  |
| Subject 1                              | 0.6369   | 0.2196   |  |  |  |  |  |  |
| Subject 2                              | 0.8972   | 0.8835   |  |  |  |  |  |  |
| Subject 3                              | 0.7427   | 0.6667   |  |  |  |  |  |  |
| Subject 4                              | 0.7709   | 0.7975   |  |  |  |  |  |  |
| Subject 5                              | 0.9574   | 0.9455   |  |  |  |  |  |  |
| Subject 6                              | 0.7491   | 0.6788   |  |  |  |  |  |  |
| Subject 7                              | 0.9220   | 0.9200   |  |  |  |  |  |  |
| Subject 8                              | 0.9758   | 0.9725   |  |  |  |  |  |  |
| Subject 9                              | 0.9574   | 0.9639   |  |  |  |  |  |  |
| Subject 10                             | 0.7241   | 0.4121   |  |  |  |  |  |  |
| Subject 11                             | 0.8969   | 0.9004   |  |  |  |  |  |  |
| Subject 12                             | 0.9504   | 0.9289   |  |  |  |  |  |  |
| Subject 13                             | 0.7427   | 0.6667   |  |  |  |  |  |  |
| Subject 14                             | 0.9973   | 0.9982   |  |  |  |  |  |  |
| Subject 15                             | 0.8933   | 0.8571   |  |  |  |  |  |  |
| Subject 16                             | 0.7744   | 0.7031   |  |  |  |  |  |  |
| Subject 17                             | 1.0000   | 1.0000   |  |  |  |  |  |  |
| Subject 18                             | 0.9308   | 0.9278   |  |  |  |  |  |  |
| Subject 19                             | 0.8590   | 0.8125   |  |  |  |  |  |  |
| Subject 20                             | 0.7771   | 0.7028   |  |  |  |  |  |  |
| Subject 21                             | 1.0000   | 1.0000   |  |  |  |  |  |  |
| Subject 22                             | 0.9622   | 0.9463   |  |  |  |  |  |  |
| Leave-One-Task-Out Cross-Validation    |          |          |  |  |  |  |  |  |
| LeaveOutTask0                          | 0.9463   | 0.0000   |  |  |  |  |  |  |
| LeaveOutTask1                          | 0.9499   | 0.0000   |  |  |  |  |  |  |
| LeaveOutTask2                          | 0.0560   | 0.1061   |  |  |  |  |  |  |
| LeaveOutTask3                          | 0.2947   | 0.4553   |  |  |  |  |  |  |

patterns, such as the distinct bias in the yaw component for lowperforming subjects. Third, [Figure](#page-7-1) 5 validates our feature selection, as the clear visual separation between internal (Tasks 0/1) and external attention (Tasks 2/3) confirms that our chosen features contain meaningful, separable information about the user's core attentional state.

External Attention Limits. Although subjects in external attention conditions may use different strategies when observing virtual AR elements versus real objects [\[92\]](#page-18-7), further analysis shows that, in most EEG measures as well as in acceleration on the x-axis, angular velocity on the x- and z-axes, and Euler angle pitch, the signal distributions across all tasks remain similar. This indicates that the differences between the two external attention scenarios may be mainly reflected in subtle head motion variations rather

than EEG signals. Based on these results, we speculate that using only EEG or IMU data to distinguish external attention (especially to differentiate AR interfaces from real-world objects) has its limitations. Combining additional modalities (such as eye-tracking data) may offer more comprehensive information and improve overall classification performance.

#### 3.5 External Attention Target Detection

To determine whether users were focused on AR elements or realworld objects, we utilized HoloLens 2's eye-tracking system. As shown in [Figure](#page-5-0) 3(b), we classified external attention by detecting whether the user's gaze ray intersected with AR elements, allowing for refined attention tracking.

#### 4 User Survey on Safety Risks

To gain insights into users' perceptions of safety hazards and their expectations for safety assistive systems, we conducted an online survey with 26 participants. This section outlines the survey methodology, key findings, and design implications based on the results.

# 4.1 Survey Methodology and Participant Background

We recruited 26 participants(6 female, 20 male, aged 21–47) through [redacted social media], representing diverse professions, including video editors, software engineers, teachers, concept artists, office workers, researchers, and students. Each participant completed an online questionnaire.

The survey began with an introduction to the concept of safety hazards in everyday life [\[78\]](#page-18-20), followed by three key questions:

1. When walking, what situations or factors do you think might pose a threat to your safety? (Provide at least three examples.)

2. When distracted in a hazardous environment, what potential consequences do you foresee?

3. If you find yourself in a hazardous environment while distracted, would you want a system to automatically alert you? Please explain why.

#### 4.2 Results

Two researchers analyzed the responses and identified commonalities and differences in safety risk assessments:

Common Safety Hazards: Most participants agreed that vehicles, uneven pavement (e.g., potholes, slippery surfaces, uncovered manholes), and sudden obstacles (e.g., falling objects, debris) were primary hazards. Some also mentioned fast-moving pedestrians, cyclists, and unexpected animals as additional risk factors.

Consequences of Distraction: Participants commonly expressed concerns about falling, injuries, property damage, or even lifethreatening accidents. These concerns highlight the serious consequences of external attention loss and the need for preventive measures.

Desire for Automated Alerts: While most participants favored an automatic alert system to mitigate potential risks, some worried that frequent notifications might disrupt their normal activities (P9). A few also raised privacy concerns (P15, who was concerned about camera-based monitoring).

#### <span id="page-8-0"></span>4.3 Design Implications

Based on the survey results, we propose the following design implications for an AR-based safety assistive system. A core design goal, derived directly from this user feedback, was to create a system that provides proportional warnings: the intensity of the alert should be directly proportional to the severity of the detected risk [\[86\]](#page-18-32). This principle aims to balance the need for effective safety interventions with the desire to minimize unnecessary disruptions and avoid the "alarm fatigue" mentioned by participants (P9).

Diverse Threat Recognition and Personalized Alerts. Participants identified various threats ranging from minor hazards to life-threatening dangers. The system should comprehensively detect potential hazards and adapt alert strategies based on user behavior and situational context. For high-risk scenarios (e.g., an oncoming vehicle [\[75\]](#page-18-33)), the system should issue high-priority warnings immediately. For lower-risk situations, alerts should be subtle and infrequent to minimize disruption and avoid introducing new distractions.

Risk-Level Classification Model. Based on participant feedback, we developed a three-tiered risk classification model. Information from 10 reported hazards (e.g., uneven sidewalks, crowded spaces, moving vehicles) was categorized through iterative discussions (until full agreement was reached) and coding by two researchers. The final classification is as follows:

Low Risk: 1) Definition: Hazardsthat might cause minorinjuries or brief moments of discomfort. 2) Explanation: These hazards involve subtle spatial cues and minimal interference (e.g., slight road unevenness, a stray dog crossing briefly) [\[101\]](#page-19-3). They typically result in minor inconveniences rather than serious harm.

Moderate Risk: 1) Definition: Hazards that may lead to significant injuries. 2) Explanation: These hazards are more prominent, often within the user's immediate path. For example, navigating through a crowded area increases the likelihood of accidental collisions [\[101\]](#page-19-3). While not life-threatening, they pose a moderate risk of injury if not addressed.

High Risk: 1) Definition: Hazards that pose an immediate and life-threatening danger. 2) Explanation: High-risk scenarios include clear and urgent threats, such as an oncoming vehicle in the user's path [\[75\]](#page-18-33). These require immediate intervention, as the potential for fatal injuries is high.

This classification is based on hazard intensity, urgency, and potential consequences. To validate its reliability, two researchers independently rated all remaining 15 hazard scenarios from participant feedback, achieving a high agreement (Cohen's Kappa = 0.762).

These insights provide a theoretical foundation for developing an AR safety assistive system capable of dynamically recognizing and responding to multi-level hazards while balancing warning and user experience.

#### 5 AttentionAR System

Following insights from our user survey, we developed AttentionAR, a system that integrates user attention detection with realtime environmental hazard assessment and dynamic AR adaptation to enhance user safety.

<span id="page-9-0"></span>![](_page_9_Figure_2.jpeg)

Figure 6: Overview of the AttentionAR pipeline with three modules: (1) Attention Awareness, analyzing EEG, IMU, and gaze data to detect user focus; (2) Scene Awareness, stitching 5 frames over 2 seconds and using an MLLM to predict risk level, source, and direction; and (3) AR Adaptation & Warning, dynamically adjusting AR transparency and displaying alerts to enhance situational awareness and hazard perception.

#### 5.1 4.1 Overview

The AttentionAR computational pipeline, illustrated in [Figure](#page-9-0) 6, consists of three components:

(1) Attention Awareness Module: This module collects and processes user attention data (EEG, IMU, and gaze) to determine whether the user is internally focused or paying attention to AR elements, thereby deciding when to trigger further scene analysis.

(2) Scene Awareness Module: This module utilizes an egocentric camera to capture a dynamic view of the user's environment. It stitches together 5 equally spaced frames over a 2-second interval and processes the composite image using a multimodal large language model. Through chain-of-thought reasoning, it predicts the risk level, risk source, and risk direction based on spatial cues, hazard presence, and overall severity.

(3) AR Adaptation and Warning Module: This module employs a decision tree to map the predicted risk level, risk source, and risk direction to corresponding AR adaptations and warnings. It dynamically adjusts AR overlay transparency and displays warning marks along with risk source and directional information to alert the user without overwhelming their cognitive load.

#### 5.2 Attention Awareness Module

In our research setup, AttentionAR simultaneously collects user signals using Brainco Oxyzen and HoloLens 2. Specifically, EEG and IMU data (capturing brain and head dynamics) as well as gaze information are acquired and fed directly into our attention model. The model then classifies the user's attention state (see [Figure](#page-9-0) 6(a)). When the output indicates either internal attention or external attention focused on AR elements, a trigger signal is sent from the mobile devices (HoloLens 2 and Brainco Oxyzen) to the computing center (16 GB RAM, RTX 4060) via UDP (using Python's socket

module). This signal activates the subsequent Scene Awareness Module.

#### 5.3 Scene Awareness Module

AttentionAR also incorporates an egocentric camera (Logitech Brio 90) to continuously capture real-world video streams of the user's environment (see [Figure](#page-9-0) 6(b)). We envision that future versions of AttentionAR will integrate seamlessly with lightweight, wearable AR glasses or head-mounted displays (HMDs) equipped with a broad array of sensors (e.g., RGBD cameras [\[21\]](#page-17-37), microphones [\[61\]](#page-18-15), physiological sensors [\[97\]](#page-18-10), eye trackers [\[97\]](#page-18-10), face trackers [\[69\]](#page-18-34) and IMUs) to provide richer and more comprehensive contextual data.

When triggered, the Scene Awareness Module immediately captures five equally spaced frames within a 2-second interval. These frames are then concatenated into a composite image that encapsulates 2 seconds of dynamic scene information. This timing setup draws inspiration from [\[10\]](#page-16-2) to ensure a balance between information richness and system processing time. However, considering the urgency of our task, we have set the interval shorter than the 5 seconds used in [\[10\]](#page-16-2). This composite image is processed by a multimodal large language model (MLLM) employing a chain-ofthought (CoT) prompting strategy to predict the scene's risk level, risk sources, and risk direction. The prediction results are then transmitted back to the HoloLens 2 via UDP from the computing center.

5.3.1 Reasoning. AttentionAR determines the safety risk of the current scene by directly analyzing the visual data within approximately 3-5 seconds. Specifically, a first-person perspective image is analyzed using CoT prompting (as described in [\[94\]](#page-18-35)) with GPT-4o[3.](#page-9-1)

<span id="page-9-1"></span>[<sup>3</sup>https://openai.com/index/hello-gpt-4o](https://3https://openai.com/index/hello-gpt-4o)/

#### UIST '25, September 28–October 01, 2025, Busan, Republic of Korea Pei, et al.

<span id="page-10-0"></span>![](_page_10_Picture_1.jpeg)

Figure 7: Movement Video Processing and Analysis. (a) Pipeline: Selected 10 videos ( 2 hrs) from HUJI EgoSeg, segmented into 200 clips, and processed single/multi-frame inputs for annotation and MLLM risk evaluation. (b) Location Distribution: Sample counts across different settings. (c) Failure Cases: Examples of incorrect risk predictions.

The CoT approach guides the model through intermediate reasoning steps—evaluating spatial cues, the presence of hazards, and overall severity—to generate the final output (risk level, risk source, and risk direction). Previous studies [\[52,](#page-17-19) [61\]](#page-18-15) first converted images into textual descriptions (e.g., scene descriptions and user activities) before inputting them to a language model. However, this two-step process may lose important spatial and dynamic details. In contrast, our method directly processes the composite image with the MLLM, thereby preserving all relevant information. The prompt consists of an Instruction, Few-shot Examples, and the Current Context (i.e., the composite image). (See [Figure](#page-9-0) 6(b) and Appendix A for further details.)

Instruction. A prefix that clarifies the definitions of our three level scale risk, as outlined in [subsection](#page-8-0) 4.3, supplementary guidelines, and the task.

The supplementary guidelines:

"1) The image is a first-person view, all people in the image are bystanders. 2) Identify dynamic hazards (e.g., distracted pedestrians, animals, or moving objects) that could cause collisions. 3) Detect static hazards such as obstacles, stairs, or uneven surfaces. 4) Consider the user's activity (e.g., walking, climbing stairs, standing). 5) The image is a composite of 5 frames stitched horizontally (captured within 2 seconds, with each frame numbered at the top-left) and may include user movement. 6) Analysis order for risk source, risk direction, and risk level: Step 1:... 7) All responses for risk source, risk direction, and risk level must be in lowercase."

The task is described as follows:

"Please examine the provided first-person view composite image and assess any potential safety hazards you observe. Identify both dynamic hazards (such as approaching people or vehicles) and static hazards (like obstacles or uneven surfaces), classify them by risk level as described, and based on all frames, determine whether the risk source(s) appears on the left, right, or both sides of the user's view. Provide your answer in the specified format."

Few-shot Examples. Three few-shot examples are provided, each comprising an input, a chain-of-thought, and an output. We selected three examplesrepresenting distinctrisk scenariosin urban environments: one where a vehicle obstructs a pedestrian crossing [\[75\]](#page-18-33), another where no obvious hazard is detected, and a third involving an inattentive pedestrian [\[101\]](#page-19-3). In each case, the input is presented as a stitched image capturing the scene, while the chain-of-thought outlines the intermediate reasoning steps that the

model should follow to evaluate the situation based on spatial cues, hazard presence, and overall severity.

To construct the chain-of-thought, we define a step-by-step reasoning process that systematically evaluates the key elements of the scene: the level of risk, the source of the risk, and its directional attribute. For example, in the first scenario, the reasoning assesses how a car blocking the pedestrian crossing on the right directly endangers pedestrians, leading to a high-risk designation. In the second scenario, the reasoning finds that no obvious hazard is present; therefore, the risk level is low, with both risk source and risk direction set to "none." In the third example, subtle cues—such as an inattentive pedestrian—are analyzed to determine their potential hazard and directional positioning. This guided process ensures that the final outputs (riskLevel, riskSource, and riskDirect) are derived from a clear and structured evaluation of the scene.

Current Context refers to the stitched image of a scene constructed from 5 first-person view frames captured at equal intervals within a 2-second period [\[10\]](#page-16-2).

Output Format Consistency. Because prediction outputs can fluctuate [\[61\]](#page-18-15), we ensure the output format remains consistent by requiring the model to conform to a specific structure:

"Please start answering after all the questions (Q) with 'A: Let's think step by step. Reasoning: XXX. riskLevel=XXX, riskSource=XXX, riskDirect=XXX. [ANSWER COMPLETED]'."

#### 5.4 AR Adaptation and Warning Module

In the AR Adaptation Module, a decision tree is employed to map the predicted risk level, risk source, and risk direction to appropriate AR adaptations and warnings. To mitigate the potential occlusion of real-world information by AR content [\[15\]](#page-17-38), we adjust the transparency of the AR overlay based on the risk level. In parallel, to enhance situational awareness, warning marks [\[5\]](#page-16-1), along with explicit indicators of the risk source and its direction [\[11\]](#page-16-10), are superimposed on top of the AR elements. These warning elements are designed to be positioned closer to the user than the AR content, ensuring they are highly noticeable.

[Figure](#page-9-0) 6(c) illustrates our decision tree rules: 1) For risk level 1, the AR transparency is set to 75% and no warnings are displayed. 2) For risk level 2, the AR transparency is set to 50%, and warning icons along with risk source and direction indicators are shown, and the generation of new AR content is paused. 3) For risk level

3, the AR transparency is reduced to 25%, with the same warning information displayed in level 2 .

# 6 Technical Evaluation with Movement-Related Videos

We evaluated AttentionAR on 200 clips from a set of 20 walkingrelated egocentric video recordings under 13 different locations. We report the accuracy (mean absolute error and classification accuracy) of our system on risk level predictions.

#### 6.1 Materials

Our sample was sourced from HUJI EgoSeg[\[72\]](#page-18-36) [4,](#page-11-0) an extensive egocentric dataset with over 65 hours of daily-life walking activity videos, recorded both outdoors and indoors. [Figure](#page-10-0) 7(a) shows the complete data processing procedure. We manually selected 10 videos related to walking and stair climbing, totaling about 2 hours. To evaluate the generalization ability of AttentionAR across various walking scenarios and its effectiveness in discriminating risks in different environments, we randomly selected 200 non-overlapping 2-second intervals from these videos, forming 5 frames per video clip. The first frame from each set was also extracted and compiled into the control group. Simultaneously, the 5 frames from each group were horizontally concatenated in chronological order to create a composite image with spatiotemporal information, forming the experimental group. A total of 400 test samples were generated, consisting of both experimental and control groups.

Additionally, to standardize the video frame sizes and reduce the computational load of the MLLM, all video frames were resized to 640×480 [\[61\]](#page-18-15). Our final sample comprised 13 distinct locations (shown in [Figure](#page-10-0) 7(b), with the first 9 locations displayed), including parks, stairs/steps, covered walkways, open plazas, offices, streets, lawns, restaurants, and hallway corridors in academic buildings, among others. We ran AttentionAR on all test samples, logging various data points such as LLM reasoning output, and predictions of risk level, risk source, and risk direction.

#### 6.2 Data Annotation

The researchers first discussed and finalized the risk source and risk direction annotations for the 200 experimental images.

Risk Source: If no obvious risk source was observed, the image was labeled as "none."

Risk Direction: The vertical centerline of the image was used to delineate left and right. A "middle" category was not included because prior research has shown that the MLLM reliably distinguishes between left and right[\[33\]](#page-17-39). Defining a middle category would require an arbitrary threshold, complicating annotation consistency.

Control Group Alignment: The risk source and direction annotations for the 200 control images were set to match those of their corresponding experimental images.

Once risk source and direction were determined, the two researchers independently evaluated and assigned risk levels to the 400 images. Consistent with our findings in [subsection](#page-8-0) 4.3, interrater agreement on risk level classification was high (Cohen's Kappa

 = 0.815). Discrepancies were discussed and resolved, resulting in the final dataset distribution: 1) 1.5% labeled as "3" (high risk). 2) 36.5% labeled as "2" (moderate risk) 3) 62.0% labeled as "1" (low risk).

This imbalanced distribution likely reflects the natural occurrence of hazards in everyday walking scenarios—severe risks (level 3) are inherently rare, whereas moderate (level 2) and low risks (level 1) are more common. However, this does not negatively impact our evaluation, as our methodology and metrics are designed to accommodate such variations.

To assess whether the MLLM interprets multi-frame and singleframe representations differently, we controlled for annotation variability by assigning identical risk labels (e.g., levels, sources, and directions) to both the 200 single-frame images in the control group and the 200 stitched images in the experimental group.

#### 6.3 Metrics

We assess AttentionAR using two quantitative metrics: (1) Mean Absolute Error (MAE): This metric measures the average absolute difference between predicted risk levels and the ground truth across all risk level categories. Given the ordinal nature of our data (where misclassifying "Low Risk" as "Moderate Risk" is less severe than misclassifying "Low Risk" as "High Risk"), MAE provides a nuanced error representation. Risk levels are numerically mapped to integer values ranging from 1 (Low) to 3 (High). (2) Averaged Classification Accuracy (ACC): To complement MAE, we report classification accuracy to intuitively assess performance in predicting risk levels, sources, and directions.

#### 6.4 Results

We evaluated our system's performance in predicting risk attributes using both 5-frame stitched images and single-frame images, assummarized in [Table](#page-12-0) 3. For risk level predictions, the models achieved MAEs ranging from 0.19 to 0.32 and accuracies between 63% and 82% when using five-frame inputs. However, with single-frame inputs, the models exhibited higher MAEs, ranging from 0.27 to 0.43, and lower accuracies between 55% and 74%. Notably, Qwen-VL-Max attained the best risk level performance on 5-frame inputs with an MAE of 0.19 and an accuracy of 82%, while GPT-4o demonstrated robust results with an MAE of 0.23 and an accuracy of 78%.

Beyond serving as visual warning cues, the risk source and direction annotations also acted as auxiliary indicators for validating the MLLM's risk level predictions. Notably, although Qwen-VL-Max achieved the highest risk level accuracy, its performance in predicting risk source (65% vs. 81% for GPT-4o) and risk direction (56% vs. 76% for GPT-4o) was lower. This suggests that GPT-4o is more reliable in spatially and directionally assessing risks, thereby enhancing comprehensive hazard evaluation.

For risk source and risk direction predictions, the models also exhibited stronger performance with five-frame inputs compared to single-frame inputs. For instance, GPT-4o achieved 81% and 76% accuracy, respectively, on risk source and risk direction with 5-frame inputs, but only 60% and 55% accuracy, respectively, with singleframe inputs. These results indicate that our system effectively captures complex risk-related information and that multi-frame

<span id="page-11-0"></span><sup>4</sup>https://vision.huji.ac.il/egoseg/videos/dataset.html

| MLLM             | Risk Attribute | 5 Frames |      | Single Frame       |      |      |                    |
|------------------|----------------|----------|------|--------------------|------|------|--------------------|
|                  |                | MAE      | ACC  | Inference Time (s) | MAE  | ACC  | Inference Time (s) |
| GPT4o[38]        | Risk Level     | 0.23     | 0.78 |                    | 0.27 | 0.73 |                    |
|                  | Risk Source    | -        | 0.81 | 5.27               | -    | 0.60 | 5.09               |
|                  | Risk Direction | -        | 0.76 |                    | -    | 0.54 |                    |
| GPT4o-mini       | Risk Level     | 0.32     | 0.68 |                    | 0.40 | 0.60 |                    |
|                  | Risk Source    | -        | 0.64 | 4.68               | -    | 0.55 | 4.27               |
|                  | Risk Direction | -        | 0.43 |                    | -    | 0.39 |                    |
| LLaMA-3.2-Vision | Risk Level     | 0.30     | 0.63 |                    | 0.43 | 0.55 |                    |
|                  | Risk Source    | -        | 0.45 | 5.45               | -    | 0.42 | 5.34               |
|                  | Risk Direction | -        | 0.39 |                    | -    | 0.41 |                    |
| Qwen-VL-Max[8]   | Risk Level     | 0.19     | 0.82 |                    | 0.28 | 0.74 |                    |
|                  | Risk Source    | -        | 0.65 | 15.12              | -    | 0.54 | 14.34              |
|                  | Risk Direction | -        | 0.56 |                    | -    | 0.50 |                    |

<span id="page-12-0"></span>Table 3: Performance of MLLMs in risk assessment, comparing multi-frame (5 frames) and single-frame inputs. Metrics include Mean Absolute Error (MAE), Classification Accuracy (ACC), and Inference Time.

representations generally yield lower MAEs and higher accuracies than single-frame inputs.

For instance, in a multi-frame image, a pedestrian approaching the user may be correctly identified as a moderate risk, whereas in a single-frame image, the same pedestrian might be misinterpreted as a stationary figure, leading to a low risk assessment. This gap suggests that the additional spatial and temporal context provided by multi-frame inputs allows MLLMs to better understand scene dynamics and assess potential safety hazards more accurately [\[66\]](#page-18-19).

#### 6.5 Latency

We also assessed the latency of our inference pipeline, which computes risk level, source, and direction in a single pass. The total inference times ranged from approximately 4.27 seconds (GPT4omini with single-frame inputs) to 15.12 seconds (Qwen-VL-Max with 5-frame inputs). Although the multi-frame inputs tend to incur slightly higher processing times than the single-frame ones, the additional latency is justified by the richer spatiotemporal context they provide. Importantly, these inference times remain within acceptable limits for real-time risk assessment in dynamic environments, where hazards typically persist over longer durations. This balance between prediction accuracy and computational efficiency underscores the practical viability of our approach.

Overall, considering the combined performance in terms of MAE, ACC, and latency, GPT4o emerges as the most balanced model. Its robust risk level predictions coupled with acceptable inference times make it the optimal choice for our system.

#### 6.6 Failure Cases Analysis

Our analysis revealed several challenges in accurately predicting risk level and risk source, see failure cases in [Figure](#page-10-0) 7(c). In multiple instances, misinterpretations of the scene resulted in low-risk situations being erroneously classified as moderate risk. For example, a tilted camera angle led the model to interpret a flat road as a slope, and reflections on the ground were mistaken for indications of a wet surface—both causing a shift from low to moderate risk.

Additional failure cases highlight issues with reflective surfaces and distance perception. In one instance, the model misinterpreted a reflection in a glass window by mistaking the reflected image of the user for an oncoming pedestrian, thereby escalating the risk level. Similarly, a distant person was incorrectly identified as being close, further contributing to the overestimation of risk.

These failure cases underscore the complexities inherent in interpreting dynamic real-world environments from multi-frame inputs. They highlight the need for improved spatial calibration and context-aware analysisto better handle ambiguous visual cues,such as reflections and camera tilt. Future enhancements to the system should focus on refining these aspects to achieve more consistent and accurate risk assessments.

#### 7 Experiencing AttentionAR in Real-time

While our focus remains on the detection of risk in the scene, we conducted an additional study to understand users' integrated experiences when AttentionAR is employed to enable common interface adaptation and warning strategies.

#### 7.1 Procedure

We conducted a user study with AttentionAR to understand its potential and challenges for real users in assisting them in realtime hazard detection and risk response during various everyday mobility scenarios. The study setup involved an egocentric camera (Logitech Brio 90), an AR HMD (Hololens 2) for adaptive and warning displays, and a Brainco Oxyzen device for EEG capturing.

AttentionAR: Attention-Gated MLLM Reasoning for AR Safety UIST '25, September 28–October 01, 2025, Busan, Republic of Korea

<span id="page-13-0"></span>![](_page_13_Figure_2.jpeg)

Figure 8: Real-World Validation Experiment Setup.

Ten participants were recruited from a university, representing diverse academic backgrounds (undergraduate, master's, and PhD). Their ages ranged from 20 to 30 years (mean = 24.9, standard deviation = 3.78), and three of the participants were female. These participants did not overlap with those described in [subsection](#page-4-3) 3.1. Additionally, 30% of the participants had prior experience with AR wearables.

Participants first familiarized themselves withAttentionAR. They then simulated two scenarios in indoor or outdoor spaces (see [Fig](#page-13-0)[ure](#page-13-0) 8): climbing stairs (indoor, scenarios 1) and walking on a narrow road (outdoor, scenarios 2) . Scenarios were selected to represent varying hazards encountered during everyday mobility, ranging from static hazards (e.g., steep staircases in scenario 1) to dynamic threats(e.g., oncoming pedestrians distracted by their phonesin scenarios 2). During each scenario, a path approximately 8-10 meters long was defined with a designated start and end point. Participants, while wearing the Hololens 2, were asked to watch an engaging video (Mr. Bea[n5\)](#page-13-1), which appeared as an AR element that moved along with their field of view (developed based on AUIT[\[25\]](#page-17-16)), as they moved from the start to the end. Additionally, to further increase user engagement, we will inform participants in advance that they will be asked questions related to the video content after the task.

We designed corresponding adaptation and warning strategies on AttentionAR to provide timely adaptations and warnings when risks were detected. For example, if user attention was detected to be diverted from the real world (either internally focused or on AR content), AttentionAR would automatically assess the scene's hazard level, source, and direction. It would then adjust the transparency of AR elements to reduce occlusion of the real scene and simultaneously issue a warning indicating the hazard's source and direction. Each scenario was conducted with and without AttentionAR assistance in a within-subject design, and the order of the conditions was counter-balanced across participants to mitigate potential learning effects. All participants experienced two scenarios both with (w/) and without (w/o) AttentionAR. When AttentionAR was activated, participants followed the provided adaptation and warning strategies to modify their navigation behavior in response to hazard alerts. When AttentionAR was deactivated, they were

<span id="page-13-2"></span>![](_page_13_Figure_8.jpeg)

Figure 9: Paired t-test of subjective and objective measures between conditions with and without AttentionAR. Significant differences are marked with stars.

asked to rely solely on their natural perception and judgment for hazard detection and route navigation.

In evaluating our system's effectiveness, we employed both objective and subjective measures during and after each scenario. Objective data encompassed the time users required to complete their movements. Subjectively, participants assessed system safety using a 7-point Likert scale, responding to statements like "The system is safe (safety perception)" and "The system reliably mitigates potential hazards (risk mitigation)" (Cronbach's = .890). They also evaluated situational awareness with items such as "The system enhanced my overall situational awareness (situational awareness)" and "I could accurately assess the direction and source of potential hazards using the system (risk identification)" (Cronbach's = .852). Detailed scales are provided in Appendix B. Additionally, we conducted semi-structured interviews to gather qualitative feedback on participants' experiences.

#### 7.2 Results

Enhanced Safety and Risk Mitigation. Participants reported a significant improvement in perceived safety and risk mitigation when using AttentionAR. Ratings for system safety—assessed via statements such as "The system is safe" and "The system reliably mitigates potential hazards"—increased from a mean of 3.25 in the unassisted condition to 5.10 with AttentionAR (p < 0.001 via Wilcoxon signed-rank tests). Similarly, ratings for risk mitigation improved from 2.85 to 5.15 ( [Figure](#page-13-2) 9). These findings suggest that the real-time warnings and clear visual cues provided by AttentionAR instill greater confidence in users, allowing them to more effectively manage and respond to potential hazards during navigation.

Improved Situational Awareness and Risk Identification. AttentionAR also had a marked positive impact on users'situational awareness and their ability to identify risks. Participants' ratings for overall situational awareness rose from a mean of 2.75 without

<span id="page-13-1"></span><sup>5</sup>https://www.youtube.com/watch?v=9LhLjpsstPY&ab\_channel=MrBean

the system to 4.75 with AttentionAR (p < 0.001 via Wilcoxon signedrank tests), while risk identification ratings increased from 2.90 to 4.45. This enhanced performance indicates that the dynamic AR overlays, which display the hazard's source and direction, enable users to better understand and interpret their environment, leading to more accurate hazard assessments in both indoor and outdoor settings.

Task Completion Time Trade-offs. Although the completion time did not show a significant difference between conditions—averaging 49.65 seconds without AttentionAR and 51.45 seconds with it—the slight increase observed in the AttentionAR condition (from 49.65s to 51.45s) is not an indicator of inefficiency. On the contrary, we interpret this 1.8-second difference as a positive behavioral outcome and a measurable indicator of our system's success. This extra time represents a valuable "safety investment," where users consciously paused to read and process our contextrich warnings before re-evaluating their physical surroundings. This very act of investing time in safety is precisely what led to the significantly higher scores in Situational Awareness and Perceived Safety.

System Latency and User Perception. During our study, the typical end-to-end system latency was approximately 5–7 seconds, composed of data capture ( 2s), network transmission ( 200-300ms), and MLLM inference ( 3-5s for GPT-4o). Our qualitative analysis provides key insights into the user's perception of this delay. One participant (P2) did mention that the delay was "noticeable" in the more complex outdoor scenario. However, the majority of participants did not report the latency as a significant drawback. Instead, their feedback focused on the system's benefits in enhancing situational awareness. This positive subjective feedback is strongly supported by the quantitative results, where scores for Safety Perception and Risk Mitigation were significantly higher. This suggests that for the developing and persistent hazard scenarios tested, the system's typical 5–7 second delay was within a perceptually acceptable range, as the benefit of receiving a deep, context-aware safety analysis appeared to outweigh the perceptible, but not prohibitive, delay.

User Feedback and Interface Customization. Semi-structured interviews provided rich insights into participants' perceptions of the system interface. Most participants(P4-5, P7-10) generally found the detection of hazard sources to be relatively accurate. However, a closer examination revealed some nuances. Several participants commented on the accuracy of the system's hazard source detection: P1 observed that "indoor monitoring was more accurate than outdoor monitoring," while P2 noted, "hazard sources were accurately detected indoors, but there was a noticeable delay in outdoor detection." We speculate that these differences may stem from variations in environmental lighting [\[68\]](#page-18-37) and other outdoor conditions, as well as hardware limitations such as camera performance. Such factors can affect the clarity and consistency of images captured indoors versus outdoors, ultimately influencing the MLLM's ability to accurately interpret the scene information [\[82\]](#page-18-38).

Regarding the visual interface, general approval was evident. For example, P1 commented, "The overall interface was good," and similar positive views were shared by P3, P9, and P10. P5 also stated, "The system's reminders were helpful; once the AR elements were adjusted to be more transparent, I could observe the real world

more clearly," underscoring the importance of balancing visual enhancements with real-world visibility. Specific recommendations for refinement also emerged. P2 suggested, "The hazard source arrow could be directed more precisely—perhaps indicating a leftup direction instead of just left." Additionally, P4 pointed out,"There is noticeable lag in the AR elements when my view shifts rapidly."

Feedback on system reminders was mixed. While many participants (P2, P4-6, P8-10) found the alerts beneficial, some indicated that the warnings occasionally disrupted their natural interaction flow. For instance, P3 mentioned that the alerts were "somewhat distracting," and P7 expressed a negative view, stating, "Since the AR video isn't important, I don't mind being a bit distracted," thereby preferring not to have automatic reminders in that context.

#### 8 Discussion and Future Work

On the Necessity of the Attention Awareness Module. A primary concern is whether the attention sensing module is necessary, or if a simpler trigger (e.g., gaze-based) would suffice. We argue that this module is not only necessary but fundamental to the system's core value for two critical reasons: enabling computational efficiency and ensuring a superior user experience by preventing "alarm fatigue" and addressing "inattentional blindness."

First, from a computational efficiency perspective, the attention module acts as an intelligent trigger. Continuously running the MLLM for scene analysis would be computationally expensive—our own analysis in [Table](#page-12-0) 3 shows a single inference takes between 5-15 seconds—and would rapidly drain the battery of a mobile AR device, rendering it impractical. The Attention Awareness module serves as an intelligent and efficient gate, ensuring that the expensive MLLM analysis is triggered only when it is most needed: when the user's attention is disengaged from their surroundings.

Second, and more critically, from a user experience perspective, the module acts as a smart filter to prevent "alarm fatigue"[\[18\]](#page-17-41), a well-documented HCI challenge where users become desensitized and eventually ignore a system that produces frequent, low-utility alerts. A system that constantly flags hazards a user is already aware of would be ignored or disabled. While a simpler gaze-based trigger can detect overt distraction (i.e., not looking at the environment), our EEG+IMU approach is vital for countering the far more perilous "inattentional blindness" or "Looked-But-Failed-To-See" (LBFTS) phenomenon [\[93\]](#page-18-25). In LBFTS scenarios, a user's eyes are directed at a hazard, but their cognitive attention is elsewhere (e.g., mind-wandering). A gaze-only system would fail completely in this common but dangerous state, offering a false sense of security precisely when the user is most vulnerable.

While our work establishes the feasibility and value of the integrated system, we acknowledge that a key limitation of the current study is the lack of an empirical dissection of each module's independent contribution to user behavior. Our primary focus was on demonstrating the viability of the novel, holistic pipeline as a proof-of-concept.

To empirically validate these distinct contributions, we acknowledge that an ablation study is the ideal approach. A valuable direction for future work, therefore, is to conduct a study comparing three conditions: (1) No Assistance (baseline), (2) a Gaze-Only Triggered System (where MLLM analysis is triggered only by sustained

gaze on AR elements), and (3) the full AttentionAR System. This will allow us to quantitatively dissect the influence of each component on user safety and behavior.

Multimodal Sensing Limitations. Our experiments for collecting attention modeling data successfully integrated EEG, IMU, and eye-tracking information. However, the overall prediction performance still has room for improvement, particularly in samples where certain modalities contain noise or insufficient information (e.g., anomalous yaw component readings in motion data for some subjects). This was especially evident in the Leave-One-Subject-Out Cross-Validation (LOSO CV) analysis, where unique movement patterns of certain participants (P1, P10) impacted the model's generalizability. Inspired by the approach in [\[59\]](#page-18-28), their multiplicative combination strategy could automatically reduce the contribution of noisy modalities to the final loss, thereby mitigating the risk of overfitting.

Furthermore, given that the two external attention-inducing tasks (AR UI vs. Real World) in the Leave-One-Task-Out Cross-Validation (LOTO CV) showed differences in certain modalities (especially IMU signals) while EEG signals offered less discriminability, future work could explore joint probability modeling or methods based on adaptive modal weighting. This would allow for a more fine-grained classification and prediction of external attention, helping to more accurately distinguish the signal effects of different external attention strategies and thus enhancing model robustness across diverse tasks and individuals.

Risk Assessment & Adaptive Warnings. While the current risk assessment and warning system can identify environmental safety hazards, as demonstrated in the experiment validating MLLM effectiveness for scene risk inference, existing methods typically handle risk assessment and attention state monitoring separately. For instance, relying solely on a trained attention classification model to determine user distraction overlooks the intrinsic link between specific risk attributes (e.g., hazard location, type, severity) and the user's specific focus of attention. This separation prevents the system from dynamically adapting its warning strategy based on whether the user is already aware of, or oriented towards, a particular hazard. For example, the system may struggle to differentiate between needing a strong directional cue to capture the attention of an unaware user versus providing a simple confirmation to a user who has already noticed the risk [\[79\]](#page-18-39).

Precisely because of this lack of attention-based contextual adaptation, the system exhibits suboptimal performance in certain realworld hazardous situations. This is corroborated by findings from the real-world system evaluation experiment: user feedback (participants P2, P4) mentioned issues such as ambiguous warning directions (the system failed to provide sufficiently precise guidance relative to the user's gaze) and perceived response delays (warnings might seem untimely or ineffective because they don't align well with the user's current attentional state). These issues underscore the necessity of integrating risk and attention information for synergistic decision-making.

To overcome this limitation, it is necessary to leverage large language models (LLMs) for a joint analysis of scene risk attributes (from MLLM assessment) and user attention states (from multimodal sensing) to construct a flexible and adaptive warning system. This approach may offer advantages over relying solely on an attention classification model, potentially providing better information fusion and real-time responsiveness to dynamic environments and user states. Concurrently, incorporating solutions that combine eye tracking, contextual memory, and multimodal feedback [\[9\]](#page-16-12) holds promise for improving the precision and timeliness of warnings, enhancing the system's responsiveness to individual user needs, and addressing the directionality and latency issues raised in user feedback.

MLLM Trade-offs & Latency. While the current fusion inference using 5 frames provides essential spatio-temporal context [\[66\]](#page-18-19), we agree that such delays are unacceptable for scenarios requiring instantaneous reactions (e.g., a rapidly approaching vehicle), a point we now clarify. Our system's primary contribution is not to replace fast, reactive detectors but to explore a new paradigm of proactive, context-aware risk assessment for developing hazardous situations. The goal is to move beyond simple object detection towards a deeper understanding of situations where analytical depth is more valuable than raw speed. That said, to address this limitation, we propose a future hybrid system: one that integrates fast, low-level detectors for immediate, reflexive warnings, while our MLLM-based reasoning module runs in the background to provide continuous, high-level assessment of developing hazards. This tiered approach would offer both immediate protection and deep situational awareness.

AR Adaptation & Visual Coverage. The current system primarily addresses occlusion in AR adaptation by increasing the transparency of AR elements, as experienced by participant P5 in the real-world system evaluation experiment. However, this method only partially resolves the issue of obscuring critical real-world cues, as it lacks the capability for dynamic repositioning based on real-time environmental context and user state [\[58\]](#page-18-40).

Simultaneously, the inherent limitation of the user's first-person perspective means that potential hazards outside the immediate field of view (e.g., threats from the periphery or behind) may not be detected promptly, leading to incomplete visual coverage. To overcome this limitation, future systems should consider integrating additional external sensors—such as peripheral cameras [\[31\]](#page-17-42) to broaden the perceptual range—and combining them with predictive models [\[28,](#page-17-43) [66\]](#page-18-19) to infer dangers beyond the direct line of sight, thereby providing a more comprehensive situational understanding. Furthermore, intelligently repositioning AR overlays based on real-time environmental analysis to place information in areas less likely to obstruct critical visual cues [\[25,](#page-17-16) [57\]](#page-17-17) will help supplement risk information within the user's view while ensuring the visibility of essential real-world elements, ultimately building a safer and more practical context-aware platform.

Personalized AR Adaptation. Current AR adaptation and warning strategies are relatively fixed, struggling to flexibly respond to the varying demands of dynamic real-world scenarios concerning risk levels and user attention states (the complexity of which was evident from the attention modeling data collection experiment). User feedback from the real-world system evaluation experiment also indicated that while the system was generally beneficial, some participants (P3, P7) still found the prompts occasionally distracting and desired more personalized settings. Consequently, future work should leverage advanced techniques

like LLMs to perform a joint analysis of scene risk (from MLLM analysis) and user attention state (from multimodal sensing), enabling more personalized and context-adaptive AR prompts and interface adjustments [\[77\]](#page-18-41). Compared to training a separate attention classification model—which has limitations in risk attribute understanding and real-time capability—multimodal information fusion can more comprehensively capture environmental dynamics and user internal states, thus providing more accurate and timely warnings and information presentation.

To further enhance interaction naturalness and user acceptance, we plan to introduce a virtual agent. This agent would integrate eye tracking, contextual memory, and multimodal feedback (such as voice prompts and dynamic spatial cues), possibly incorporating natural non-verbal interaction elements (like facial expressions and gestures) to proactively anticipate and respond to user needs [\[9\]](#page-16-12). We hope this design will not only reduce the cognitive load associated with abrupt warning prompts but also improve user response efficiency and safety when facing sudden risks, making the entire system more personalized and practical.

Privacy & Ethics. Systems that continuously monitor a user's physiological state, behavior, and surrounding environment (potentially including other pedestrians) inherently raise significant privacy and ethical concerns, a point echoed by some participants' worries (P15) in the User Survey on Safety Risks. Key challenges include preventing privacy infringement concerning the user's private activities or the public nearby [\[61\]](#page-18-15), and ensuring the security of sensitive data (like EEG, eye-tracking, IMU, and location information) during processing (local or cloud) and storage to prevent leaks and misuse. Although our research (such as the attention modeling data collection experiment and the real-world system evaluation experiment) was conducted primarily in controlled environments, future real-world deployments should prioritize these considerations. Mitigation strategies should include maximizing on-device processing to minimize data outflow, employing privacy-preserving techniques like federated learning, differential privacy, and visual data anonymization (e.g., face blurring), and ensuring transparency with users, granting them explicit control over data collection and system behavior.

User Trust, AR Content, and Study Limitations. A deep consideration of user trust is vital for the successful real-world deployment of any safety-critical system like AttentionAR. The challenge lies in managing a delicate balance, avoiding the dual pitfalls of both under-trust and over-trust. Under-trust can arise if the system is perceived as inaccurate, leading to "alarm fatigue" where usersignore warnings[\[18\]](#page-17-41). Conversely, over-trust can lead to "automation bias," where users reduce their own natural vigilance, which is equally dangerous [\[95\]](#page-18-42). Future work should focus on trust calibration, helping users build an appropriate level of trust. Mechanisms to explore include providing explainable warnings (e.g., "Warning: Unaware pedestrian detected") and visualizing the system's confidence level.

We also acknowledge that the AR content used in our evaluation (Section 7) was limited to a single engaging video. This was a deliberate methodological choice to induce a standardized cognitive load and ensure the internal validity of our results by minimizing confounding variables. However, we agree that testing the system's effectiveness across a wider variety of AR content and tasks is an important next step, which we identify as a key direction for future work.

#### 9 Conclusion

In this paper, we introduced AttentionAR, a novel AR system that enhances user safety by dynamically adapting content based on real-time attention monitoring and environmental risk assessment. By leveraging multi-modal signals (EEG, IMU, and gaze) and a multimodal large language model for scene understanding, AttentionAR bridges the gap between static AR interfaces and complex real-world contexts. Our experiments show that it significantly improves situational awareness and reduces distraction-related risks, with minor latency trade-offs. While challenges like spatial calibration and ambiguous visual cues remain, AttentionAR marks a promising step toward safer, context-aware AR experiences.

#### Acknowledgments

This work was supported in part by the National Natural Science Foundation of China under grant U23B2011, 62102069, U20B2063 and 62220106008, the Key R&D Program of Zhejiang under grant 2024SSYS0091.

#### References

- <span id="page-16-4"></span>[1] Mohammad Abu Tami, Huthaifa I Ashqar, Mohammed Elhenawy, Sebastien Glaser, and Andry Rakotonirainy. 2024. Using multimodal large language models (MLLMs) for automated detection of traffic safety-critical events. Vehicles 6, 3 (2024), 1571–1590.
- <span id="page-16-5"></span>[2] Tolegen Akhmetov and Huseyin Atakan Varol. 2022. An augmented realitybased warning system for enhanced safety in industrial settings. IEEE Transactions on Industrial Informatics 19, 7 (2022), 7966–7977.
- <span id="page-16-9"></span>[3] Mona Algarni, Faisal Saeed, Tawfik Al-Hadhrami, Fahad Ghabban, and Mohammed Al-Sarem. 2022. Deep learning-based approach for emotion recognition using electroencephalography (EEG) signals using bi-directional long short-term memory (Bi-LSTM). Sensors 22, 8 (2022), 2976.
- <span id="page-16-8"></span>[4] Madyan Alsenwi, Tawfik Ismail, and M Saeed Darweesh. 2018. Hybrid Compression Techniquesfor EEG Data Based on Lossy/Lossless Compression Algorithms. arXiv preprint arXiv:1804.02713 (2018).
- <span id="page-16-1"></span>[5] Fatemeh Banani Ardecani, Amit Kumar, Sepehr Sabeti, and Omidreza Shoghli. 2025. Neural correlates of augmented reality safety warnings: EEG analysis of situational awareness and cognitive performance in roadway work zones. Safety Science 185 (2025), 106802.
- <span id="page-16-3"></span>[6] Huthaifa I Ashqar, Taqwa I Alhadidi, Mohammed Elhenawy, and Nour O Khanfar. 2024. Leveraging multimodal large language models (MLLMs) for enhanced object detection and scene understanding in thermal images for autonomous driving systems. Automation 5, 4 (2024), 508–526.
- <span id="page-16-7"></span>[7] Dominik R Bach, Guillaume Flandin, Karl J Friston, and Raymond J Dolan. 2009. Time-series analysis for rapid event-related skin conductance responses. Journal of neuroscience methods 184, 2 (2009), 224–234.
- <span id="page-16-11"></span>[8] Jinze Bai, Shuai Bai, Yunfei Chu, Zeyu Cui, Kai Dang, Xiaodong Deng, Yang Fan, Wenbin Ge, Yu Han, Fei Huang, et al. 2023. Qwen technical report. arXiv preprint arXiv:2309.16609 (2023).
- <span id="page-16-12"></span>[9] Riccardo Bovo, Steven Abreu, Karan Ahuja, Eric J Gonzalez, Li-Te Cheng, and Mar Gonzalez-Franco. 2024. Embardiment: an embodied ai agent for productivity in xr. arXiv preprint arXiv:2408.08158 (2024).
- <span id="page-16-2"></span>[10] Runze Cai, Nuwan Janaka, Hyeongcheol Kim, Yang Chen, Shengdong Zhao, Yun Huang, and David Hsu. 2025. AiGet: Transforming Everyday Moments into Hidden Knowledge Discovery with AI Assistance on Smart Glasses. arXiv preprint arXiv:2501.16240 (2025).
- <span id="page-16-10"></span>[11] Alessandro Calvi, Fabrizio D'Amico, Chiara Ferrante, and Luca Bianchini Ciampoli. 2020. Effectiveness of augmented reality warnings on driving behaviour whilst approaching pedestrian crossings: A driving simulator study. Accident Analysis & Prevention 147 (2020), 105760.
- <span id="page-16-6"></span>[12] Chiao-Ju Chang, Yu Lun Hsu, Wei Tian Mireille Tan, Yu-Cheng Chang, Pin Chun Lu, Yu Chen, Yi-Han Wang, and Mike Y Chen. 2024. Exploring Augmented Reality Interface Designs for Virtual Meetings in Real-world Walking Contexts. In Proceedings of the 2024 ACM Designing Interactive Systems Conference. 391– 408.
- <span id="page-16-0"></span>[13] Sromona Chatterjee, Kevin Scheck, Dennis Küster, Felix Putze, Harish Moturu, Johannes Schering, Jorge Marx Gómez, and Tanja Schultz. 2020. Smarthelm:

AttentionAR: Attention-Gated MLLM Reasoning for AR Safety UIST '25, September 28–October 01, 2025, Busan, Republic of Korea

Towards multimodal detection of attention in an outdoor augmented reality biking scenario. In Companion Publication of the 2020 International Conference on Multimodal Interaction. 426–432.

- <span id="page-17-25"></span>[14] Isha Chaturvedi, Farshid Hassani Bijarbooneh, Tristan Braud, and Pan Hui. 2019. Peripheral vision: a new killer app for smart glasses. In Proceedings of the 24th international conference on intelligent user interfaces. 625–636.
- <span id="page-17-38"></span>[15] Kaiming Cheng, Arkaprabha Bhattacharya, Michelle Lin, Jaewook Lee, Aroosh Kumar, Jeffery F Tian, Tadayoshi Kohno, and Franziska Roesner. 2024. When the User Is Inside the User Interface: An Empirical Study of {UI} Security Properties in Augmented Reality. In 33rd USENIX Security Symposium (USENIX Security 24). 2707–2723.
- <span id="page-17-26"></span>[16] Lung-Pan Cheng, Eyal Ofek, Christian Holz, and Andrew D Wilson. 2019. Vroamer: generating on-the-fly VR experiences while walking inside large, unknown real-world building environments. In 2019 IEEE conference on virtual reality and 3D user interfaces (VR). IEEE, 359–366.
- <span id="page-17-9"></span>[17] Marvin M Chun, Julie D Golomb, and Nicholas B Turk-Browne. 2011. A taxonomy of external and internal attention. Annual review of psychology 62, 1 (2011), 73–101.
- <span id="page-17-41"></span>[18] Maria Cvach. 2012. Monitor alarm fatigue: an integrative review. Biomedical instrumentation & technology 46, 4 (2012), 268–277.
- <span id="page-17-31"></span>[19] Arnaud Delorme, Terrence Sejnowski, and Scott Makeig. 2007. Enhanced detection of artifacts in EEG data using higher-order statistics and independent component analysis. Neuroimage 34, 4 (2007), 1443–1449.
- <span id="page-17-11"></span>[20] Henrik Detjen, Sarah Faltaous, Jonas Keppel, Marvin Prochazka, Uwe Gruenefeld, Shadan Sadeghian, and Stefan Schneegass. 2022. Investigating the influence of gaze-and context-adaptive head-up displays on take-over requests. In Proceedings of the 14th International Conference on Automotive User Interfaces and Interactive Vehicular Applications. 108–118.
- <span id="page-17-37"></span>[21] Mustafa Doga Dogan, Eric J Gonzalez, Karan Ahuja, Ruofei Du, Andrea Colaço, Johnny Lee, Mar Gonzalez-Franco, and David Kim. 2024. Augmented object intelligence: Making the analog world interactable with xr-objects. arXiv preprint arXiv:2404.13274 (2024).
- <span id="page-17-36"></span>[22] Henry W Dong, Caitlin Mills, Robert T Knight, and Julia WY Kam. 2021. Detection of mind wandering using EEG: Within and across individuals. Plos one 16, 5 (2021), e0251490.
- <span id="page-17-5"></span>[23] Mica R Endsley. 1995. Toward a theory of situation awareness in dynamic systems. Human factors 37, 1 (1995), 32–64.
- <span id="page-17-6"></span>[24] Mica R Endsley, Betty Bolté, and Debra G Jones. 2003. Designing for situation awareness: An approach to user-centered design. CRC press.
- <span id="page-17-16"></span>[25] João Marcelo Evangelista Belo, Mathias N Lystbæk, Anna Maria Feit, Ken Pfeuffer, Peter Kán, Antti Oulasvirta, and Kaj Grønbæk. 2022. Auit–the adaptive user interfaces toolkit for designing xr applications. In Proceedings of the 35th Annual ACM Symposium on User Interface Software and Technology. 1–16.
- <span id="page-17-34"></span>[26] Tobias Feigl, Sebastian Kram, Philipp Woller, Ramiz H Siddiqui, Michael Philippsen, and Christopher Mutschler. 2019. A bidirectional LSTM for estimating dynamic human velocities from a single IMU. In 2019 International Conference on Indoor Positioning and Indoor Navigation (IPIN). IEEE, 1–8.
- <span id="page-17-20"></span>[27] Xueyang Feng, Zhi-Yuan Chen, Yujia Qin, Yankai Lin, Xu Chen, Zhiyuan Liu, and Ji-Rong Wen. 2024. Large Language Model-based Human-Agent Collaboration for Complex Task Solving. arXiv preprint arXiv:2402.12914 (2024).
- <span id="page-17-43"></span>[28] Xingyu Fu, Yushi Hu, Bangzheng Li, Yu Feng, Haoyu Wang, Xudong Lin, Dan Roth, Noah A Smith, Wei-Chiu Ma, and Ranjay Krishna. 2024. Blink: Multimodal large language models can see but not perceive. In European Conference on Computer Vision. Springer, 148–166.
- <span id="page-17-29"></span>[29] Alessio Ghio, Sebastian Escalante, and Jimmy Tarrillo. 2018. Analysis of moving average filter for IMU measurements on an 8-bit microcontroller. In 2018 IEEE XXV International Conference on Electronics, Electrical Engineering and Computing (INTERCON). IEEE, 1–4.
- <span id="page-17-13"></span>[30] Thomas Alexander Goodge, Frank Pollick, and Stephen Anthony Brewster. 2024. Can You Hazard a Guess?: Evaluating the Effect of Augmented Reality Cues on Driver Hazard Prediction. In Proceedings of the 2024 CHI Conference on Human Factors in Computing Systems. 1–28.
- <span id="page-17-42"></span>[31] Akshay Gopalkrishnan, Ross Greer, and Mohan Trivedi. 2024. Multi-frame, lightweight & efficient vision-language models for question answering in autonomous driving. arXiv preprint arXiv:2403.19838 (2024).
- <span id="page-17-3"></span>[32] Jens Grubert, Lukas Witzani, Alexander Otte, Travis Gesslein, Matthias Kranz, and Per Ola Kristensson. 2023. Text Entry Performance and Situation Awareness of a Joint Optical See-Through Head-Mounted Display and Smartphone System. IEEE Transactions on Visualization and Computer Graphics 30, 8 (2023), 5830– 5846.
- <span id="page-17-39"></span>[33] Xianda Guo, Ruijun Zhang, Yiqun Duan, Yuhang He, Chenming Zhang, Shuai Liu, and Long Chen. 2024. Drivemllm: A benchmark for spatial understanding with multimodal large language models in autonomous driving. arXiv preprint arXiv:2411.13112 (2024).
- <span id="page-17-27"></span>[34] Thalía Harmony, Thalía Fernández, Juan Silva, Jorge Bernal, Lourdes Díaz-Comas, Alfonso Reyes, Erzsébet Marosi, Mario Rodríguez, and Miguel Rodríguez. 1996. EEG delta activity: an indicator of attention to internal processing during performance of mental tasks. International journal of psychophysiology 24, 1-2

(1996), 161–171.

- <span id="page-17-32"></span>[35] Haibo He and Edwardo A Garcia. 2009. Learning from imbalanced data. IEEE Transactions on knowledge and data engineering 21, 9 (2009), 1263–1284.
- <span id="page-17-33"></span>[36] Sepp Hochreiter and Jürgen Schmidhuber. 1997. Long short-term memory. Neural computation 9, 8 (1997), 1735–1780.
- <span id="page-17-35"></span>[37] Zhentao Huang, Yahong Ma, Rongrong Wang, Weisu Li, and Yongsheng Dai. 2023. A model for EEG-based emotion recognition: CNN-BI-LSTM with attention mechanism. Electronics 12, 14 (2023), 3188.
- <span id="page-17-40"></span>[38] Raisa Islam and Owana Marzia Moushi. 2024. GPT-4o: The Cutting-Edge Advancement in Multimodal LLM. Authorea Preprints (2024).
- <span id="page-17-28"></span>[39] Houtan Jebelli, Sungjoo Hwang, and SangHyun Lee. 2018. EEG signal-processing framework to obtain high-quality brain waves from an off-the-shelf wearable EEG device. Journal of Computing in Civil Engineering 32, 1 (2018), 04017070.
- <span id="page-17-8"></span>[40] Marcia K Johnson. 1983. A multiple-entry, modular memory system. In Psychology of Learning and Motivation. Vol. 17. Elsevier, 81–123.
- <span id="page-17-1"></span>[41] Jinki Jung, Hyeopwoo Lee, Jeehye Choi, Abhilasha Nanda, Uwe Gruenefeld, Tim Stratmann, and Wilko Heuten. 2018. Ensuring safety in augmented reality from trade-off between immersion and situation awareness. In 2018 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, 70–79.
- <span id="page-17-4"></span>[42] David Kadish, Arezoo Sarkheyli-Hägele, Jose Font, Georg Hägele, Diederick C Niehorster, and Thomas Pederson. 2022. Towards Situation Awareness and Attention Guidance in a Multiplayer Environment using Augmented Reality and Carcassonne. In Extended Abstracts of the 2022 Annual Symposium on Computer-Human Interaction in Play. 133–139.
- <span id="page-17-23"></span>[43] HyeongYeop Kang, Geonsun Lee, and JungHyun Han. 2019. Obstacle detection and alert system for smartphone ar users. In Proceedings of the 25th ACM Symposium on Virtual Reality Software and Technology. 1–11.
- <span id="page-17-2"></span>[44] Hyungil Kim, Joseph L Gabbard, Alexandre Miranda Anon, and Teruhisa Misu. 2018. Driver behavior and performance with augmented reality pedestrian collision warning: An outdoor user study. IEEE transactions on visualization and computer graphics 24, 4 (2018), 1515–1524.
- <span id="page-17-21"></span>[45] Hyungil Kim, Alexandre Miranda Anon, Teruhisa Misu, Nanxiang Li, Ashish Tawari, and Kikuo Fujimura. 2016. Look at me: Augmented reality pedestrian warning system using an in-vehicle volumetric head up display. In Proceedings of the 21st International Conference on Intelligent User Interfaces. 294–298.
- <span id="page-17-14"></span>[46] Kinam Kim, Hongjo Kim, and Hyoungkwan Kim. 2017. Image-based construction hazard avoidance system using augmented reality in wearable device. Automation in construction 83 (2017), 390–403.
- <span id="page-17-22"></span>[47] Elisa Maria Klose, Nils Adrian Mack, Jens Hegenberg, and Ludger Schmidt. 2019. Text presentation for augmented reality applications in dual-task situations. In 2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR). IEEE, 636–644.
- <span id="page-17-24"></span>[48] Sho Kodama, Yu Enokibori, and Kenji Mase. 2016. Examination of safe-walking support system for" texting while walking" using time-of-flight range image sensors. In Proceedings of the 2016 ACM International Joint Conference on Pervasive and Ubiquitous Computing: Adjunct. 129–132.
- <span id="page-17-10"></span>[49] Nataliya Kosmyna, Chi-Yun Hu, Yujie Wang, Qiuxuan Wu, Cassandra Scheirer, and Pattie Maes. 2021. A pilot study using covert visuospatial attention as an EEG-based brain computer interface to enhance AR interaction. In Proceedings of the 2021 ACM International Symposium on Wearable Computers. 43–47.
- <span id="page-17-15"></span>[50] Hyunjin Lee and Woontack Woo. 2023. Exploring the effects of augmented reality notification type and placement in AR HMD while walking. In 2023 IEEE Conference Virtual Reality and 3D User Interfaces (VR). IEEE, 519–529.
- <span id="page-17-18"></span>[51] Teesid Leelasawassuk, Dima Damen, and Walterio Mayol-Cuevas. 2017. Automated capture and delivery of assistive task guidance with an eyewear computer: the glaciar system. In Proceedings of the 8th Augmented Human International Conference. 1–9.
- <span id="page-17-19"></span>[52] Jiahao Nick Li, Yan Xu, Tovi Grossman, Stephanie Santosa, and Michelle Li. 2024. OmniActions: Predicting Digital Actions in Response to Real-World Multimodal Sensory Inputs with LLMs. In Proceedings of the CHI Conference on Human Factors in Computing Systems. 1–22.
- <span id="page-17-7"></span>[53] Mengfan Li, Zhongxiang Feng, Weihua Zhang, Lei Wang, Liyang Wei, and Cheng Wang. 2023. How much situation awareness does the driver have when driving autonomously? A study based on driver attention allocation. Transportation research part C: emerging technologies 156 (2023), 104324.
- <span id="page-17-12"></span>[54] Wangfan Li, Rohit Mallick, Carlos Toxtli-Hernandez, Christopher Flathmann, and Nathan J McNeese. 2024. Leveraging Artificial Intelligence to Promote Awareness in Augmented Reality Systems. arXiv preprint arXiv:2405.05916 (2024).
- <span id="page-17-0"></span>[55] Xiao Li, Wen Yi, Hung-Lin Chi, Xiangyu Wang, and Albert PC Chan. 2018. A critical review of virtual and augmented reality (VR/AR) applications in construction safety. Automation in construction 86 (2018), 150–162.
- <span id="page-17-30"></span>[56] Yi Li, Zengyu Liu, Xiandi Zhu, and Ning Xie. 2024. Zeitgebers-Based User Time Perception Analysis and Data-Driven Modeling via Transformer in VR. arXiv preprint arXiv:2412.08223 (2024).
- <span id="page-17-17"></span>[57] Zhipeng Li, Christoph Gebhardt, Yves Inglin, Nicolas Steck, Paul Streli, and Christian Holz. 2024. Situationadapt: Contextual ui optimization in mixed reality with situation awareness via llm reasoning. In Proceedings of the 37th Annual

ACM Symposium on User Interface Software and Technology. 1–13.

- <span id="page-18-40"></span>[58] David Lindlbauer, Anna Maria Feit, and Otmar Hilliges. 2019. Context-aware online adaptation of mixed reality interfaces. In Proceedings of the 32nd annual ACM symposium on user interface software and technology. 147–160.
- <span id="page-18-28"></span>[59] Kuan Liu, Yanen Li, Ning Xu, and Prem Natarajan. 2018. Learn to combine modalities in multimodal deep learning. arXiv preprint arXiv:1805.11730 (2018).
- <span id="page-18-18"></span>[60] Shilong Liu, Hao Cheng, Haotian Liu, Hao Zhang, Feng Li, Tianhe Ren, Xueyan Zou, Jianwei Yang, Hang Su, Jun Zhu, et al. 2023. Llava-plus: Learning to use tools for creating multimodal agents. arXiv preprint arXiv:2311.05437 (2023).
- <span id="page-18-15"></span>[61] Xingyu Bruce Liu, Jiahao Nick Li, David Kim, Xiang'Anthony' Chen, and Ruofei Du. 2024. Human I/O: Towards a Unified Approach to Detecting Situational Impairments. In Proceedings of the CHI Conference on Human Factors in Computing Systems. 1–18.
- <span id="page-18-21"></span>[62] Feiyu Lu and Yan Xu. 2022. Exploring spatial ui transition mechanisms with head-worn augmented reality. In Proceedings of the 2022 CHI Conference on Human Factors in Computing Systems. 1–16.
- <span id="page-18-8"></span>[63] Nachuan Ma, Jiahe Fan, Wenshuo Wang, Jin Wu, Yu Jiang, Lihua Xie, and Rui Fan. 2022. Computer vision for road imaging and pothole detection: a state-ofthe-art review of systems and algorithms. Transportation safety and Environment 4, 4 (2022), tdac026.
- <span id="page-18-13"></span>[64] Elisa Magosso, Francesca De Crescenzio, Giulia Ricci, Sergio Piastra, and Mauro Ursino. 2019. EEG alpha power is modulated by attentional changes during cognitive tasks and virtual reality immersion. Computational intelligence and neuroscience 2019, 1 (2019), 7051079.
- <span id="page-18-22"></span>[65] Pavel Manakhov, Ludwig Sidenmark, Ken Pfeuffer, and Hans Gellersen. 2024. Gaze on the go: Effect of spatial reference frame on visual target acquisition during physical locomotion in extended reality. In Proceedings of the 2024 CHI Conference on Human Factors in Computing Systems. 1–16.
- <span id="page-18-19"></span>[66] Fanqing Meng, Jin Wang, Chuanhao Li, Quanfeng Lu, Hao Tian, Jiaqi Liao, Xizhou Zhu, Jifeng Dai, Yu Qiao, Ping Luo, et al. 2024. Mmiu: Multimodal multi-image understanding for evaluating large vision-language models. arXiv preprint arXiv:2408.02718 (2024).
- <span id="page-18-4"></span>[67] Earl K Miller and Jonathan D Cohen. 2001. An integrative theory of prefrontal cortex function. Annual review of neuroscience 24, 1 (2001), 167–202.
- <span id="page-18-37"></span>[68] Andrew Payne and Sameer Singh. 2005. Indoor vs. outdoor scene classification in digital photographs. Pattern Recognition 38, 10 (2005), 1533–1545.
- <span id="page-18-34"></span>[69] Yunqiang Pei, Jialei Tang, Qihang Tang, Mingfeng Zha, Dongyu Xie, Guoqing Wang, Zhitao Liu, Ning Xie, Peng Wang, Yang Yang, et al. 2024. Emotion Recognition in HMDs: A Multi-task Approach Using Physiological Signals and Occluded Faces. In Proceedings of the 32nd ACM International Conference on Multimedia. 5977–5986.
- <span id="page-18-27"></span>[70] Yunqiang Pei, Keiyue Zhang, Hongrong Yang, Yong Tao, Qihang Tang, Jialei Tang, Guoqing Wang, Zhitao Liu, Ning Xie, Peng Wang, et al. 2024. Improving Interaction Comfort in Authoring Task in AR-HRI through Dynamic Dual-Layer Interaction Adjustment. In Proceedings of the 32nd ACM International Conference on Multimedia. 88–97.
- <span id="page-18-11"></span>[71] Lucas Plabst, Aditya Raikwar, Sebastian Oberdörfer, Francisco Raul Ortega, and Florian Niebling. 2023. Exploring Unimodal Notification Interaction and Display Methods in Augmented Reality. In Proceedings of the 29th ACM Symposium on Virtual Reality Software and Technology. 1–11.
- <span id="page-18-36"></span>[72] Yair Poleg, Chetan Arora, and Shmuel Peleg. 2014. Temporal segmentation of egocentric videos. In Proceedings of the IEEE conference on computer vision and pattern recognition. 2537–2544.
- <span id="page-18-0"></span>[73] Romain Pourchon, Pierre-Majorique Léger, Élise Labonté-LeMoyne, Sylvain Sénécal, François Bellavance, Marc Fredette, and François Courtemanche. 2017. Is augmented reality leading to more risky behaviors? An experiment with Pokémon Go. In HCI in Business, Government and Organizations. Interacting with Information Systems: 4th International Conference, HCIBGO 2017, Held as Part of HCI International 2017, Vancouver, BC, Canada, July 9-14, 2017, Proceedings, Part I 4. Springer, 354–361.
- <span id="page-18-26"></span>[74] Jérôme Prado and André Knops. 2024. Spatial attention in mental arithmetic: A literature review and meta-analysis. Psychonomic Bulletin & Review 31, 5 (2024), 2036–2057.
- <span id="page-18-33"></span>[75] D Alex Quistberg, Eric J Howard, Beth E Ebel, Anne V Moudon, Brian E Saelens, Philip M Hurvitz, James E Curtin, and Frederick P Rivara. 2015. Multilevel models for evaluating the risk of pedestrian–motor vehicle collisions at intersections and mid-blocks. Accident Analysis & Prevention 84 (2015), 99–111.
- <span id="page-18-23"></span>[76] Ashwin Ram and Shengdong Zhao. 2021. Lsvp: Towards effective on-the-go video learning using optical head-mounted displays. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies 5, 1 (2021), 1–27.
- <span id="page-18-41"></span>[77] Andreas Riegler, Andreas Riener, and Clemens Holzmann. 2022. Content presentation on 3D augmented reality windshield displays in the context of automated driving. In 2022 IEEE Conference on Virtual Reality and 3D User Interfaces (VR). IEEE, 543–552.
- <span id="page-18-20"></span>[78] Birat Rijal and Nadir Yilmaz. 2024. Effects of Distracted Pedestrian Behavior on Transportation Safety: Causes and Contributing Factors. Applied Sciences 14, 23 (2024), 11068.
- <span id="page-18-39"></span>[79] Michelle L Rusch, Mark C Schall Jr, Patrick Gavin, John D Lee, Jeffrey D Dawson, Shaun Vecera, and Matthew Rizzo. 2013. Directing driver attention with augmented reality cues. Transportation research part F: traffic psychology and behaviour 16 (2013), 127–137.
- <span id="page-18-3"></span>[80] Eric E Sabelman and Roger Lam. 2015. The real-life dangers of augmented reality. IEEE Spectrum 52, 7 (2015), 48–53.
- <span id="page-18-5"></span>[81] Mazen Salous, Dennis Küster, Kevin Scheck, Aytac Dikfidan, Tim Neumann, Felix Putze, and Tanja Schultz. 2022. Smarthelm: User studies from lab to field for attention modeling. In 2022 IEEE International Conference on Systems, Man, and Cybernetics (SMC). IEEE, 1012–1019.
- <span id="page-18-38"></span>[82] Adarsh Jagan Sathyamoorthy, Kasun Weerakoon, Mohamed Elnoor, Anuj Zore, Brian Ichter, Fei Xia, Jie Tan, Wenhao Yu, and Dinesh Manocha. 2024. Convoi: Context-aware navigation using vision language models in outdoor and indoor environments. In 2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 13837–13844.
- <span id="page-18-14"></span>[83] Nathan Semertzidis, Michaela Jayne Vranic-Peters, Xiao Zoe Fang, Rakesh Patibanda, Aryan Saini, Don Samitha Elvitigala, Fabio Zambetta, and Florian 'Floyd' Mueller. 2024. PsiNet: Toward Understanding the Design of Brain-to-Brain Interfaces for Augmenting Inter-Brain Synchrony. In Proceedings of the 2024 CHI Conference on Human Factors in Computing Systems. 1–18.
- <span id="page-18-2"></span>[84] Xia Su, Han Zhang, Kaiming Cheng, Jaewook Lee, Qiaochu Liu, Wyatt Olson, and Jon E Froehlich. 2024. RASSAR: Room Accessibility and Safety Scanning in Augmented Reality. In Proceedings of the 2024 CHI Conference on Human Factors in Computing Systems. 1–17.
- <span id="page-18-31"></span>[85] Tae Kyung Sung, Namsik Chang, and Gunhee Lee. 1999. Dynamics of modeling in data mining: interpretive approach to bankruptcy prediction. Journal of management information systems 16, 1 (1999), 63–85.
- <span id="page-18-32"></span>[86] Robert J Taggart and David J Wilke. 2025. Warnings based on risk matrices: a coherent framework with consistent evaluation. arXiv preprint arXiv:2502.08891 (2025).
- <span id="page-18-1"></span>[87] Dušan Tatić and Bojan Tešić. 2017. The application of augmented reality technologies for the improvement of occupational safety in an industrial environment. Computers in Industry 85 (2017), 1–10.
- <span id="page-18-12"></span>[88] Julian F Thayer and Richard D Lane. 2009. Claude Bernard and the heart– brain connection: Further elaboration of a model of neurovisceral integration. Neuroscience & Biobehavioral Reviews 33, 2 (2009), 81–88.
- <span id="page-18-29"></span>[89] Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez, Łukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need. Advances in neural information processing systems 30 (2017).
- <span id="page-18-9"></span>[90] Lisa-Marie Vortmann, Felix Kroll, and Felix Putze. 2019. EEG-based classification of internally-and externally-directed attention in an augmented reality paradigm. Frontiers in human neuroscience 13 (2019), 348.
- <span id="page-18-6"></span>[91] Lisa-Marie Vortmann and Felix Putze. 2020. Attention-aware brain computer interface to avoid distractions in augmented reality. In Extended abstracts of the 2020 chi conference on human factors in computing systems. 1–8.
- <span id="page-18-7"></span>[92] Lisa-Marie Vortmann, Leonid Schwenke, and Felix Putze. 2021. Real or virtual? Using brain activity patterns to differentiate attended targets during augmented reality scenarios. arXiv preprint arXiv:2101.05272 (2021).
- <span id="page-18-25"></span>[93] Yuwei Wang, Yimin Wu, Cheng Chen, Bohan Wu, Shu Ma, Duming Wang, Hongting Li, and Zhen Yang. 2022. Inattentional blindness in augmented reality head-up display-assisted driving. International Journal of Human–Computer Interaction 38, 9 (2022), 837–850.
- <span id="page-18-35"></span>[94] Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Fei Xia, Ed Chi, Quoc V Le, Denny Zhou, et al. 2022. Chain-of-thought prompting elicits reasoning in large language models. Advances in neural information processing systems 35 (2022), 24824–24837.
- <span id="page-18-42"></span>[95] Magdalena Wischnewski, Nicole Krämer, and Emmanuel Müller. 2023. Measuring and understanding trust calibrations for automated systems: A survey of the state-of-the-art and future directions. In Proceedings of the 2023 CHI conference on human factors in computing systems. 1–16.
- <span id="page-18-16"></span>[96] Junlin Xie, Zhihong Chen, Ruifei Zhang, Xiang Wan, and Guanbin Li. 2024. Large multimodal agents: A survey. arXiv preprint arXiv:2402.15116 (2024).
- <span id="page-18-10"></span>[97] Xuhai Xu, Anna Yu, Tanya R Jonker, Kashyap Todi, Feiyu Lu, Xun Qian, João Marcelo Evangelista Belo, Tianyi Wang, Michelle Li, Aran Mun, et al. 2023. Xair: A framework of explainable ai in augmented reality. In Proceedings of the 2023 CHI Conference on Human Factors in Computing Systems. 1–30.
- <span id="page-18-24"></span>[98] Jackie Yang, Christian Holz, Eyal Ofek, and Andrew D Wilson. 2019. Dreamwalker: Substituting real-world walking experiences with a virtual reality. In Proceedings of the 32nd annual ACM symposium on user interface software and technology. 1093–1107.
- <span id="page-18-17"></span>[99] Duzhen Zhang, Yahan Yu, Jiahua Dong, Chenxing Li, Dan Su, Chenhui Chu, and Dong Yu. 2024. Mm-llms: Recent advances in multimodal large language models. arXiv preprint arXiv:2401.13601 (2024).
- <span id="page-18-30"></span>[100] Xiaowei Zhang, Xiangyu Wei, Zhongyi Zhou, Qiqi Zhao, Sipo Zhang, Yikun Yang, Rui Li, and Bin Hu. 2023. Dynamic Alignment and Fusion of Multimodal Physiological Patterns for Stress Recognition. IEEE Transactions on Affective Computing (2023).

<span id="page-19-0"></span>

- <span id="page-19-3"></span>[101] Yijing Zhang, Linjun Lu, Qiujia Liu, and Miaoqing Hu. 2023. Modeling of low-risk behavior of pedestrian movement based on dynamic data analysis. Transportation research part A: policy and practice 168 (2023), 103576.
- <span id="page-19-1"></span>[102] Yuhang Zhao, Elizabeth Kupferstein, Brenda Veronica Castro, Steven Feiner, and Shiri Azenkot. 2019. Designing AR visualizations to facilitate stair navigation for people with low vision. In Proceedings of the 32nd annual ACM symposium

on user interface software and technology. 387–402.

<span id="page-19-2"></span>[103] Peng Zhou, Wei Shi, Jun Tian, Zhenyu Qi, Bingchen Li, Hongwei Hao, and Bo Xu. 2016. Attention-based bidirectional long short-term memory networks for relation classification. In Proceedings of the 54th annual meeting of the association for computational linguistics (volume 2: Short papers). 207–212.