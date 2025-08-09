 <img width="1080" height="379" alt="image" src="https://github.com/user-attachments/assets/5651cf91-42cf-4a3e-8606-5ce0830c02bc" />

 
 # TURNOVER PREDICTION

🎓 Projeto Final da Trilha de Ciência de Dados do Bootcamp RESTART, 2025: Predição de Turnover (Rotatividade) de Funcionários com Machine Learning.  
___
# DOCUMENTAÇÃO

### METODOLOGIA
Este projeto segue a metodologia CRISP-DM (Cross-Industry Standard Process for Data Mining) com as seguintes etapas: 
1. Entendimento do Negócio: objetivo do projeto alinhado às dores e perguntas de negócio, determinar objetivo do projeto, elaborar plano do projeto. 
2. Entendimento dos Dados: carregar dados, descrever dados, explorar dados, verificar qualidade dos dados. 
3. Preparo dos dados: selecionar dados, limpar, feature engineering, formatar dados.
4. Modelagem: selecionar modelo, treinar, designing tests, ajustar modelo e avaliar modelo. 
5. Avaliação dos modelos 
6. Deployment: planejar deployment (próximos passos).

### FERRAMENTAS
![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252) ![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)

[![Pandas](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)

[![Numpy](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
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
* **Education:** Nível educacional (1-5, onde 1="Below College", 5="Doctor").  
* **EducationField:** Área de formação (ex: "Life Sciences", "Medical", "Technical Degree").  
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

** 📚 Referência Dados**
**Title:** “IBM HR Analytics Attrition & Performance
**Source:** [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/data)
**Author:** pavansubhash
**License:** Database Contents License (DbCL) v1.0

** 📚 Referência Dados**
