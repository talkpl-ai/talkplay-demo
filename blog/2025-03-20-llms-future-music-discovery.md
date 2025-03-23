# LLMs are the Future for Music Discovery

Posted on March 20, 2025

It's 2025, and finding music is still surprisingly hard. As someone who has dedicated significant time to music AI - from Spotify to ByteDance - I can say with confidence that we need fresh approaches. Traditional recommendation techniques, while valuable, have shown their limitations.

## Why Bet on LLMs?

The answer lies in the lessons learned from AI research, particularly Rich Sutton's [The Bitter Lesson](http://www.incompleteideas.net/IncIdeas/BitterLesson.html): betting on general-purpose learning systems with scaled computation often outperforms carefully engineered, domain-specific solutions.

The key insight here is end-to-end learning. Current music recommendation systems, including those that use LLMs, typically consist of separate modules:
- A dialogue manager for conversation
- A retrieval system for finding candidates
- A ranking module for final recommendations
- Various feature extractors and embedders

Each module is trained separately, optimized for its specific task. Even recent LLM-based approaches often use the language model as just another module - for dialogue management or feature extraction. This modular approach, while intuitive, has a fundamental limitation: you can't optimize the entire system end-to-end.

## Our Approach with TalkPlay

With TalkPlay, we made a radical bet: transform the entire recommendation process into a single, differentiable token generation task. This means:

1. Every component (dialogue, retrieval, ranking) becomes part of the same neural network
2. The entire system is trained end-to-end through backpropagation
3. Every parameter is optimized for the final goal: finding the right music

This isn't just an architectural choice - it's about enabling continuous, holistic improvement. When you have separate modules, each one can only get marginally better at its specific task. But with end-to-end learning, the entire system can adapt and discover novel ways to connect user intentions with music recommendations.

## Why This Matters

Traditional and hybrid approaches have hit a ceiling because:
- Module boundaries create information bottlenecks
- Separate training means sub-optimal solutions
- You can't backpropagate through discrete module interfaces

TalkPlay breaks through these limitations by making everything differentiable and trainable as one system. This isn't just about architectural elegance - it's about creating a system that can truly learn to understand the deep connections between conversation and music discovery.

## Looking Forward

While it might be tempting to build hybrid systems that give immediate gains, we believe the real breakthroughs will come from fully embracing end-to-end learning. As we continue to develop TalkPlay, our focus remains on pushing the boundaries of what's possible with a single, unified model that can learn and improve holistically.

The future of music discovery isn't in better modules - it's in systems that can learn to make connections we never thought to engineer.

---
*This post is written by Keunwoo Choi, based on our recent work on [TalkPlay](https://arxiv.org/abs/2502.13713).* 