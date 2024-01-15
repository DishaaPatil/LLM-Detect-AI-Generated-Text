# LLM-Detect-AI-Generated-Text
Problem Statement: www.kaggle.com/competitions/llm-detect-ai-generated-text/overview/description
Dataset: https://www.kaggle.com/competitions/llm-detect-ai-generated-text/data

On doing basic EDA, it was found that the Dataset was imbalanced and it had very few AI Generated essays. This would prove to be a problem in training hence I added extra sample essays which were AI generated.
Extended dataset: https://www.kaggle.com/datasets/thedrcat/daigt-proper-train-dataset
After this I found there are nearly thrice as many non generated than generated essays, so I used an undersampler, which brought the number down to 44087 for each label '1' and '0'.
Post this, I proceeded with using the tokenizer and converting sentences into vectors to proceed with Neural Networks.
The DNN was as follows:

![Screenshot 2024-01-15 112246](https://github.com/DishaaPatil/LLM-Detect-AI-Generated-Text/assets/102872725/e3c04d9c-8c3c-4687-9ab5-ea85cfa98fd9)

Further after the training, following accuracy and loss was seen:

![image](https://github.com/DishaaPatil/LLM-Detect-AI-Generated-Text/assets/102872725/a32ad2da-a5d3-4544-b772-f739f5f2494f)
![image](https://github.com/DishaaPatil/LLM-Detect-AI-Generated-Text/assets/102872725/832ed3e4-d041-487e-a2be-33c411437f27)

This gave an accuracy of 83.3% on the test data of Kaggle.
