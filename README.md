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

-   Após o treinamento, Foram destacadas as seguintes metricas
     ![image](https://github.com/user-attachments/assets/2ac6df29-7b08-4c3d-a974-f0f1a4f1dfe4)
-   MAPE de 0.149 e WAPE de 0.103 sugerem que o modelo está fazendo previsões razoavelmente precisas, com erros médios absolutos de cerca de 14.9% e 10.3%, respectivamente.
-   RMSE de 5.977 sugere que há alguns erros maiores, pois RMSE é mais sensível a outliers.
-   MASE de 0.310 indica que o modelo é significativamente mais preciso que o modelo de referência.
    No geral, as métricas indicam que o modelo tem um desempenho bom, com erros relativamente baixos e boa precisão

### 4. Prever

-  Apos a conclusao da analise e das metricas, prossegui para predição, selecionei um item aleatorio para analisar como o modelo se comporta na predicao e tirei algumas analises deste.
   ![image](https://github.com/user-attachments/assets/ffb33b9d-1f9c-4084-a41f-a841ccf3751c)


P10 indica uma previsão conservadora, sugerindo um valor abaixo do qual a demanda real é improvável de cair (apenas 10% de chance de ser menor).
P50 (mediana) fornece um ponto médio da previsão, sugerindo que a demanda real tem 50% de chance de ser menor ou maior do que esse valor.
P90 indica uma previsão otimista, sugerindo um valor acima do qual a demanda real é improvável de subir (apenas 10% de chance de ser maior).
Uso Prático das Previsões Percentis
Esses diferentes percentuais ajudam na tomada de decisão sob incerteza. Por exemplo:

Planejamento de Estoque: Você pode usar o P90 para garantir que tenha estoque suficiente para cobrir 90% das possíveis demandas, reduzindo o risco de falta de estoque.
Gestão de Custos: Usar o P10 pode ser útil para otimizar custos e evitar excessos de estoque, garantindo que não haja desperdício de recursos.

   

