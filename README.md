# RAG-introduction

## Setup

Clone o repositório com o comando
```
git clone git@github.com:andrecaraiba/RAG-introduction.git
```

### Ambiente Virtual e Dependências
Nesse projeto, o [poetry](https://python-poetry.org/docs/basic-usage/) foi utilizado como gerenciador de dependências, em conjunto com o [conda](https://docs.anaconda.com/miniconda/) para gerenciar ambientes virtuais. Para instalação do conda siga os passos descritos nas respectivas documentações.

Se estiver usando Linux, poderá instalar o poetry seguindo as seguintes instruções:

Instalar [pipx](https://github.com/pypa/pipx)
``` bash
$ sudo apt update
$ sudo apt install pipx
$ pipx ensurepath
$ sudo pipx ensurepath --global
```

Instalar poetry
```bash
pipx install poetry
```

Após isso, crie e ative seu ambiente virtual, com o conda crie um ambiente chamado 'rag' com a versão 3.10.4 do python.
```bash
$ conda create -n rag python=3.10.4
$ conda activate rag
```

Para instalar todas as dependências listadas no `arquivo pyproject.toml` no ambiente virtual usando poetry use o seguinte comando dentro da pasta do projeto.
```bash
$ poetry install
```

### Ollama
O [Ollama](https://ollama.com/) será usado para servir o modelo Llama 3.1 8B na pipeline do RAG. Para usuários da plataforma Linux, siga os seguintes passos para fazer o download do Ollama e donwload do Llama3.1 8B.

```bash
$ curl -fsSL https://ollama.com/install.sh | sh
$ ollama run llama3.1
```

Para instalação do Ollama em outros sistemas operacionais como Macos e Windows consulte a documentação [Ollama install](https://ollama.com/).

