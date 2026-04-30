# Previsão de Score de Crédito com Inteligência Artificial

Este projeto aplica técnicas de Machine Learning para automatizar a análise de score de crédito de clientes de um banco. A partir de dados históricos, a Inteligência Artificial aprende a classificar novos clientes em três categorias de risco: **Ruim (Poor), Ok (Standard) ou Bom (Good)**.

## 🚀 Contexto do Desafio
Bancos recebem milhares de solicitações de crédito diariamente. Analisar manualmente o histórico, salário e contas de cada cliente é inviável e sujeito a erros. O objetivo deste projeto é:
1. Analisar uma base de dados com 100.000 clientes.
2. Preparar e codificar os dados para o formato exigido por algoritmos de Machine Learning.
3. Treinar e comparar dois modelos de Inteligência Artificial para escolher o mais preciso.
4. Utilizar o modelo vencedor para prever automaticamente o score de novos clientes.

## 🛠️ Tecnologias Utilizadas
- **Python** 
- **Pandas** (Manipulação e leitura de dados)
- **Scikit-Learn (sklearn)** (Criação e treinamento dos modelos de Machine Learning)
- **Jupyter Notebook** (Ambiente de desenvolvimento)

## 📋 Etapas do Projeto
1. **Importação:** Carregamento do dataset `clientes.csv`.
2. **Pré-processamento (Label Encoding):** Conversão de variáveis categóricas (texto) como `profissao` e `comportamento_pagamento` em valores numéricos para que a IA possa processá-los.
3. **Divisão de Dados:** Separação da base em dados de treino (70%) e teste (30%).
4. **Treinamento de Modelos:** Construção de duas IAs diferentes para fins de comparação:
   - *Random Forest* (Floresta Aleatória)
   - *K-Nearest Neighbors* (KNN - Vizinhos Mais Próximos)
5. **Avaliação:** A *Random Forest* obteve uma performance superior, alcançando **~82.4% de acurácia** nos testes.
6. **Previsão em Produção:** Importação do dataset `novos_clientes.csv` e aplicação do modelo treinado para definir o score de crédito de novos usuários de forma 100% automática.

## 📂 Como Executar
1. Clone este repositório.
2. Certifique-se de que os arquivos `clientes.csv` e `novos_clientes.csv` estejam na mesma pasta do código.
3. Instale as bibliotecas necessárias:
   ```bash
   pip install pandas scikit-learn

   ---

## Desenvolvido por Kauan Santana
