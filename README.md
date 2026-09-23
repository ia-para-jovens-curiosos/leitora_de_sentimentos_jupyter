# 💬 IA para Jovens Curiosos — Leitora de Sentimentos

[![GitHub Repo](https://img.shields.io/badge/GitHub-ia--para--jovens--curiosos%2Fleitora__de__sentimentos__jupyter-blue?logo=github)](https://github.com/ia-para-jovens-curiosos/leitora_de_sentimentos_jupyter)

Um projeto para crianças treinarem sua própria Inteligência Artificial para ler frases digitadas e
adivinhar se estão **positivas**, **negativas** ou **neutras** — sem câmera, sem internet, só Python.

Esta é a versão **Jupyter/PyCharm** do projeto. Existe também a versão
[`leitora_de_sentimentos_colab`](https://github.com/ia-para-jovens-curiosos/leitora_de_sentimentos_colab),
que roda direto no navegador pelo Google Colab.

## Como abrir

Abra o arquivo `sample.ipynb` no Jupyter/PyCharm e execute as células de cima para baixo, com
`Shift + Enter`.

O notebook guia você por cinco passos:

1. **Dados de treino** — a turma monta, em grupo, as listas de palavras positivas e negativas
2. **Limpar a frase** — deixar o texto digitado pronto para comparar (minúsculas, sem pontuação)
3. **Classificar** — a função que decide se a frase é positiva, negativa ou neutra
4. **Testar** — conferir o robô com frases já conhecidas e ajustar as listas quando ele errar
5. **Modo estande** — deixar o programa rodando para o público testar na exposição

Há também uma célula opcional de **modo avançado**, comparando o robô caseiro com uma IA
profissional de verdade (Hugging Face).

## Como funciona por baixo dos panos

Diferente do projeto de Pedra-Papel-Tesoura, aqui **nada fica escondido**: as listas de palavras e a
função `classificar_sentimento()` ficam à vista, dentro do próprio notebook — é literalmente assim
que a turma "programa" a IA. O robô não entende a frase como uma pessoa; ele só reconhece as
palavras que estiverem nas listas de treino que a turma escreveu.

## Ambiente

Este projeto usa só **Python puro** (biblioteca `re`, já incluída) — não precisa instalar nada para
rodar os passos 1 a 5. O arquivo `requirements.txt` só é necessário se a turma quiser tentar a célula
opcional de **modo avançado**, que baixa um modelo de linguagem real (`transformers`).

```
pip install -r requirements.txt
```
