# Documentação de limpeza de dados
## [Fitbit dataset](https://www.kaggle.com/datasets/arashnic/fitbit)
* não houve necessidade de lidar com dados faltantes ou discrepantes
* no dataset weightlog - criação de coluna tornando o IMC numérico em categórico. 
    * coluna de IMC numérico não foi sobrescrita para manter a referência e completude dos dados. 
    * os níveis 1 2 e 3 de obesidade foram incluídos apenas como obesidade, já que essa granularidade não seria necessária para a análise
* criação de segundo dataframe de weightlog incluindo ids sem informação de IMC para contagem correta de distribuição de IMC/ falta de informação

## [Healthlifestyle dataset](https://www.kaggle.com/datasets/mahdimashayekhi/health-and-lifestyle-dataset)

* não houve necessidade de lidar com dados faltantes ou discrepantes. 
    * De fato o dataset é bastante homogêneo, o que levantou a preocupação seos dados poderiam ser levados em conta para qualquer análise.
* criação de coluna tornando o IMC numérico em categórico. 
    * Coluna de IMC numérico não foi sobrescrita para manter a referência e completude dos dados. 
    * Os níveis 1 2 e 3 de obesidade foram incluídos apenas como obesidade, já que essa granularidade não seria necessária para a análise
* criação de faixas etárias também em coluna nova
* reordenação das colunas para que IMC e faixa etária ficassem consequentes às originais

## [Obesity dataset](https://www.kaggle.com/datasets/suleymansulak/obesity-dataset)
* o primeiro dataset de hábitos de pessoas de diferentes IMCs estava bastante instável e precisou ser substituído [Link dataset obesity worlds](https://www.kaggle.com/datasets/willianoliveiragibin/obesity-worlds)
* nesse dataset, foi necessário mudar valores numéricos para categóricos seguindo o dicionário do dataset para a maioria das colunas (Overweight_Obese_Family, Consumption_of_Fast_Food, Frequency_of_Consuming_Vegetables, Number_of_Main_Meals_Daily, Food_Intake_Between_Meals, Smoking, Liquid_Intake_Daily, Calculation_of_Calorie_Intake, Physical_Excercise, Schedule_Dedicated_to_Technology, Type_of_Transportation_Used, Class)
* algumas colunas também foram renomeadas por motivo de clareza ('Sex':'Gender' , 'Height':'Height (cm)', 'Overweight_Obese_Family':'Overweight_Family' , 'Physical_Excercise':'Weekly_Physical_Activity' , Class : BMI_Category)
* a coluna de 'BMI_Category' foi substituída e também deu origem a outra com apenas duas categorias mais genéricas, que englobam obesos e overweight na mesma categoria, assim como underweight e normal weight na mesma categoria. 
    * Isso foi feito para que a coluna mais apropriada para cada situação pudesse ser usada