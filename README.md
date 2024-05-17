# Chatbot de Agendamento de Consultas

Este é um projeto de um chatbot desenvolvido com o Rasa para facilitar o agendamento de consultas médicas.

## Funcionalidades

- O chatbot é capaz de receber solicitações de agendamento de consulta.
- Ele pode solicitar informações sobre a especialidade desejada, dia e horário da consulta.
- O chatbot confirma o agendamento com o usuário.
- Ele também pode cancelar uma consulta previamente agendada.

## Pré-requisitos

- Python 
- Rasa 3.1

## Instalação

1. Clone este repositório:

```bash
git clone https://github.com/seuusuario/chatbot-agendamento-consulta.git

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Graziele-Rodrigues/demo-Rasa-Bot/HEAD)
```
2. Instale as dependências:

```bash
cd chatbot-agendamento-consulta
pip install -r requirements.txt
```

## Uso

1. Treine o modelo Rasa:

```bash
rasa train
```

2. Inicie o servidor de ações:

```bash
rasa run actions
```
3. Inicie o servidor do chatbot:
```bash
rasa run -m models --enable-api --cors "*" --debug
```

## Arquivos do Projeto
- data/nlu.yml: Contém os exemplos de frases para treinamento do modelo NLU.
- data/stories.yml: Contém as histórias de conversação para treinamento do modelo de políticas de conversação.
- data/rules.yml: Contém as regras de conversação para o chatbot.
- domain.yml: Define o domínio do chatbot, incluindo intenções, entidades, slots e respostas de ação.
- config.yml: Arquivo de configuração do Rasa.
- actions.py: Define as ações personalizadas do chatbot.

## Licença
Este projeto está licenciado sob a Apache License.