## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Selecionado o Dataset com preços, feito o download e apos isso realizado o upload do dataset no sagemaker canvas,
    para posteriormente realizar a construção do modelo.
    ![image](https://github.com/user-attachments/assets/d108deb2-6b50-44ca-be52-306c01f9db79)


### 2. Construir/Treinar

-   No SageMaker Canvas, utilzando o dataset importado, comecei a construir o modelo.
-   Ele ja me a opção de  predição no caso é time series ou series temporais, isso pelo atributo de data existente no dataset.
-   Algumas configurações para melhorar o desempenho do modelo, excluir a coluna de flag promocional, no caso pode atrapalhar a prediçao, eu ja havia testado outros modelos, por isso decidi neste tirar para avaliar, alem de lidar com valores que estavam faltando
-   Feito isso, começar a treinar o modelo com a opção de Quick Build
    ![image](https://github.com/user-attachments/assets/cd784f05-146a-4f96-8946-e6ab0abed720)


### 3. Analisar

-   Após o treinamento, examine as métricas de performance do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   Use o modelo treinado para fazer previsões de estoque.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

## 🤔 Dúvidas?

Esperamos que esta experiência tenha sido enriquecedora e que você tenha aprendido mais sobre Machine Learning aplicado a problemas reais. Se tiver alguma dúvida, não hesite em abrir uma issue neste repositório ou entrar em contato com a equipe da DIO.
