# Attention-guided Chained Context Aggregation for Semantic Segmentation on Indian Driving Dataset
 
Final Observation

Encoder: Here in Attention mechanism simple encoder is used

Decoder: In decoder block I used slightly different architecture With attention mechanism

In this projet, I applied One Step Decoder Which Apply Attention Mechanism and Decoder Block Step by Step for Each Time-stamp.. So Basically, Vanila Encoder-Decoder Can not work Excellently when Machine Translation Task contains Long Sequences.... that's Why Attention Based Mechanism Comes in Picture, Attention Layer Finds the Word from Input Space which help alot to translate the word in other Language for specific Timestamp by Calculating the Score

In this I used Luong - Style Attention Which is very similar to Bahadanau Attention, but the slight difference is in Calculating Score for Global Attention. Paper. https://arxiv.org/pdf/1508.04025.pdf

So Luong-style Attention have the three Scoring Methods 1) Dot-Score 2) General-Score 3) Concat-Score

After Applying the All three score in Training Process we used The BLEU Score for Evaluation Process .

We got same Bleu- Score Aroung --> 0.61 in Case of applying Dot and General Score in Attention Mechanism But with Concat Score we get slighty good BLUE Result --> 0.6687
