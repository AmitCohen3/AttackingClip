# AttackingClip
An adversarial attack against CLIP model in the textual domain

## Overview

This project demonstrates an adversarial attack on OpenAI’s CLIP model, specifically targeting the textual domain. The goal is to craft adversarial text that maximizes or minimizes the similarity score between the text and a given image. The adversarial text is generated iteratively by modifying embeddings based on gradient-based optimization.

## Features


* Leverages the CLIP model’s text and image embeddings for attack generation.
* Applies gradient-based optimization to craft adversarial text.
* Includes functionality to decode adversarial embeddings back into human-readable text.
* Can optionally target a reference text, reducing its similarity to the adversarial text.


The notebook, AttackingClip.ipynb, includes everything needed to run the attack, provided PyTorch and basic libraries are installed. It uses a customized version of CLIP that enables separate encoding and embedding functionalities for enhanced flexibility

## Example Output

* Attacking Text: “an adversarial example”
* Probability Scores:
* Attacking Text: 0.85
* Reference Text: 0.1
* Other Texts: [0.05, 0.05]

## Notes

* The notebook runs standalone and assumes basic libraries like PyTorch are installed.
* A sample image file (e.g., cat.png) can be used as input.
