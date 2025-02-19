# talkplay-demo

## TalkPlay: Multimodal Music Recommendation with Large Language Models

We present TalkPlay, a multimodal music recommendation system that reformulates the recommendation task as large language model token generation. TalkPlay represents music through an expanded token vocabulary that encodes multiple modalities - audio, lyrics, metadata, semantic tags, and playlist co-occurrence. Using these rich representations, the model learns to generate recommendations through next-token prediction on music recommendation conversations, that requires learning the associations natural language query and response, as well as music items. In other words, the formulation transforms music recommendation into a natural language understanding task, where the model's ability to predict conversation tokens directly optimizes query-item relevance. Our approach eliminates traditional recommendation-dialogue pipeline complexity, enabling end-to-end learning of query-aware music recommendations. In the experiment, TalkPlay is successfully trained and outperforms baseline methods in various aspects, demonstrating strong context understanding as a conversational music recommender.

