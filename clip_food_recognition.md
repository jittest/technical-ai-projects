# 🍽️ CLIP-Based Food Image Recognition

## 🧪 Title: Building a Food Image Recognition System with CLIP and Python

In my early exploration of applied AI, I experimented with OpenAI’s CLIP (Contrastive Language–Image Pretraining) model to identify food items in user-uploaded images. The goal was to simulate a lightweight food-tracking or menu-recognition system using open-source tools and a simple local dataset.

## 🎯 Motivation

Accurate food image recognition has applications in nutrition tracking, calorie estimation, and menu digitization. I wanted to understand how vision-language models like CLIP associate visual inputs with natural language labels and evaluate their effectiveness in small, domain-specific tasks like food categorization.

## 🛠️ Approach

Built a Python-based prototype with the following features:
- Accepts a user-uploaded image.
- Compare it with a predefined list of food labels (e.g., “pasta,” “salad,” “pizza”).
- Uses CLIP (ViT-B/32) to encode both the image and text labels into a shared vector space.
- Computes cosine similarity between the image embedding and each label to determine the most likely match.
- Accessed CLIP through the transformers and open_clip libraries.

## 📈 Outcome

The system worked well for clean, well-lit images from standard datasets, achieving ~70–80% accuracy in simple cases. However, it required fine-tuning or more specific prompts for composite dishes or low-quality images.

## 📚 Learnings

- CLIP is powerful for general-purpose visual-text matching but requires prompt engineering or fine tuning to adapt for specialized use cases.
- Multi-modal embedding allows for efficient similarity comparisons between images and text.
- Gained hands-on exposure with image processing, vector similarity and pre-trained vision-language model behavior.
