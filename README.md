# MVP - Previsão de Valor FIPE de Veículos

Esta Monografia implementa um modelo de Machine Learning para prever o valor FIPE de veículos baseado em suas característica.

## 📁 Arquivos Entregues

### Arquivos Principais
- **`MVP_Veiculos_Colab.ipynb`** - Notebook Jupyter formatado para Google Colab (ARQUIVO PRINCIPAL)
- **`mvp_veiculos_colab.py`** - Script Python completo com todo o código
- **`veiculos_limpo.csv`** - Dataset limpo e preparado para análise

### Arquivos de Análise
- **`analise_exploratoria.png`** - Gráficos da análise exploratória
- **`comparacao_modelos.png`** - Comparação visual dos modelos
- **`notas_analise.md`** - Documentação da análise inicial

### Arquivos de Apoio
- **`analise_inicial.py`** - Script de análise inicial dos dados
- **`analise_exploratoria.py`** - Script de análise exploratória detalhada
- **`README.md`** - Este arquivo com instruções

## 🚀 Como Usar no Google Colab

### Opção 1: Usar o Notebook (Recomendado)
1. Faça o upload do arquivo `MVP_Veiculos_Colab.ipynb` para o Google Colab
2. Faça o upload do arquivo `veiculos_limpo.csv` quando solicitado
3. Execute as células sequencialmente

### Opção 2: Usar o Script Python
1. Crie um novo notebook no Google Colab
2. Copie e cole o conteúdo do arquivo `mvp_veiculos_colab.py`
3. Faça o upload do arquivo `veiculos_limpo.csv`
4. Execute o código

## 📊 Resultados Obtidos

### Problema Definido
- **Tipo**: Regressão
- **Target**: Valor FIPE
- **Features**: Montadora, Modelo, Cor, Grupo, Situação, Ano Modelo

### Modelos Testados
1. **Linear Regression** (Melhor desempenho)
   - R² = 0.9780
   - MAE = R$ 658.71
   - RMSE = R$ 4,732.00

2. **XGBoost**
   - R² = 0.8979
   - MAE = R$ 1,076.88
   - RMSE = R$ 10,200.96

3. **Random Forest**
   - R² = 0.8817
   - MAE = R$ 1,664.07
   - RMSE = R$ 10,978.81

### Insights Principais
- O modelo Linear Regression teve desempenho surpreendentemente superior
- Correlação moderada (0.366) entre Ano Modelo e Valor FIPE
- Dataset final: 1.048 veículos após limpeza
- Principais montadoras: FIAT, CITROËN, PEUGEOT

## 📋 Checklist do MVP (Conforme PDF)

### ✅ Definição do Problema
- [x] Objetivo claro: Prever Valor FIPE
- [x] Descrição do problema: Regressão
- [x] Premissas definidas
- [x] Restrições para seleção dos dados

### ✅ Preparação de Dados
- [x] Operações de preparação realizadas
- [x] Separação treino/teste (80%/20%)
- [x] Justificativa para não usar validação cruzada (MVP simples)
- [x] Transformações apropriadas (StandardScaler, OneHotEncoder)

### ✅ Modelagem e Treinamento
- [x] Modelos construídos para resolver o problema
- [x] Algoritmos selecionados e justificados
- [x] Verificação de underfitting/overfitting
- [x] Comparação de múltiplos modelos

### ✅ Avaliação de Resultados
- [x] Análise em dados não vistos (conjunto de teste)
- [x] Métricas condizentes (MAE, RMSE, R²)
- [x] Comparação entre modelos
- [x] Melhor solução identificada e justificada

## 🔧 Dependências

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```

## 📈 Próximos Passos Sugeridos

1. **Otimização de Hiperparâmetros**: GridSearchCV/RandomizedSearchCV
2. **Feature Engineering Avançada**: Idade do veículo, combinações de features
3. **Análise de Erros**: Investigar casos de maior erro
4. **Validação Cruzada**: K-Fold para estimativa mais robusta
5. **Inclusão de Mais Dados**: Features adicionais ou dados externos

## 👨‍💻 Autor

Análise realizada com Andre Luiz Marques Serrano - 10/09/2025

---


