
# 📊 Análise Exploratória e Preditiva de Criptomoedas (BTC, ETH e BNB)

## 🧩 Descrição do Projeto
Este projeto tem como objetivo realizar uma **análise exploratória de dados (EDA)** e preparar a base para uma **análise preditiva** do valor de mercado de três criptomoedas principais:

- **Bitcoin (BTC)**
- **Ethereum (ETH)**
- **Binance Coin (BNB)**

A análise utiliza dados históricos diários de preços obtidos pela **API pública da Binance**, referentes ao período de **01/05/2017 a 10/11/2025*.

O foco desta primeira entrega é a **Análise Exploratória dos Dados (EDA)**, com a coleta, limpeza, estruturação e observação de padrões, tendências e correlações iniciais entre as variáveis.

---

## 📅 Etapas do Projeto

### 1️⃣ Coleta de Dados
Os dados foram obtidos diretamente da **API da Binance**, usando o endpoint `/api/v3/klines`.  
Cada dataset contém as seguintes colunas:

| Coluna | Descrição |
|--------|------------|
| `open_time` | Data e hora de abertura do candle |
| `open` | Preço de abertura |
| `high` | Preço máximo do período |
| `low` | Preço mínimo do período |
| `close` | Preço de fechamento |
| `volume` | Volume negociado |
| `close_time` | Data e hora de fechamento do candle |
| `num_trades` | Número de negociações realizadas |

---

### 2️⃣ Limpeza e Estruturação
Após a coleta, os dados passam por:
- Conversão de timestamps para o formato de data (`datetime`);
- Conversão das colunas numéricas (`open`, `high`, `low`, `close`, `volume`) para `float`;
- Exportação dos dados limpos em arquivos `.csv`:
  - `bitcoin_2025.csv`
  - `ethereum_2025.csv`
  - `bnb_2025.csv`

---

### 3️⃣ Análise Exploratória (EDA)
Na etapa exploratória, serão analisados:
- Distribuições de preço (abertura, fechamento, volume);
- Variações diárias e médias móveis;
- Correlações entre variáveis;
- Tendências e volatilidade ao longo do tempo.

Gráficos e estatísticas descritivas serão utilizados para compreender melhor o comportamento das moedas no período de 2024.

---

### 4️⃣ (Próxima Entrega) - Análise Preditiva
Na segunda parte do projeto, os dados tratados serão utilizados em **modelos preditivos** para estimar valores futuros das criptomoedas.  
Modelos candidatos incluem:
- **Regressão Linear**
- **ARIMA / Prophet**
- **Redes Neurais Recorrentes (LSTM)**

---

## ⚙️ Como Executar o Projeto

### 🔹 Opção 1 — Google Colab
1. Acesse o link do notebook do projeto (enviado junto à entrega);
2. Execute as células em ordem;
3. Os datasets serão automaticamente baixados e processados.

### 🔹 Opção 2 — Execução Local
1. Clone o repositório:
   ```bash
   git clone https://github.com/usuario/projeto-cripto-analise.git
   cd projeto-cripto-analise
   ```
2. Instale as dependências:
   ```bash
   pip install pandas requests matplotlib seaborn
   ```
3. Execute os scripts:
   ```bash
   python btc_analise.py
   python eth_analise.py
   python bnb_analise.py
   ```

---

## 📁 Estrutura do Projeto

```
📦 projeto-cripto-analise
├── btc_analise.py
├── eth_analise.py
├── bnb_analise.py
├── bitcoin_2024.csv
├── ethereum_2024.csv
├── bnb_2024.csv
├── README.md
└── analise_exploratoria.ipynb
```

---

## 👨‍💻 Integrantes do Grupo

- **Murillo Weiss Kist**  
- **Jean Claudio de Barro**

---

## 🏫 Informações Acadêmicas
**Disciplina:** MIneração de Dados  
**Professor:** *Diogo Stelle*  
**Entrega:** 12/11/2025  
**Instituição:** *FAG*  
