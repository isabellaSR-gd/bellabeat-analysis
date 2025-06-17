# Documentação de limpeza de dados
## [Fitbit dataset](https://www.kaggle.com/datasets/arashnic/fitbit)
* Não houve necessidade de lidar com dados faltantes ou discrepantes
* No dataset weightlog - criação de coluna tornando o IMC numérico em categórico. 
    * Coluna de IMC numérico não foi sobrescrita para manter a referência e completude dos dados. 
    * Os níveis 1 2 e 3 de obesidade foram incluídos apenas como obesidade, já que essa granularidade não seria necessária para a análise
* Criação de segundo dataframe de weightlog incluindo ids sem informação de IMC para contagem correta de distribuição de IMC/ falta de informação

## [Obesity dataset](https://www.kaggle.com/datasets/suleymansulak/obesity-dataset)
* Nesse dataset, foi necessário mudar valores numéricos para categóricos seguindo o dicionário do dataset para a maioria das colunas (Overweight_Obese_Family, Consumption_of_Fast_Food, Frequency_of_Consuming_Vegetables, Number_of_Main_Meals_Daily, Food_Intake_Between_Meals, Smoking, Liquid_Intake_Daily, Calculation_of_Calorie_Intake, Physical_Excercise, Schedule_Dedicated_to_Technology, Type_of_Transportation_Used, Class).
* Algumas colunas também foram renomeadas por motivo de clareza ('Sex':'Gender' , 'Height':'Height (cm)', 'Overweight_Obese_Family':'Overweight_Family' , 'Physical_Excercise':'Weekly_Physical_Activity' , Class : BMI_Category).
* A coluna de 'BMI_Category' foi substituída e também deu origem a outra com apenas duas categorias mais genéricas, que englobam obesos e overweight na mesma categoria, assim como underweight e normal weight na mesma categoria. 
    * Isso foi feito para que a coluna mais apropriada para cada situação pudesse ser usada.


# Datasets testados mas não usados
## [Healthlifestyle dataset](https://www.kaggle.com/datasets/mahdimashayekhi/health-and-lifestyle-dataset)
* Objetivo de usar o dataset acima era avaliar prática de exercício por idade para sugerir uma idade ideal para o público do Bellabeat.
* Porém os dados eram muito homogêneos entre diferentes categorias, apenas insights e correlações muito fracas podiam ser obtidas. 
* Decisão foi rejeitar os dados e em um futuro podemos avaliar o uso de outro dado.

## [Obesity worlds](https://www.kaggle.com/datasets/willianoliveiragibin/obesity-worlds)
* Primeiro dataset usado para análises de exercício por categoria de IMC
* Foi descartado por conter muitos valores de idade incorretos, muitas idades abaixo de 18 e acima de 100. Apesar de idades abaixo de 18 não serem necessariamente um dado sujo, essa população não traria insights para a análise.