# Exploration of the Fine-Grained Question Subjectivity Dataset (FQSD)
 

This notebook provides a comprehensive exploration of the `Fine-Grained Question Subjectivity Dataset (FQSD)`in the smartphone domain. Designed to distinguish not only between subjective and objective questions, FQSD offers additional categorizations to foster advancements in Automatic Subjective Question Answering (ASQA) systems.

## An Introduction to the Dataset

  FQSD presents a curated collection of 10,000 questions, each meticulously classified to delve into the multifaceted aspects of question subjectivity. The dataset is heralded for its remarkable granularity and detailed categorizations, offering researchers and practitioners alike a robust foundation for examining and constructing ASQA systems.

### Main Classification Task: Fine-Grained Question Subjectivity Classification (FQSC)

  

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
For detailed examples and usage of the dataset, along with insights from figures pertaining to our analysis, please refer to the [Example Usage Notebook](./Figures.ipynb), which includes figures from our article.

For detailed insights and usage examples of our dataset and analysis, refer to the Example Usage Notebook, which includes figures from our article. To showcase our methodology and facilitate a comparative analysis with other transformer models like BERT and XLNet, we provide links to Sample Runs below:
To further illustrate the effectiveness of our approach and facilitate comparative analysis with other transformer models like BERT and XLNet, we have provided Sample Runs for each model evaluation, aligned with our article's methodology.

 - Our Approach with RoBERTa Evaluation: [Sample Run for RoBERTa Notebook](./RoBERTa_Model.ipynb)
 - Comparative Evaluation with BERT: [Sample Run for BERT Notebook](./BERT_Model.ipynb)
 - Comparative Evaluation with XLNet: [Sample Run for XLnet Notebook](./XLnet_Model.ipynb)

It should be noted that our findings are based on the average of five runs, using a 5-fold cross-validation strategy to ensure robustness. The showcased code represents one run, highlighting our training and evaluation process on the FQSD across metrics like precision, recall, and F1-score. This approach offers a glimpse into the comparative performance of these models.


## Sample Data

Below is a sample from the dataset to give a brief overview of its structure:

| Example                                                         | FSQC | Comparison-Form | Subjectivity | Subjective-Type |ComparisonForm-Subjectivity|
|-----------------------------------------------------------------|------|-----------------|--------------|-----------------|---------------------------|
| Which smartphone would you suggest, the Samsung Galaxy Note 10 Plus or the Huawei P30?	| TSS  | Single          | Subjective   | Target          | Single Subjective  |
| Which one has a more attractive interface, the Samsung Galaxy S21 + or the iPhone 12 Pro Max?	| TCS  | Comparative     | Subjective   | Target          | Comparative Subjective  |
| How well does the Galaxy Z Flip 2 handle gaming and graphic-intensive apps?| ASS  | Single          | Subjective   | Attitude        | Single Subjective |
| How does the camera sharpness compare between Honor 10X and Realme 8 Pro+?	| ACS  | Comparative     | Subjective   | Attitude        | Comparative Subjective   |
| Why might users who seek a smartphone that balances performance and affordability consider the Micromax Selfie 2X?	 | RSS  | Single          | Subjective   | Reason          | Single Subjective         |
| Why might someone go for the Realme 8 Pro Extreme over the Sony Xperia 1 VI for faster charging?	| RCS  | Comparative     | Subjective   | Reason          | Comparative Subjective    |
| Do you think the iPhone SE Plus offers sufficient security features?    | YSS  | Single          | Subjective   | Yes/No          | Single Subjective         |
| Is the iPhone 12 Mini better at handling large amounts of data than the Xiaomi Redmi K40?	 | YCS  | Comparative     | Subjective   | Yes/No          | Comparative Subjective    |
| Does the Zenfone 14 Mini provide various camera modes and features?| NSO  | Single          | Objective    | None            | Single Objective          |
| Is the Vivo X70's user interface customizable with different themes and icon packs?| NCO  | Comparative     | Objective    | None            | Comparative Objective     |


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
