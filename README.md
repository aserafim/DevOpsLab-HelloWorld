# DevOpsLab-HelloWorld

Este repositório contém um projeto de exemplo utilizado para práticas de integração e entrega contínua (CI/CD) dentro do contexto de DevOps. O objetivo é demonstrar conceitos básicos de automação de pipeline, versionamento e deploy de aplicações simples.

## 🚀 Descrição

O projeto implementa uma aplicação simples em Python que exibe uma mensagem "Hello, World!" via linha de comando ou via servidor web (dependendo da versão que você executar). Este laboratório serve como base para explorar ferramentas e práticas como:

- Git e GitHub
- Pipeline de CI/CD
- Containers (Docker)
- Automação com GitHub Actions
- Boas práticas de versionamento de código

## 🛠️ Tecnologias e Ferramentas

- **Python 3.x**
- **Docker**
- **GitHub Actions**
- **Git**
- **Linux/MacOS/Windows (compatível)**

## 📁 Estrutura do Projeto

```plaintext
DevOpsLab-HelloWorld/
├── .github/           # Workflows do GitHub Actions
├── app/               # Código-fonte da aplicação
│   └── main.py
├── Dockerfile         # Arquivo para criação da imagem Docker
├── requirements.txt   # Dependências Python
├── LICENSE
├── README.md          # Este arquivo
└── .gitignore         # Arquivos ignorados pelo git
```

## 🐳 Executando com Docker
## Build da imagem

```bash
docker build -t devopslab-helloworld .
```

## Rodando o container

```bash
docker run -p 5000:5000 devopslab-helloworld
```

Acesse no navegador: http://localhost:5000/

## 🧪 Executando Localmente (sem Docker)
## Pré-requisitos

- Python 3.x instalado na sua máquina

## Passos
1. Instale as dependências:
```bash
pip install -r requirements.txt
```

2. Execute a aplicação:
```bash
python app/main.py
```

## 🔄 Pipeline CI/CD

Este repositório contém um workflow automatizado com GitHub Actions, que realiza:

- Instalação de dependências
- Execução de testes
- Build da imagem Docker
- Publicação em repositórios (opcional)

O arquivo do pipeline está localizado em:
```bash
.github/workflows/main.yml
```

## 📝 Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.
