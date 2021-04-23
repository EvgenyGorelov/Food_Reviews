# Fine food reviews - sentiment analysis of Amazon data

## Overview
A sentiment analysis of review texts using pre-trained BERT models for classifying
the attitude of the reviewer on a 5 grade scale. This type of analysis is highly relevant 
for companies introducing new products and tracking online reactions.

Over 500 000 reviews from over 250 000 users for over 70 000 products available as text, text summary and score.
Measuring review sentiment could be more precise than analysing just a star-score,
many reviewers use only extreme scores. A users segmentation can be performed for targeted advertising.
Reasons for success/fail of particular products can be identified, as well as
early detection of problematic items.

## Workflow
- BERT - pretrained bidirectional transformer; Main training is already complete
- Only fine tuning needed for particular task - the model can be tuned for sentiment prediction

- Original reviews data has been analyzed and cleaned
- Model training performed on Nvidia GPU
- Only 6 hours training on single GPU needed for 75% accuracy

- Score predicted from review text with 82% accuracy 
- 79k predictions made within 10minutes on single GPU
- Model successfully tested on completely unrelated reviews from TrustPilot

- Score predicted from short summary with 80% accuracy The sentiment of Summary and Text is generally aligned
- The sentiment can be correctly extracted even from a short summary

- Users with multiple reviews can be successfully classified
- Unsupervised machine learning used for users classification
- The reviews from more critical users can be used for early item problem detection
- Users with highest sentiment reviews can be a subject for targeted advertising of similar products
