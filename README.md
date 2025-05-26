# Previsão de Séries Temporais com Redes Neurais Recorrentes (RNNs)

As RNNs (Redes Neurais Recorrentes) são um tipo de rede neural especialmente projetado para lidar com **dados sequenciais ou temporais**, como séries temporais financeiras, sensores ambientais, ou qualquer dado que tenha dependência do tempo.

Diferentemente das redes neurais tradicionais, as RNNs possuem **memória interna**, permitindo que informações de entradas anteriores influenciem o resultado atual. Isso as torna ideais para prever comportamentos futuros com base em padrões anteriores.

### Por que RNNs são eficientes?

- Mantêm um **estado interno (memória)** das entradas anteriores
- Modelam dependências temporais de curto e longo prazo
- São fundamentais em aplicações como **tradução automática, previsão de séries temporais, e reconhecimento de fala**
- Podem ser expandidas com variantes como **LSTM** e **GRU** para melhor performance

### Exemplo intuitivo

Imagine tentar prever o preço de uma ação amanhã. É natural considerar não apenas o preço de hoje, mas também o comportamento dos últimos dias. As RNNs fazem exatamente isso: **lembram do passado para prever o futuro**.

---

## 📂 Estrutura dos Notebooks

### 1. `RNN1_Bolsa_uma_saida_Orlando.ipynb`
**📌 Tarefa:** Previsão de preço futuro com uma única saída  
**📚 Dataset:** Série temporal da Bolsa de Valores  
**🔍 Destaques:**
- Uso de uma única variável como entrada
- Previsão de uma única etapa futura
- Visualização da série real vs. prevista

### 2. `RNN2_Multiplos_previsores_Orlando.ipynb`
**📌 Tarefa:** Previsão com múltiplos atributos de entrada  
**📚 Dataset:** Série com diversas variáveis explicativas  
**🔍 Destaques:**
- Uso de múltiplos preditores (features)
- Preparação dos dados com múltiplas colunas
- Otimização da estrutura da RNN para lidar com entradas complexas

### 3. `RNN3_Multiplas_saidas_Orlando.ipynb`
**📌 Tarefa:** Previsão de múltiplas etapas futuras (horizonte temporal)  
**📚 Dataset:** Série temporal multivariada  
**🔍 Destaques:**
- Arquitetura para previsões em sequência
- Saídas múltiplas para prever vários dias à frente
- Comparação visual entre sequência real e prevista

### 4. `RNN4_Multiplas_entradas_e_saidas_Orlando.ipynb`
**📌 Tarefa:** Previsão com múltiplas variáveis de entrada e múltiplas saídas  
**📚 Dataset:** Série temporal com várias variáveis e horizonte estendido  
**🔍 Destaques:**
- Entrada com vários preditores
- Previsão simultânea de várias saídas
- Estrutura robusta de entrada/saída em formato 3D (samples, time_steps, features)

### 5. `RNN5_Poluicao_China_Orlando.ipynb`
**📌 Tarefa:** Previsão de poluição ambiental na China  
**📚 Dataset:** Dados históricos de poluentes atmosféricos  
**🔍 Destaques:**
- Aplicação real em dados ambientais
- Pré-processamento robusto e normalização
- Interpretação de tendências e variações sazonais

---

## 📈 Métricas de Avaliação

As RNNs foram avaliadas com as métricas de:

- **Erro Médio Absoluto (MAE)**
- **Erro Quadrático Médio (MSE)**
- **Visualização temporal das previsões**
- **Comparação entre série real e prevista**
"""
