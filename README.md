
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
* Published model license: Apache License 2.0 (subject to the model card and associated files).

⸻

🚀 Project Resources & Demo

Resource	Link
📂 Google Drive – Project & Demo	Open Google Drive
📓 Google Colab Notebook	Open Notebook
🤗 Pretrained Model	Hugging Face
📊 Dataset	TweetEval
📜 Project License	View LICENSE
💻 GitHub Repository	EmpathyBot

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

The complete license terms are available in the repository’s LICENSE file.

License: MIT License with Additional Attribution Requirement

This license permits:

* Commercial and private use of the original project code.
* Copying and modifying the original source code.
* Distribution of original and modified versions.
* Incorporating substantial portions of the original code into other projects.

All permissions are subject to the conditions specified in the LICENSE file.

Mandatory Attribution Requirement

Anyone using, copying, modifying, distributing, or incorporating substantial portions of the original EmpathyBot source code into another project must provide clear and visible credit to the original author.

Original Author: Mahmoud Saeed Mansour

* GitHub Profile: @Mahmoud3301
* Original Repository: EmpathyBot – GitHub
* License: LICENSE

The attribution must not be removed, obscured, or misrepresented.

Where applicable, users must include a link to the original repository.

Third-Party Components & External Resources

This project incorporates or references third-party resources that remain subject to their respective licenses and terms.

Component	Original Source	License / Terms
Emotion Classification Model	Hugging Face	Apache 2.0 (verify model card and associated files)
TweetEval Dataset	Cardiff NLP	Check dataset card and applicable terms
FAISS	Facebook Research	MIT
SentenceTransformers	UKPLab	See upstream license
Streamlit	Streamlit	See upstream license

Important:

The custom license in this repository applies only to the original source code authored for EmpathyBot.

It does not:

* Transfer ownership of third-party components to the project author.
* Override third-party licenses or usage restrictions.
* Grant additional rights to external models, datasets, APIs, or services.
* Automatically authorize commercial use of third-party resources.

Users and organizations are responsible for reviewing and complying with the applicable terms of every external dependency.

Copyright & Attribution Protection

Copyright © 2026 Mahmoud Saeed Mansour.

The original project contributions are protected under the terms specified in the repository’s LICENSE file.

Unauthorized removal, concealment, or misrepresentation of the original authorship and required attribution is not permitted.

⸻

👨‍💻 Author

Mahmoud Saeed Mansour

AI & Machine Learning Engineer | NLP | RAG | Deep Learning

* GitHub: @Mahmoud3301
* LinkedIn: Mahmoud Saeed Mansour
* Portfolio: Personal Portfolio

⸻

© 2026 Mahmoud Saeed Mansour. All rights reserved to the original project contributions, subject to the applicable license terms and third-party rights.