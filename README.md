# Hallucination Detection in LLMs using Reverse Retrieval and Cross-Document Verification

## Overview
This repository contains the implementation of a hallucination detection system for Large Language Models with two novel innovations:
- **Reverse Retrieval**: Decompose claims before evidence search to prevent hallucination contamination
- **Cross-Document Verification**: Aggregate multiple evidence sources with 6-category classification

## Results
| Configuration | Accuracy |
|---------------|----------|
| Baseline (Zero-shot) | 18% |
| Fine-tuned NLI (3 epochs) | 64% |
| Fine-tuned NLI (10 epochs) | **68%** |

Our 125M model outperforms Llama-2-13B (13%) by 55 percentage points.

## Dataset
ME-FEVER (Multi-Evidence FEVER) - 2,663 training claims, 1,238 test claims

## Requirements
See `requirements.txt`

## Usage
Run the notebook in Google Colab with GPU enabled:
`notebooks/final_pipeline.ipynb`
