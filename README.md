 <img width="1080" height="379" alt="image" src="https://github.com/user-attachments/assets/5651cf91-42cf-4a3e-8606-5ce0830c02bc" />

 
 # TURNOVER PREDICTION

🎓 Projeto Final da Trilha de Ciência de Dados do Bootcamp RESTART, 2025: Predição de Turnover (Rotatividade) de Funcionários com Machine Learning.  
___
# DOCUMENTAÇÃO

### METODOLOGIA
Este projeto se baseia com adaptações na metodologia CRISP-DM (Cross-Industry Standard Process for Data Mining) com as seguintes etapas: 

1. Entendimento do Negócio: objetivo do projeto alinhado às dores e perguntas de negócio, determinar objetivo do projeto, elaborar plano do projeto. 
2. Entendimento dos Dados: carregar dados, descrever dados, explorar dados, verificar qualidade dos dados. 
3. Preparo dos dados: pré-seleção de features.
4. Modelagem: selecionar modelo, treinar, ajustar modelo e avaliar modelo. 
5. Avaliação do modelos: importância das features, validação cruzada.
6. Conclusão


### FERRAMENTAS
![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252) ![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)

___

### 1. Entendimento do Negócio

**| 🎯 Perguntas Norteadoras**
* Quais características mais influenciam na rotatividade de funcionários?
* Qual perfil de colaborador tem maior propensão a sair da empresa?
* Um modelo de machine learning pode prever com boa precisão a saída de um
funcionário?
* Que ações a empresa pode tomar com base nessas previsões?
___
### 2. Entendimento dos Dados 

**| 🗂️ Glossário Variáveis**

* **Age:** Idade do funcionário (em anos).  
* **Attrition:** Indica se o funcionário deixou a empresa (Yes/No).  
* **BusinessTravel:** Frequência de viagens a trabalho (ex: "Travel_Rarely", "Travel_Frequently", "Non-Travel").  
* **DailyRate:** Diária, valor de um dia de trabalho(valor numérico).  
* **Department:** Departamento do funcionário (ex: "Sales", "Research & Development", "Human Resources").  
* **DistanceFromHome:** Distância entre casa e trabalho (em km).  
* **Education:** Nível educacional (1-5, onde 1="Below College", 5="Doctor").  * **EducationField:** Área de formação (ex: "Life Sciences", "Medical", "Technical Degree").  
* **EmployeeCount:** Contagem de funcionários (normalmente 1 para registros individuais).  
* **EmployeeNumber:** ID único do funcionário.  
* **EnvironmentSatisfaction:** Satisfação com o ambiente de trabalho (escala numérica, normalmente 1-4).  
* **Gender:** Gênero ("Male" ou "Female").  
* **HourlyRate:** Remuneração por hora.  
* **JobInvolvement:** Engajamento no trabalho (escala numérica, ex: 1-4).  
* **JobLevel:** Nível hierárquico (1=júnior, 5=sênior).  
* **JobRole:** Cargo ocupado (ex: "Sales Executive", "Research Scientist").  
* **JobSatisfaction:** Satisfação com o trabalho (escala numérica, ex: 1-4).  
* **MaritalStatus:** Estado civil ("Single", "Married", "Divorced").  
* **MonthlyIncome:** Salário mensal bruto.  
* **MonthlyRate:** Salário mensal base.  
* **NumCompaniesWorked:** Número de empresas onde já trabalhou.  
* **Over18:** Se é maior de 18 anos (normalmente "Yes" para todos).  
* **OverTime:** Faz horas extras ("Yes" ou "No").  
* **PercentSalaryHike:** Percentual do último aumento salarial.  
* **PerformanceRating:** Avaliação de desempenho (ex: 1-5).  
* **RelationshipSatisfaction:** Satisfação com relacionamentos no trabalho (escala numérica).  
* **StandardHours:** Carga horária padrão (ex: 80 horas/mês).  
* **StockOptionLevel:** Nível de opções de ações (ex: 0-3).  
* **TotalWorkingYears:** Total de anos de experiência profissional.  
* **TrainingTimesLastYear:** Número de treinamentos no último ano.  
* **WorkLifeBalance:** Equilíbrio vida-trabalho (escala numérica).  
* **YearsAtCompany:** Tempo na empresa atual (em anos).  
* **YearsInCurrentRole:** Tempo no cargo atual (em anos).  
* **YearsSinceLastPromotion:** Tempo desde a última promoção (em anos).  
* **YearsWithCurrManager:** Tempo com o mesmo gerente (em anos).

**📚 Referência Dados**

* **Title:** “IBM HR Analytics Attrition & Performance
* **Source:** [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/data)
* **Author:** pavansubhash
* **License:** Database Contents License (DbCL) v1.0

**1. ENTENDENDO DADOS**
   
<img width="990" height="201" alt="image" src="https://github.com/user-attachments/assets/01c6e16c-7e64-46cc-bfc0-64e68d30bd70" />
<img width="1000" height="240" alt="image" src="https://github.com/user-attachments/assets/9782e3de-c247-4126-8aa4-85670cd63f7d" />

<img width="1007" height="282" alt="image" src="https://github.com/user-attachments/assets/2773b431-0fef-4453-8f64-4e5ea10ca007" />
<img width="1002" height="349" alt="image" src="https://github.com/user-attachments/assets/ede95caf-3e9d-411e-b625-99f6ba4adfbf" />
<img width="993" height="250" alt="image" src="https://github.com/user-attachments/assets/a54f717b-d4f9-42bf-8436-537aa712b16d" />

___
### 3. Preparo dos Dados
<img width="990" height="135" alt="image" src="https://github.com/user-attachments/assets/f27e53c9-2f70-45a9-a25c-b1f0c67e7aa6" />

___
### 4. Modelagem

 #### **Estratégia de avaliação**
 
 * Métricas: F1-Score e custo computacional.
 * Justificativa: Os falsos negativos (colaboradores que saem sem serem previstos pelo modelo) representam um custo significativamente maior para a organização do que os falsos positivos (ações de retenção desnecessárias). O F1-Score, que balanceia precisão e recall, é a métrica ideal para avaliar esse trade-off. Paralelamente, a eficiência computacional é crucial para arantir tempos de resposta ágeis na tomada de decisão, permitir a escalabilidade do modelo com otimização dos custos operacionais além de se alinhar com estratégias de sustentabilidade.

  #### **Modelos testados**  
* Os modelos testados foram Regressão Logística, Logistic Regression (L2 - Ridge), Logistic Regression (L1 - LASSO) e Random Forest.
* Justificativa: modelos com boa explicabilidade, requisito levantado na definição do problema de negócio.

<img width="1206" height="301" alt="image" src="https://github.com/user-attachments/assets/a6cedb02-115c-4b91-85cf-c9a99ea0aca5" />

 * Ajuste de Hiperparâmetros com GridSearchCV
<img width="555" height="212" alt="image" src="https://github.com/user-attachments/assets/4f46f82a-4877-4128-8f68-82eabe5cab0c" />

* Feature Importance e Seleção de Feature para modelagem final com Permurarion Importance e Feature Importance (Coeficientes).
   
___
### 5. Treino e Avaliação de Modelo

* Após exclusão de fetures menos importantes o modelo otimizado foi treinado, avaliado e salvo.

___
### 6. Conclusão

<img width="652" height="136" alt="image" src="https://github.com/user-attachments/assets/87f9ab90-673b-4cc8-80f5-8017353ef473" />

<img width="540" height="166" alt="image" src="https://github.com/user-attachments/assets/902f88a9-c1e6-4e24-9198-b0c70bf5813f" />

<img width="713" height="317" alt="image" src="https://github.com/user-attachments/assets/9b1404ef-633a-43c2-852d-621479e4e38c" />

<img width="706" height="248" alt="image" src="https://github.com/user-attachments/assets/88bed8b4-3227-43a5-b57e-abc2192caa0b" />
