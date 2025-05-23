# Student Habits and Performance Analysis

Este projeto explora a relação entre os hábitos de vida dos estudantes e seu desempenho acadêmico, por meio de análise exploratória de dados, engenharia de atributos, visualizações, análise de informação mútua e clustering com K-Means.

## Objetivo

Investigar como fatores como hábitos de estudo, uso de redes sociais, sono, dieta, saúde mental e participação em atividades extracurriculares afetam a **nota final dos estudantes (`exam_score`)**, além de segmentar perfis de estudantes com base em características comuns.

## Tecnologias e Bibliotecas

- Python 3
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- PCA (Análise de Componentes Principais)
- K-Means (implementação manual)

## Dataset

O conjunto de dados está localizado em: [Student Habits vs Academic Performance](https://www.kaggle.com/datasets/jayaantanaath/student-habits-vs-academic-performance/data)

### Principais colunas do dataset:

- **Variáveis Numéricas:**
  - `age`, `study_hours_per_day`, `social_media_hours`, `netflix_hours`, `attendance_percentage`, `sleep_hours`, `exercise_frequency`, `mental_health_rating`
  
- **Variáveis Categóricas:**
  - `gender`, `part_time_job`, `diet_quality`, `parental_education_level`, `internet_quality`, `extracurricular_participation`
  
- **Variável Alvo:**
  - `exam_score`

## Etapas do Projeto

1. **Pré-processamento**
   - Normalização de atributos numéricos com `StandardScaler`
   - Codificação de atributos categóricos com `OneHotEncoder`

2. **Análise Exploratória de Dados**
   - Criação de gráficos de barras para verificar a relação entre cada atributo e a média de `exam_score`
   - Binagem de variáveis numéricas para facilitar a visualização

3. **Avaliação de Informação Mútua**
   - Cálculo do quanto cada atributo contribui individualmente para prever a `exam_score`

4. **Clustering com K-Means**
   - Implementação manual do algoritmo
   - Determinação do número ideal de clusters com o método do cotovelo
   - Visualização dos clusters com PCA

5. **Análise dos Clusters**
   - Boxplot para avaliar a distribuição de notas por cluster
   - Tabela resumo com a média de atributos por grupo

## Exemplos de Visualizações

- Gráficos de barras mostrando o impacto de cada variável em `exam_score`
- Elbow method para escolha de k ideal
- Visualização 2D dos clusters usando PCA
- Boxplots comparando desempenho por cluster

## Resultados Esperados

- Compreender quais hábitos têm maior correlação com o desempenho acadêmico.
- Identificar perfis de estudantes com características semelhantes e diferentes padrões de desempenho.

## Como Executar

Certifique-se de ter instalado:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
