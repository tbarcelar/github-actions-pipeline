# GitHub Actions: Python CI Pipeline 🚀

Este repositório demonstra como configurar uma pipeline de Integração Contínua (CI) usando **GitHub Actions** para executar scripts Python automaticamente.

## Visão Geral 📋

A pipeline realiza as seguintes etapas ao detectar um `push` no branch `main`:

1. Faz o checkout do repositório.
2. Configura o ambiente Python.
3. Instala as dependências necessárias.
4. Executa um script Python localizado em `.github/workflows/script.py`.

## Estrutura do Repositório 📂

- **`.github/workflows/ci.yml`**: Arquivo de configuração da pipeline do GitHub Actions.
- **`.github/workflows/script.py`**: Script Python simples que é executado pela pipeline.

## Configuração da Pipeline 🔧

O arquivo `ci.yml` define a pipeline. 


Explicação:
Disparador (on):

A pipeline é acionada quando há um push no branch main.
Ambiente (runs-on):

A pipeline é executada em um ambiente Ubuntu mais recente (ubuntu-latest).
Etapas (steps):

Checkout: Clona o repositório no ambiente de execução.
Configuração do Python: Configura o Python 3.x.
Instalação de dependências: Atualiza o pip (não há dependências adicionais neste exemplo).
Execução do script: Roda o arquivo script.py.
O Script Python 🐍
O arquivo script.py é um exemplo simples que imprime uma mensagem no console:


Como Usar 🚀
Faça um push ou merge no branch main.
Acesse a aba Actions no repositório para visualizar o progresso da pipeline.
Verifique os logs para garantir que o script Python foi executado com sucesso.
Melhorias Futuras 🌟
Adicionar testes automatizados com frameworks como pytest.
Configurar a pipeline para instalar dependências listadas em um requirements.txt.
Expandir o script para incluir funcionalidades mais complexas.
Autor: tbarcelar
Licença: MIT 📜