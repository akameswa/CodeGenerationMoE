## CodeGenerationMoE

A Mixture-of-Experts (MoE) approach to code generation using Mistral-7B as the base model.

### Overview
This project explores the efficacy of the Mixture-of-Experts (MoE) framework in code generation, demonstrating significant performance improvements compared to monolithic model architecture. Using Mistral-7B as the base model, we developed specialized experts for different programming languages (Python, C++, Java, and JavaScript).

### Key Features
- Fine-tuned models for specific programming languages
- MoE architecture with specialized experts
- 51% performance improvement over baseline using CodeBLEU benchmark
- Resource-efficient implementation using QLoRA and PEFT

### Results
| Language   | Baseline | Fine-tuned |
|------------|----------|------------|
| Python     | 0.1800   | 0.4000     |
| Java       | 0.1860   | 0.4287     |
| JavaScript | 0.1909   | 0.4182     |
| C++        | 0.2170   | 0.3340     |

### Technical Details
- Base Model: Mistral-7B
- Training Infrastructure: AWS A10G GPU
- Evaluation Metric: CodeBLEU
- Dataset: xlcost-text-to-code from Hugging Face

### Resources
- [Video presentation](https://www.youtube.com/watch?v=FjxlqdsM-KI)
- [Final Report](docs/final_report.pdf)

### Future Work
- Enhanced dataset curation
- Refinement of model architecture
- Expanded evaluation metrics
- Instruction tuning
- Model alignment using RLHF/DPO
