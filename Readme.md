# Exploration of the Fine-Grained Question Subjectivity Dataset (FQSD)
 

This notebook provides a comprehensive exploration of the `Fine-Grained Question Subjectivity Dataset (FQSD)`in the smartphone domain. Designed to distinguish not only between subjective and objective questions, FQSD offers additional categorizations to foster advancements in Automatic Subjective Question Answering (ASQA) systems.

## An Introduction to the Dataset

  FQSD presents a curated collection of 10,000 questions, each meticulously classified to delve into the multifaceted aspects of question subjectivity. The dataset is heralded for its remarkable granularity and detailed categorizations, offering researchers and practitioners alike a robust foundation for examining and constructing ASQA systems.

### Main Classification Task

  

The FQSD segments questions into 10 unique classes, each tailored to offer insights into different dimensions of Fine-grained Subjectivity classification:

  

- **[TSS]:** Target Single Subjective

- **[TCS]:** Target Comparative Subjective

- **[ASS]:** Attitude Single Subjective

- **[ACS]:** Attitude Comparative Subjective

- **[RSS]:** Reason Single Subjective

- **[RCS]:** Reason Comparative Subjective

- **[YSS]:** Yes/No Single Subjective

- **[YCS]:** Yes/No Comparative Subjective

- **[NSO]:** None Single Objective

- **[NCO]:** None Comparative Objective

  

Each class serves as a lens through which the nuances of question subjectivity can be further discerned and analyzed, offering a structured framework for both exploration and model training within the domain.

  

## Diving Deeper: Exploring Subtasks

  

### 1. Subjectivity Classification

  

Under this subtask, the focus is pinned on bifurcating questions into generalized types such as:

- **[S]:** Subjective, where the question implies subjectivity or opinion.

- **[O]:** Objective, where the question seeks factual and verifiable information.

  

### 2. Comparison-form Classification

  

This classification subtask differentiates between distinct forms of questions:

- **[C]:** Comparative, implying a comparison between products.

- **[S]:** Single, implying no comparative analysis.

  

### 3. Subjective-types Classification

  

This level delves into the specific type of subjectivity found in questions, categorized as:

- **[T]:** Target,Inquiring about the entity subject to public perception.

- **[A]:** Attitude, Seeking the rationale behind prevailing public views about a particular entity.

- **[R]:** Reason, Querying public sentiment regarding a specific entity.

- **[Y]:** Yes/No, Probing to confirm the accuracy of a statement related to a particular entity.

- **[N]:** None

  

### 4. Subjectiveity_ComparisionForm Classification

  

This subtask meticulously categorizes subjective questions into further distinct types, such as:

- **[CS]:** Comparative Subjective

- **[CO]:** Comparative Objective

- **[SS]:** Single Subjective

- **[SO]:** Single Objective

  

FQSD, through its detailed categorization and well-defined structure, aims to be a pivotal tool for researchers and engineers in developing, validating, and optimizing ASQA systems, thus paving the way for more accurate and reliable subjectivity analysis in automated question answering.


## Usage Example and Guide 
For detailed examples and usage of the dataset, refer to the [Example Usage Notebook](./ExampleUsage.ipynb).


## Sample Data

Below is a sample from the dataset to give a brief overview of its structure:


| Example                                                         | FSQC | Comparison-Form | Subjective-Type | Subjectivity | Additional Info        |
|-----------------------------------------------------------------|------|-----------------|-----------------|--------------|------------------------|
| Which phone has a good camera with a price range of 120 – 210 $?| TSS  | Single          | Target          | Subjective   | Single Subjective      |
| Which phone is slightly better than Samsung X?                  | TCS  | Comparative     | Target          | Subjective   | Comparative Subjective |   | What do people say about the sound quality of Samsung X?        | ASS  | Single          | Attitude        | Subjective   | Single Subjective      |
| What's better: iPhone X or Samsung Y?                           | ACS  | Comparative     | Attitude        | Subjective   | Comparative Subjective |
| Why do people recommend buying Samsung X?                       | RSS  | Single          | Reason          | Subjective   | Single Subjective      |
| Why do people prefer iPhone X over Samsung Y?                   | RCS  | Comparative     | Reason          | Subjective   | Comparative Subjective |
| Do people recommend buying Samsung X?                           | YSS  | Single          | Yes/No          | Subjective   | Single Subjective      |
| Is Samsung as good as Samsung Y?                                | YCS  | Comparative     | Yes/No          | Subjective   | Comparative Subjective |
| How long does the Samsung battery life last?                    | NSO  | Single          | None            | Objective    | Single Objective       |
| Which of Samsung X and Samsung Y are heavier?                   | NCO  | Comparative     | None            | Objective    | Comparative Objective  |



## Benchmarking

FQSD has been tested against well-known datasets like:

- **Yu, Zha, and Chua (2012)**

- **SubjQA by Bjerva, Bhutani, Golshan, Tan, and Augenstein (2020)**

- **ConvEx-DS by Hernandez-Bocanegra and Ziegler (2021)**

In these comparisons, FQSD showcased superiority in terms of scale, linguistic diversity, and syntactic intricacy.



## Usage & Guidelines

Researchers leveraging FQSD can benefit from its granular categorization system. We recommend a thorough exploration of the dataset's linguistic nuances for better model generalization.



## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.
