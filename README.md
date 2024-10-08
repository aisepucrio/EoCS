# Eyes on Code Smells: Analyzing Developers' Responses During Code Snippet Analysis

This repository contains supplementary results and the data used in the study "Eyes on Code Smells: Analyzing Developers’ Responses During Code Snippet Analysis". The study investigates how the presence of code smells influences developers' program comprehension using eye-tracking technology. The accepted paper can be accessed [here](https://github.com/aisepucrio/EoCS/blob/main/Eyes_on_Code_Smell_Analyzing_Developers%E2%80%99_Responses_During_Code_Snippet_Analysis.pdf).

## Overview

![Overview](overview.png)

In this study, we conducted an analysis of developers' responses to code smells using eye-tracking technology. We examined 13 code snippets, each potentially containing one of three types of code smells: data class, feature envy, or long method. Our objective was to understand the cognitive load these smells impose on developers during program comprehension.

The code snippets were selected from the "MLCQ" (Madeyski Lewowski Code Quest) dataset, which includes 4,770 manually reviewed code samples from 792 open-source projects. This dataset was chosen for its robustness and relevance, as it was developed with the support of 26 experienced industry developers who provided detailed severity classifications for various code smells.

Data was collected from 12 participants, who analyzed the selected code snippets while their eye movements were tracked. The experiment took place in a controlled university environment, ensuring minimal external interference. We measured fixation metrics, such as Average Fixation Duration (AFD) and fixation count (FC), to determine how different code smells influence developers' attention and cognitive effort.

All participants provided informed consent, and their data were anonymized to protect their privacy.

### Required Skills
The reviewer should have a basic understanding of Java programming to review and understand the code snippets. Familiarity with common Java coding patterns and practices will be beneficial for interpreting the code snippets and the presence or not of code smells.

### Required Resources
The artifacts can be reviewed and executed on any standard computer system. There are no specific hardware requirements. The artifacts are compatible with any operating system. No additional software packages or specific devices are required.

-----

## Results

![Correlation between Perceived Complexity, Feeling and Cognitive Effort in Code Snippets](feeling_complexity_fixation.png)

To demonstrate our results, we used normalized qualitative data about the perceived complexity of the code snippet by the participants and quantitative fixation data from the eye tracker. Our results indicate that the code snippets considered more complex by the developers required more fixations, resulting in higher cognitive effort. This is particularly evident in the case of the "long method" code smells. Additionally, we noted that the "data class" code smell presents a lower cognitive effort compared to other code smells, as reflected by lower fixation values.

--------

## Data

### Data Provenance

The data used in this study was sourced from the ["MLCQ" dataset](https://zenodo.org/records/3666840), developed by Lech Madeyski and Tomasz Lewowski, as presented in the paper "MLCQ: Industry-relevant code smell data set" (EASE2020). The dataset includes 4,770 manually reviewed code samples from 792 open-source projects and was developed with the support of 26 experienced industry developers who classified the severity of various code smells. The original paper can be accessed [here](https://doi.org/10.1145/3383219.3383264).

### Developers Fixations

The *01_12_merged_fixation.tsv* file contains the fixations data of the developers who participated in the study.

Fixations were extracted from databases generated by iTrace-Tools. Due to the size of each generated database, we extracted the table that represented each developer's fixation data and aggregated it into a .tsv file.

### Developers Answers

The *answers_experiments.tsv* file contains the answers of the developers who participated in the study.

### Data Dictionary

The *data_dictionary.pdf* provides the data dictionary for the features collected with the iTrace-Tools from the *01_12_merged_fixation.tsv* file and the questions for each column in the answers_experiments.tsv file.

### Code Snippets

The *code_snippets.xlsx* file contains the data for each code snippet extracted from MLCQ dataset that was analyzed by the developers who participated in the study.

### Survey

The *Survey.pdf* file presents the form used for the collection of qualitative data from the participants who performed the experiment.

## Storage Requirements

The total size of the dataset, including fixation data and developer answers, is approximately 4 MB. All files are in standard formats such as .tsv, .xlsx, and .pdf, which can be opened with common tools like Excel, LibreOffice, and any text editor. No special storage hardware or software is required beyond the capacity to store and process up to 4 MB of data.

## Ethical and Legal Statements

The experiment was submitted and approved by the research ethics committee (CEP) through the Plataforma Brasil under the Certificate of Presentation of Ethical Appreciation (CAAE) number 74286223.4.0000.5235. Any data or elements that could identify the participant, such as their name or image, have not been and will not be disclosed, being kept anonymous. All participants agreed to participate by signing the "Free and Informed Consent Form" (TCLE), which outlined the data collection process and how their data would be treated.

## License

This repository is licensed under the GNU License. Please see the LICENSE file for more details.
