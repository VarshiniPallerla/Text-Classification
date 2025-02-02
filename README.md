# Evaluation of Text Classification Pretrained Models using Topsis

In this project, I have used several text classification models from the Hugging Face Transformers library. Further, I have applied these Pre-Trained models to short text multi labeled emotion classification dataset. Using the obtained evaluation parameters results, I have compared the performance of these models using the Topsis score ranking. 

**Dataset:** https://huggingface.co/datasets/jakeazcona/short-text-multi-labeled-emotion-classification

**Input Data:**
| Unnamed  | Sample                                                                                                       | Emotion |
|----------|--------------------------------------------------------------------------------------------------------------|---------|
| 0        | i didnt feel humiliated                                                                                      | 5       |
| 1        | i can go from feeling so hopeless to so damned hopeful just from being around someone who cares and is awake | 5       |
| 2        | im grabbing a minute to post i feel greedy wrong                                                             | 0       |
| 3        | i am ever feeling nostalgic about the fireplace i will know that it is still on the property                 | 3       |
| 4        | i am feeling grouchy                                                                                         | 0       |


**Models Used:**
1. Bert-base-uncased: A pretrained BERT model (uncased) for natural language understanding tasks like text classification and question answering.
2. Distilbert-base-uncased: A smaller, faster, and lighter version of BERT with 40% fewer parameters while retaining 97% of its performance.
3. Roberta-base: An optimized variant of BERT trained with more data and dynamic masking for improved language understanding.
4. Albert-base-v2: A lightweight version of BERT with parameter-sharing and factorized embeddings for efficiency and scalability.
5. Xlnet-base-cased: A transformer model that uses permutation-based training to capture bidirectional context more effectively than BERT.


**Evaluation Metrics**
1. Accuracy
2. Precision (Macro and Micro)
3. Recall (Macro and Micro)
4. F1 Score (Macro and Micro)
5. Cohen's Kappa


**Output:**
| Model                     | Accuracy | Precision Weighted | Recall Weighted | F1 Weighted | Cohen Kappa |
|---------------------------|----------|--------------------|-----------------|-------------|-------------|
| bert-base-uncased         | 0.1272   | 0.0298419          | 0.1272          | 0.0378302   | 0.00216505  |
| roberta-base              | 0.1268   | 0.0160782          | 0.1268          | 0.0285379   | 0           |
| distilbert-base-uncased   | 0.1264   | 0.0414592          | 0.1264          | 0.0382028   | 0.0013111   |
| xlnet-base-cased          | 0.1296   | 0.0363586          | 0.1296          | 0.0431487   | 0.00489431  |
| albert-base-v2            | 0.1204   | 0.0300729          | 0.1204          | 0.0467224   |-0.00678552  |



**Evaluation parameters of different models**

<img width="667" alt="{90582F28-4441-4FC3-A444-8C6CE032E31E}" src="https://github.com/user-attachments/assets/ca52ba2d-5221-45d6-9128-01964000f333" />



**Bargraph showing topsis score vs models**

<img width="321" alt="{D408CD7E-2ACD-4C92-A90E-6EC6412BBB4D}" src="https://github.com/user-attachments/assets/dff2704c-af98-4b69-9d6b-6dcc8b631492" />



**Use Cases**
1. Sentiment Analysis
2. Topic Classification
3. Spam Detection
4. Document Categorization
5. Customer Feedback Analysis
