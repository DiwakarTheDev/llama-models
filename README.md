# 🦙 LLaMA: Open and Efficient Foundation Language Models

LLaMA (Large Language Model Meta AI) is a family of state-of-the-art foundational language models developed by [Meta AI](https://ai.meta.com/).  
It is designed to be **efficient**, **scalable**, and **accessible** for researchers, developers, and the open-source community.  

---

## 🚀 Features
- Multiple model sizes: **7B, 13B, 30B, 65B** parameters
- Optimized for **training efficiency** and **inference speed**
- Supports **research in NLP, reasoning, coding, and more**
- Open weights available under a community-friendly license

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/facebookresearch/llama.git
cd llama
````

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🔑 Accessing Weights

To download LLaMA model weights:

1. Fill out the [Meta AI request form](https://ai.meta.com/llama/)
2. Once approved, you’ll receive download instructions.
3. Place the weights in the `./checkpoints` folder.

---

## 🖥️ Usage

Example: Running text generation with a 7B model

```python
from llama import LLaMA

# Load model
model = LLaMA.load("checkpoints/llama-7b")

# Generate text
prompt = "Once upon a time in AI research..."
output = model.generate(prompt, max_length=100)

print(output)
```

---

## 📊 Model Variants

| Model     | Parameters | Memory (FP16) | Use Case                          |
| --------- | ---------- | ------------- | --------------------------------- |
| LLaMA-7B  | 7 Billion  | \~13 GB       | Small-scale research, prototyping |
| LLaMA-13B | 13 Billion | \~24 GB       | General NLP tasks                 |
| LLaMA-30B | 30 Billion | \~60 GB       | Complex reasoning                 |
| LLaMA-65B | 65 Billion | \~120 GB      | Cutting-edge research             |

---

## 📚 Resources

* [Research Paper](https://arxiv.org/abs/2302.13971)
* [Model Card](https://ai.meta.com/llama/)
* [Community Discussions](https://github.com/facebookresearch/llama/discussions)

---

## 🤝 Contributing

We welcome contributions!

* Open an issue for bug reports or feature requests
* Submit pull requests to improve docs, code, or tooling

Please follow the [contributing guidelines](CONTRIBUTING.md).

---

## 📄 License

LLaMA is released under the [Meta AI license agreement](LICENSE).
Please review the terms before using the models.

---

## 🌟 Citation

If you use **LLaMA** in your research or work, please cite the following paper:

> **LLaMA: Open and Efficient Foundation Language Models**  
> Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurélien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample  
> *arXiv preprint arXiv:2302.13971, 2023*  
> [📄 Read on arXiv](https://arxiv.org/abs/2302.13971)

```bibtex
@article{touvron2023llama,
  title={LLaMA: Open and Efficient Foundation Language Models},
  author={Touvron, Hugo and Lavril, Thibaut and Izacard, Gautier and Martinet, Xavier and Lachaux, Marie-Anne and Lacroix, Timothée and Rozière, Baptiste and Goyal, Naman and Hambro, Eric and Azhar, Faisal and Rodriguez, Aurélien and Joulin, Armand and Grave, Edouard and Lample, Guillaume},
  journal={arXiv preprint arXiv:2302.13971},
  year={2023}
}

