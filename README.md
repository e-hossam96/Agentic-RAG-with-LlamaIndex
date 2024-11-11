# Agentic-RAG-with-LlamaIndex

Building Multi-Document Agentic RAG with LlamaIndex.

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
