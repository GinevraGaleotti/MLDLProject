**Natural Language Queries on Ego4D Dataset**

This project addresses the task of Natural Language Queries (NLQ) from the egocentric Ego4D dataset, a benchmark requiring the prediction of video temporal segments in response to natural language queries. The main objective was to improve the performance of existing models by augmenting the dataset using a language model (LLM) called GEMMA to generate new queries based on the annotations of the original dataset.

Initially, we conducted a comparison of existing networks, testing different text encoders (BERT, GloVe), pre-extracted features (EgoVLP, Omnivore), and network architectures (VSLBase, VSLNet) to identify the best-performing combination. Subsequently, we explored two different approaches to create an augmented dataset, which was then used for pre-training and fine-tuning the previously selected optimal network.

**File and Notebooks descriptions**


Finetuning augmentation first approach.ipynbThis notebook creates the augmented dataset using the first approach and subsequently performs fine-tuning and pre-training on the original dataset.

Finetuning augmentation second approach.ipynbThis notebook creates the augmented dataset using the second approach and subsequently performs fine-tuning and pre-training on the original dataset.

Networks comparison.ipynbContains a comparative analysis of different model configurations, pre-extracted features, and text encoders. The files mainBase.py, VSLBase.py, and runner_utilsBase.py are utilized within this notebook. The numerical output results are documented in the PDF file Network comparison results.



