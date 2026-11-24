
🐦 EmpathyBot

Emotion-Aware Chatbot | TweetEval | RAG | FAISS | Few-Shot Prompting

EmpathyBot is an NLP-based, emotion-aware chatbot pipeline that combines emotion classification, Retrieval-Augmented Generation (RAG), semantic search, and few-shot prompt engineering to generate context-aware explanations for social media text.

The project uses a pretrained DistilBERT emotion classifier, a FAISS-powered retrieval system, and GPT-style text generation to identify emotional patterns and provide supporting context for its predictions.

⸻

✨ Key Features

🧠 1. Emotion Classification

* Uses bhadresh-savani/distilbert-base-uncased-emotion.
* Classifies text into six emotion categories:
    * 😊 Joy
    * 😢 Sadness
    * 😡 Anger
    * ❤️ Love
    * 😲 Surprise
    * 😨 Fear

🔎 2. Retrieval-Augmented Generation (RAG)

* Retrieves semantically similar tweets from a knowledge base (kb.txt).
* Uses SentenceTransformers for text embeddings.
* Uses FAISS for efficient similarity search.
* Provides retrieved examples as supporting context.

🎯 3. Few-Shot Prompt Engineering

* Incorporates three sampled (tweet, emotion) examples into the generation prompt.
* Improves contextual grounding and explanation quality.
* Combines retrieved information with emotion classification results.

💬 4. Interactive Streamlit Application

The application displays:

* Predicted emotion.
* Generated explanation.
* Retrieved supporting tweets.

☁️ 5. Google Colab Integration

* Designed to run on Google Colab.
* Uses ngrok to expose the Streamlit application through a public URL.

⸻

🏗️ System Architecture

                 User Input
                     |
                     v
             Text Preprocessing
                     |
                     v
           Emotion Classification
                  (DistilBERT)
                     |
                     v
             Predicted Emotion
                     |
          +----------+----------+
          |                     |
          v                     v
     Knowledge Base       Few-Shot Examples
          |                     |
          v                     |
   Sentence Embeddings          |
          |                     |
          v                     |
      FAISS Search              |
          |                     |
          v                     |
    Retrieved Tweets            |
          |                     |
          +----------+----------+
                     |
                     v
              RAG + Prompt
                     |
                     v
           GPT-Style Generation
                     |
                     v
          Contextual Explanation
                     |
                     v
              Streamlit UI

⸻

🛠️ Technologies & Tools

Category	Technologies
Programming Language	Python
NLP	Hugging Face Transformers
Emotion Classification	DistilBERT
Dataset	TweetEval
Embeddings	SentenceTransformers
Vector Search	FAISS
Generation	GPT-style Language Models
Application Interface	Streamlit
Cloud Environment	Google Colab
Public Tunneling	ngrok

⸻

📊 Dataset & Pretrained Model

TweetEval – Emotion Dataset

* Dataset: Cardiff NLP – TweetEval
* Used for emotion-related tweet classification and evaluation.
* Original benchmark paper:

@inproceedings{barbieri2020tweeteval,
  title={TweetEval: Unified Benchmark and Comparative Evaluation for Tweet Classification},
  author={Barbieri, Francesco and Camacho-Collados, Jose
  and Espinosa-Anke, Luis and Neves, Leonardo},
  booktitle={Findings of EMNLP},
  year={2020}
}

Pretrained Emotion Model

Model: bhadresh-savani/distilbert-base-uncased-emotion

* Architecture: DistilBERT.
* Task: Multi-class emotion classification.
* Number of emotion categories: 6.
* Published model license: Apache License 2.0 (verify the model card and associated files for applicable terms).

⸻

🚀 Project Resources & Demo

Resource	Link
📂 Google Drive – Project & Demo	Open Google Drive
📓 Google Colab Notebook	Open Notebook
🤗 Pretrained Model	Hugging Face
📊 Dataset	TweetEval

⸻

⚠️ Limitations & Responsible Use

* Emotion classification represents model predictions, not definitive knowledge of a person’s emotional or psychological state.
* Classification accuracy may vary depending on language, context, sarcasm, and text quality.
* Generated explanations depend on the retrieved examples and the configured generation model.
* The system is intended for NLP experimentation and educational purposes, not clinical diagnosis or psychological assessment.
* Users must independently comply with applicable dataset, model, library, and third-party service terms.

⸻

📜 Licensing & Intellectual Property

Project Source Code

Copyright © 2026 Mahmoud Saeed Mansour.

The original source code authored specifically for EmpathyBot is distributed under a custom MIT-derived license with an additional attribution requirement.

The full license terms are provided in the LICENSE file in this repository.

You are permitted to:

* Use the original project code commercially or privately.
* Copy and modify the original code.
* Distribute original code and modified versions.
* Incorporate substantial portions of the original code into other projects.

These permissions are subject to the conditions stated in the LICENSE file, including preservation of copyright and license notices and the additional attribution requirement.

Mandatory Attribution Requirement

Anyone using, copying, modifying, distributing, or incorporating substantial portions of the original EmpathyBot source code into another project must provide clear and visible credit to the original author:

Mahmoud Saeed Mansour

* GitHub: https://github.com/Mahmoud3301
* Original Project: EmpathyBot repository (link to this repository when applicable).

The attribution must not be removed, obscured, or misrepresented.

Third-Party Components & External Resources

This project incorporates or references third-party resources that remain subject to their respective licenses and terms:

Component	Original Source	License / Terms
Emotion Classification Model	Hugging Face	Apache 2.0 (subject to the model’s published terms)
TweetEval Dataset	Cardiff NLP	Subset-specific terms; see dataset card
FAISS	Facebook Research	MIT
SentenceTransformers	UKPLab	See upstream license
Streamlit	Streamlit	See upstream license

The license in this repository applies only to the original source code authored for EmpathyBot.

It does not grant ownership of, or override the licensing terms of, third-party models, datasets, libraries, APIs, or external resources.

Third-Party Usage Conditions

* Original third-party authors and contributors retain their respective rights.
* Applicable copyright notices and license conditions must be preserved.
* Dataset usage must comply with the original dataset terms and applicable platform policies.
* Commercial use of third-party resources must be evaluated independently.
* Users are responsible for reviewing the licenses and terms of all external dependencies before using or distributing them.

⸻

👨‍💻 Author

Mahmoud Saeed Mansour

AI & Machine Learning Engineer | NLP | RAG | Deep Learning

* GitHub: @Mahmoud3301
* LinkedIn: Mahmoud Saeed Mansour
* Portfolio: Personal Portfolio

⸻

© Copyright Notice

© 2026 Mahmoud Saeed Mansour.

All rights reserved to the original project contributions, subject to the custom license terms stated in the LICENSE file and the applicable rights and licenses of third-party components.

Unauthorized removal, concealment, or misrepresentation of the original authorship and required attribution is not permitted.