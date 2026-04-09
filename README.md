# 🎙️ Assistente de Acessibilidade por Voz

Assistente inteligente que responde perguntas por voz sobre qualquer texto ou PDF,
com respostas sempre em português. Desenvolvido com Whisper, ChatGPT e gTTS no Google Colab.

## Como funciona

1. O usuário insere um texto ou faz upload de um PDF
2. Faz perguntas por voz sobre o conteúdo
3. O Whisper transcreve o áudio
4. O ChatGPT responde em linguagem simples e acessível
5. O gTTS lê a resposta em voz alta

## Tecnologias utilizadas

- [Whisper](https://github.com/openai/whisper) — transcrição de voz
- [OpenAI API](https://platform.openai.com) — geração de respostas
- [gTTS](https://pypi.org/project/gTTS/) — síntese de voz
- [PyPDF2](https://pypi.org/project/PyPDF2/) — leitura de PDFs

## Pré-requisitos

### API Key da OpenAI
Este projeto utiliza a API da OpenAI, que é um serviço pago.
Antes de executar, você precisa:

1. Criar uma conta em [platform.openai.com](https://platform.openai.com)
2. Adicionar crédito em [Billing](https://platform.openai.com/settings/billing) (mínimo $5)
3. Gerar uma chave em [API Keys](https://platform.openai.com/api-keys)
4. Colar sua chave na Célula 2 do notebook

> Sem saldo na conta OpenAI, a execução retornará erro 429 (quota exceeded).

### Microfone
Permita o acesso ao microfone quando o navegador solicitar.
Você terá 5 segundos para falar sua pergunta (ajustável na variável `DURATION` da Célula 5).

## Como usar

1. Abra o notebook no Google Colab
2. Execute as células em ordem (1 → 2 → 3 → 4)
3. Para cada pergunta: execute a Célula 5 (grava) → Célula 6 (processa)
4. Para encerrar: fale **"finalizar assistente"** durante a gravação

## Casos de uso

- Tirar dúvidas sobre bulas de medicamento
- Entender contratos e documentos jurídicos
- Acessar conteúdo acadêmico de forma simplificada
- Qualquer texto denso que precise de explicação acessível
