# Agentic-RAG-with-LlamaIndex

Building Multi-Document Agentic RAG with LlamaIndex. This repository is an implementation of the short course [Building Agentic RAG with LlamaIndex](https://www.deeplearning.ai/short-courses/building-agentic-rag-with-llamaindex/).

The idea is to define a vector store tool and a summary tool for each document (research papers in this case). When number of tools gets large, we can define a tool retriever that works as a vector tool over the documents tools. This way we can ensure LLMs are not overwhelmed with the excessive number of tools and still calls the tools we need based on the query.

Each branch in this repository represents a lesson. The final branch `4-multi-docs-agent` contains the final version of the functions we could define and run sequentially to automate the process.

## Setup

- Clone this repository.

```bash
git clone https://github.com/e-hossam96/Agentic-RAG-with-LlamaIndex.git
```

- Download and install Miniconda

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh -b -p ./miniconda
```

- Activate conda `base` environment.

```bash
source ./miniconda/bin/activate
```

- Create **agentic-rag** env from [YAML](./environment.yml) file

```bash
cd Agentic-RAG-with-LlamaIndex
conda env create
conda activate agentic-rag
```

- Fill [.env.example](./.env.example) file and save it into a `.env` file.

```bash
cp .env.example .env
```
