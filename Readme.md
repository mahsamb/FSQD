
**Fine-Grained Question Subjectivity Dataset (FQSD)**

**Introduction**

In the evolving realm of question subjectivity classification, there's an imperative need for high-quality datasets. FQSD addresses this by introducing a fine-grained dataset tailor-made to bolster the development of Automatic Subjective Question Answering (ASQA) systems.

**Background**

Current datasets in the domain offer a binary perspective on question subjectivity, majorly distinguishing between subjective and objective questions. However, real-world questions often tread a spectrum of subjectivity nuances. Recognizing this, FQSD presents a detailed categorization system, aiming to capture the intricacies of question subjectivity more holistically.

**Task Description**

**Main Task**:

**Question Subjectivity Classification**: Identify if a question is subjective or objective.

**Subtasks**:

**Subjective-types Classification**: Here, the objective is to classify subjective questions into specific types:
**Target**: Questions focusing on specific entities or subjects.

**Attitude**: Questions reflecting a particular sentiment or perspective.

**Reason**: Questions seeking justification or rationale.

**Yes/No**: Binary subjective questions.

**None**: Questions that don't fit into the aforementioned categories.

**Comparison-form Classification**: Classify how a question is framed in terms of comparison:

**Single**: Questions without a comparative element.

**Comparative**: Questions comparing two or more entities or subjects.

**Dataset Characteristics**

**Size**: Comprises a total of 10,000 meticulously curated questions.

**Annotation Integrity**: Annotations have been vetted by three expert annotators, achieving a commendable Fleiss's Kappa score of 0.76 and Pearson correlation values peaking at 0.80.

**Columns Description**

**Question**: Textual representation of the question.

**Subjectivity_Level**: A binary column denoting if the question is subjective or objective.

**Subjective_Type**: Delineates the category of subjectivity.

**Comparison_Form**: Depicts whether the question has a comparative format.



**Sample Data**

(Provide 5-6 sample rows for a clearer understanding of the data structure)

**Benchmarking**

FQSD has been tested against well-known datasets like:

**Yu, Zha, and Chua (2012)**

**SubjQA by Bjerva, Bhutani, Golshan, Tan, and Augenstein (2020)**

**ConvEx-DS by Hernandez-Bocanegra and Ziegler (2021)**

In these comparisons, FQSD showcased superiority in terms of scale, linguistic diversity, and syntactic intricacy.

**Usage & Guidelines**

Researchers leveraging FQSD can benefit from its granular categorization system. We recommend a thorough exploration of the dataset's linguistic nuances for better model generalization.

**Licensing & Attribution**

(Include licensing details and a citation format so users can appropriately reference your dataset in their works.)
