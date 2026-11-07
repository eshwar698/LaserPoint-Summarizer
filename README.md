\# LaserPoint



\*\*Fine-tuning Mistral-7B-Instruct for abstractive text summarization and local inference.\*\*



LaserPoint is an experimental language model developed during a research internship at Digital University Kerala. The project explores parameter-efficient fine-tuning, dataset preparation, model conversion, and local deployment of a summarization-focused LLM.



\## Project Overview



LaserPoint adapts Mistral-7B-Instruct-v0.1 for summarization using supervised fine-tuning and Low-Rank Adaptation (LoRA).



The workflow covers:



\- Dataset preparation and formatting for supervised fine-tuning

\- 4-bit quantized model loading for memory-efficient training

\- LoRA-based parameter-efficient fine-tuning

\- Model saving and conversion to GGUF

\- Local inference using llama.cpp

\- A lightweight HTML interface for interacting with the local model



\## Technology Stack



\- Python

\- Mistral-7B-Instruct-v0.1

\- Hugging Face Transformers

\- PEFT / LoRA

\- BitsAndBytes

\- Hugging Face Datasets

\- llama.cpp

\- GGUF

\- HTML / JavaScript



\## Project Structure



```text

LaserPoint-Summarizer/

├── README.md

├── .gitignore

├── Untitled17.ipynb

└── chat.html

```



\## Training



The original experimental notebook is preserved as `Untitled17.ipynb`.



The notebook contains the model loading, dataset processing, LoRA configuration, and training workflow.



Key configuration:



| Parameter | Value |

|---|---|

| Base model | Mistral-7B-Instruct-v0.1 |

| Fine-tuning | LoRA |

| Quantization | 4-bit |

| LoRA rank | 16 |

| LoRA alpha | 32 |

| LoRA dropout | 0.05 |

| Training epochs | 3 |



\## Local Inference



The model was converted to GGUF format and tested using llama.cpp.



A lightweight HTML chat interface communicates with a locally running inference server through an OpenAI-compatible API endpoint.



The model files and inference binaries are not included in this repository.



\## Limitations



\- Experimental project focused on summarization.

\- Model performance depends on the training dataset and configuration.

\- Generated summaries may omit information or introduce inaccuracies.

\- Local inference requires separately obtained model files and compatible inference software.



\## Acknowledgment



Developed as part of a research internship at Digital University Kerala.



\## License



To be determined.



