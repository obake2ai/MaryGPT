![levi_pi_vis](https://github.com/user-attachments/assets/4faa13db-eee0-4198-91b4-3599e1d282ad)

# MaryGPT Model Card

MaryGPT is a is a text generation model and a fine-tuned version of [GPT-J 6B](https://huggingface.co/EleutherAI/gpt-j-6b).

This model is **fine-tuned exclusively on text from Mary Shelley's 1818 novel ["Frankenstein; or, The Modern Prometheus"](https://www.gutenberg.org/ebooks/84)**.

This will be used as a base model for [**AI Artist Yuma Kishi👤**](https://obake2ai.com/)’s activity, including art creation and exhibition curation. 

## Training Data Sources
All data was obtained ethically and in compliance with the site's terms and conditions.
No copyright texts are used in the training of this model without the permission.

- GPT-J 6B was trained on [the Pile](https://pile.eleuther.ai), a large-scale curated dataset created by [EleutherAI](https://www.eleuther.ai).
- Frankenstein; or, The Modern Prometheus, 1818 (Public domain)

## Training procedure
This model was trained for 402 billion tokens over 383,500 steps on TPU v3-256 pod. It was trained as an autoregressive language model, using cross-entropy loss to maximize the likelihood of predicting the next token correctly.

## Developed by
MaryGPT
- [Yuma Kishi](https://x.com/obake_ai)

GPT-J
- [James Bradbury](https://twitter.com/jekbradbury) for valuable assistance with debugging JAX issues.
- [Stella Biderman](https://www.stellabiderman.com), [Eric Hallahan](https://twitter.com/erichallahan), [Kurumuz](https://github.com/kurumuz/), and [Finetune](https://github.com/finetuneanon/) for converting the model to be compatible with the `transformers` package.
- [Leo Gao](https://twitter.com/nabla_theta) for running zero shot evaluations for the baseline models for the table.
- [Laurence Golding](https://github.com/researcher2/) for adding some features to the web demo.
- [Aran Komatsuzaki](https://twitter.com/arankomatsuzaki) for advice with experiment design and writing the blog posts.
- [Janko Prester](https://github.com/jprester/) for creating the web demo frontend.
