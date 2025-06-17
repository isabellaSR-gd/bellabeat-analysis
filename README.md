# Análise de uso de fitness trackers - busca por oportunidades de negócio e marketing para Bellabeat
Como dados de padrão e tendências de uso podem informar o marketing de fitness tracker 

# Analistas: 
* [Isabella Rodolfo](https://github.com/isabellaSR-gd)
* [Nínive Helen](https://github.com/ninivehelen)

# Objetivo
Identificar padrões de uso analisando dados do FitBit (fitness tracker similar ao Bellabeat) e gerar insights e apontar oportunidades de negócio para o Bellabeat Fitness tracker.


# Insights principais obtidos
### Tendências de uso de aparelhos smart
* Features mais usadas: **resumo de atividade diária**, **contagem de calorias** e **intensidade de exercício**
* **Predominância de exercícios leves**
* Uso mesmo em dias **sem dedicação à atividade física**
### Como essas tendências podem ser aplicadas aos clientes do Bellabeat?
* Direcionar marketing para mulheres de 18 a 40 anos
* Direcionar para prática de exercícios leves
* Bellabeat como 'companion app'
### Como essas tendências podem ajudar a influenciar as estratégias de marketing do Bellabeat?
* Saber que usuárias praticam exercícios leves e usam o device de forma casual informa o tom dos planos de marketing.
* Não há dados o suficiente para afirmar que pessoas acima do peso são subrepresentadas na base de usuários do Fitbit, mas com a crescente população acima do peso, direcionar o marketing também para esse público é uma oportunidade.

# Estrutura do repositório
* **/analise:** arquivos .ipynb de análises exploratórias, um para cada dataset
* **/database:** pasta para csvs brutos e tratados do projeto
* **/documentos:** arquivos finais sobre conclusões e documentação de limpeza
     * Bellabeat_final_analysis.pdf
     * documentacao_limpeza.md
* **/graficos:** arquivos .ipynb para criação de gráficos com biblioteca Seaborn
* **/limpeza_processamento:** arquivos .ipynb usados para limpar e processar os dados

# Metodologia/ escopo e processo
1. Análise de requisitos, reuniões e definição de datasets a serem usados: estudo de como os dados poderiam responder as perguntas de negócio 
2. Carregamento e processamento de dados: organização de projeto, limpeza e processamento dos dados para as necessidades do projeto
3. Análise exploratória: análises estatísticas, correlações e padrões nos dados
4. Coleta de insights potenciais e alinhamento com perguntas de negócio: organização dos insights para finalizar projeto
5. Criação de gráficos para visualizar achados: uso de biblioteca Seaborn para comunicar de forma simples e direta
6. Documentação: organização de achados em apresentação e documentação de limpeza.

# Datasets usados:
### Dataset principal
* [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)
   * [Dicionário dos dados](https://www.fitabase.com/media/1748/fitabasedatadictionary.pdf)

### Dataset de suporte (preencher lacunas do dado principal)
* [Health and lifestyle dataset](https://www.kaggle.com/datasets/mahdimashayekhi/health-and-lifestyle-dataset)
* [Obesity Dataset](https://www.kaggle.com/datasets/suleymansulak/obesity-dataset)

# Aviso sobre os dados
As bases de dados são limitadas, servindo como análise exploratória inicial para levantar hipóteses, que devem ser confirmadas em bases de dados maiores (maior nível de confiança):
* Database Fitbit
   * Amostra de poucas pessoas e período curto (32 dias) 
   * Primeiros 15 dias do dataset apresentam apenas 2 ids ativos
   * Não há informação do modelo do aparelho health tracker usado por cada Id
* Database Health lifestyle
   * amostra de 1000 pessoas, sendo 477 mulheres

# Potenciais de Análise futura
* Confirmar achados em bases de dados maiores (maior nível de confiança) por limitações da base de dados
* Houve indicação de maior taxa de exercício físico em pessoas acometidas com diabetes na faixa de 18 a 42 anos e menor taxa de exercício naquelas com doenças cardíacas, mas a amostra dessas populações no dataset Health Lifestyle é pequena para ser conclusiva
