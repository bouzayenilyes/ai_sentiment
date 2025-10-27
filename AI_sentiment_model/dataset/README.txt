AI Sentiment Analysis Project - Dataset Information
===============================================

Repository: https://github.com/bouzayenilyes/ai_sentiment
Author: Ilyes Bouzayen
Contact: bouzayen.ilyes@gmail.com

This repository contains both the AI model training code and the SaaS web application for video sentiment analysis.

PROJECT STRUCTURE
=================

ai_sentiment/
├── AI_sentiment_model/          # PyTorch model training and deployment
│   ├── training/               # Model training scripts
│   ├── deployment/             # AWS SageMaker deployment
│   ├── dataset/                # Dataset files and documentation
│   │   └── README.txt          # This file
│   └── README.md               # Model documentation
├── AI_sentiment_SASS/          # Next.js web application
│   ├── src/                    # Application source code
│   ├── prisma/                 # Database schema
│   └── README.md               # SaaS documentation
└── README.md                   # Main repository README

MELD DATASET INFORMATION
=======================

This project uses the Multimodal EmotionLines Dataset (MELD) for training the sentiment analysis model.

Dataset Details:
- Source: Friends TV Series
- Utterances: 13,000+
- Dialogues: 1,300+
- Emotions: 7 categories (Anger, Disgust, Sadness, Joy, Neutral, Surprise, Fear)
- Sentiment: 3 categories (Positive, Negative, Neutral)
- Modalities: Text, Audio, Video

DATA FILES
==========

The dataset should be downloaded from the official MELD website:
https://affective-meld.github.io

Required files:
- train_sent_emo.csv - Training set with sentiment and emotion labels
- dev_sent_emo.csv   - Development/validation set
- test_sent_emo.csv  - Test set
- Video files (.mp4) - Raw video clips for each dialogue

INSTALLATION
============

1. Download the MELD dataset from https://affective-meld.github.io
2. Extract the dataset files to this directory (AI_sentiment_model/dataset/)
3. Ensure the CSV files and video files are in the correct locations

USAGE
=====

The dataset is used by the training scripts in the ../training/ directory.
See ../README.md for detailed training instructions.

CITATION
========

If you use this dataset in your research, please cite:

S. Poria, D. Hazarika, N. Majumder, G. Naik, E. Cambria, R. Mihalcea.
Multimodal EmotionLines: A Multimodal Multi-Party Dataset for Emotion Recognition in Conversation. (2018)

Chen, S.Y., Hsu, C.C., Kuo, C.C. and Ku, L.W.
EmotionLines: An Emotion Corpus of Multi-Party Conversations. arXiv preprint arXiv:1802.08379 (2018).

LICENSE
=======

This dataset is provided under the same license as the original MELD dataset.
Please refer to the official MELD website for licensing information.

CONTACT
=======

For questions about this repository or the implementation:
- GitHub: https://github.com/bouzayenilyes/ai_sentiment
- Email: bouzayen.ilyes@gmail.com

For questions about the MELD dataset itself, please contact the original authors.
