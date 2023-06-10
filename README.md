Eixo 5 - Projeto Arquitetura de Dados em Nuvem 
 
 
Grupo 1 - Integrantes: Tayrini Martins, Daniella Borba e Lindomar Fontes. 


RESUMO  

A governança de dados é uma abordagem baseada em princípios para gerenciar dados durante o ciclo de vida, desde a aquisição até o uso e o descarte. É tudo o que você faz para garantir que os dados sejam seguros, privados, precisos, disponíveis e utilizáveis. Isso inclui as ações que as pessoas devem realizar, os processos que devem seguir e a tecnologia que oferece suporte durante todo o ciclo de vida dos dados. 

Governança de dados significa definir padrões internos (políticas de dados) que se aplicam a forma como os dados são coletados, armazenados, processados e descartados. Ela controla quem pode acessar quais tipos de dados e quais tipos de dados estão sob governança. A governança de dados também envolve a conformidade com padrões externos definidos por associações do setor, agências governamentais e outras partes interessadas. 

 
DIAGNÓSTICO DA SITUAÇÃO-PROBLEMA 

Realizado anualmente pelo Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (Inep), o Censo da Educação Superior constitui-se como importante instrumento de obtenção de dados para a geração de informações que subsidiam a formulação, o monitoramento e a avaliação das políticas públicas, além de ser elemento importante para a elaboração de estudos e pesquisas sobre o setor.  

O Censo coleta informações sobre as Instituições de Educação Superior (IES), sobre os cursos de graduação e sequenciais de formação específica e sobre os discentes e docentes vinculados a esses cursos. 

Com objetivo de avaliar os dados dos últimos 5 anos publicados, fomos contratos por uma Instituição não Governamental com objetivo de apresentar, sinteticamente, os principais resultados extraídos do Censo da Educação Superior 2017-2021.  

 
JUSTIFICATIVA 

Compreender o perfil dos ingressantes no ensino superior é essencial para avaliar a efetividade e impactos das políticas públicas de acesso, tendências que podem estar em acordo ou desacordo com o momento econômico e necessidades do mercado brasileiro.  

A relevância deste projeto justifica-se sobretudo na ausência de trabalho ou ferramenta semelhante, isto é, uma ferramenta de BI que tenha como base os dados do Censo do Ensino Superior que evidenciam o perfil dos ingressantes no Ensino Superior, no Brasil. 

Essa ferramenta, que no presente trabalho será feita utilizando o Software POWERBI, se  faz relevante, pois ao permitir uma visualização dos dados e métricas relacionados aos ingressantes no Ensino Superior no Brasil, além de atender ao interesse público de divulgação de informações deste gênero, auxilia na compreensão de tendências profissionais e avaliação da compatibilidade desta realidade com necessidades do mercado de trabalho.  

Essa compreensão é essencial, pois além de possuir grande valor teórico e prático no estabelecimento de ações de extensão em suas diversas modalidades e políticas públicas, pode ser de grande relevância para auxiliar que decisões em relação a ações futuras no contexto da educação superior sejam tomadas com maior assertividade, já que as mesmas poderão ter como base os resultados das ações implementadas no passado, que serão evidenciados pelos dados. 


OBJETIVO GERAL 

Este trabalho visa avaliar o perfil dos ingressantes no ensino superior no Brasil, no período de 2017 a 2021, a fim de realizar uma análise comparativa. 


OBJETIVOS ESPECÍFICOS 

As metas têm como objetivo quantificar os objetivos específicos a serem alcançados com a execução do projeto, uma vez que as metas estão sendo compreendidas como a expressão dos objetivos em termos quantitativos, mensuráveis e verificáveis. 

Principais Metas: 

INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR, POR ORGANIZAÇÃO ACADÊMICA E CATEGORIA ADMINISTRATIVA 

PERCENTUAL DO NÚMERO DE INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR, POR CATEGORIA ADMINISTRATIVA

NÚMERO DE INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR E MATRÍCULAS DE GRADUAÇÃO, SEGUNDO A ORGANIZAÇÃO ACADÊMICA 

DISTRIBUIÇÃO DAS IES E MATRÍCULAS DE GRADUAÇÃO POR ORGANIZAÇÃO ACADÊMICA – BRASIL 

PERFIL DO DOCENTE DE INSTITUIÇÃO DE EDUCAÇÃO SUPERIOR, POR CATEGORIA ADMINISTRATIVA (PÚBLICA E PRIVADA) 

PERFIL DO VÍNCULO DISCENTE DE GRADUAÇÃO, POR MODALIDADE DE ENSINO (PRESENCIAL E A DISTÂNCIA) 

NÚMERO DE VAGAS DE CURSOS DE GRADUAÇÃO, POR TIPO DE VAGA E CATEGORIA ADMINISTRATIVA 

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR MODALIDADE DE ENSINO  

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR CATEGORIA ADMINISTRATIVA 

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR SEXO E COR


ETAPA DE ETL

Para etapa de ETL, utilizamos o data factory, ferramenta disponibilizada pela Azure para integração e construção de processos de ETL sem a necessidade de criar codigos. Durante o pipeline de ETL, os dados de destino sao armazenados e transformados. Com isso, foi possivel, além de agregar os dados nos anos referentes à base, tratar as datas e os quantitativos, transformando as colunas do tipo string para  int ou float, com o objetivo de possibilitar o manuseio e posteriores cálculos que fossem necessários. Cabe ainda ressaltar que, para tanto, foi necessario também criar um blob storage para armazenar os arquivos que passsariam pelo processo de transformação.

MODELO DE PREVISÃO

Para essa etapa, utilizamos o modelo de previsão de série temporal disponível no Excel. A previsão de série temporal é uma técnica utilizada para analisar tendências, ciclos e padrões em dados ao longo do tempo para prever o futuro. Isso é muito útil para uma variedade de campos, incluindo finanças, economia, meteorologia, planejamento de demanda e muito mais. No contexto do Excel, a previsão de série temporal pode ser realizada usando várias funções e ferramentas incorporadas. Em versões mais recentes do Excel (2016 em diante), há uma funcionalidade chamada "Previsão.ETS" que facilita a realização de previsões de séries temporais.
Aqui está uma explicação mais detalhada de como ela funciona:

**Funcionalidade Previsão.ETS**: Esta é uma família de funções que permite prever valores futuros com base em dados históricos. ETS significa "Erro, Tendência, Sazonalidade", que são os três componentes de uma série temporal.
**Previsão.ETS.ESTAT()**: Esta função retorna estatísticas sobre a qualidade do ajuste da previsão ao histórico de dados.

Vale ressaltar que a previsão de séries temporais é uma técnica estatística avançada, e sua eficácia pode ser limitada por vários fatores, incluindo a qualidade dos dados históricos, a presença de tendências ou padrões não lineares e eventos imprevistos que podem afetar a série temporal.

-----------------------------------------------------------------------------  ETAPA 5 ----------------------------------------------------------------------

ANÁLISE DOS RESULTADOS

A acurácia e a eficácia são métricas utilizadas para avaliar a qualidade de previsões em modelos estatísticos e de aprendizado de máquina. No contexto da previsão de dados no Excel, a acurácia refere-se à proximidade entre os valores previstos e os valores reais. A eficácia, por outro lado, mede a capacidade do modelo de fazer previsões consistentes e confiáveis ao longo do tempo.

No arquivo preivisao_alunos.xlsx, temos os valores previstos para o número de alunos em cada ano até 2025. Essas previsões foram geradas pela aplicação de previsão do Excel, usando os dados históricos de anos anteriores. As métricas fornecidas (Alpha, Beta, Gamma, MASE, SMAPE, MAE e RMSE) são comumente usadas para avaliar a acurácia e a eficácia das previsões.

Alpha e Beta: Esses valores indicam a precisão e a tendência das previsões em relação aos dados reais. No caso em questão, ambos são zero, o que sugere que as previsões estão próximas dos valores reais e não apresentam tendências significativas.

Gamma: O valor de 0,13 indica uma sazonalidade nas previsões, ou seja, há uma variação previsível no número de alunos ao longo do tempo.

MASE (Mean Absolute Scaled Error): Essa métrica avalia a acurácia das previsões, normalizando o erro absoluto médio em relação à variabilidade dos dados. Um valor de 0,21 indica que as previsões têm um erro médio absoluto relativamente baixo em comparação com a variabilidade dos dados.

SMAPE (Symmetric Mean Absolute Percentage Error): Essa métrica mede a acurácia percentual das previsões, considerando a simetria entre valores previstos e reais. Um valor de 0 indica que as previsões estão perfeitamente alinhadas com os valores reais.

MAE (Mean Absolute Error) e RMSE (Root Mean Square Error): Essas métricas avaliam o erro médio absoluto e o erro quadrático médio das previsões, respectivamente. Valores de MAE e RMSE maiores indicam uma maior dispersão entre as previsões e os valores reais.

Com base nas métricas fornecidas, as previsões obtidas parecem ser razoavelmente precisas, com baixos erros médios absolutos e uma boa aderência aos valores reais. No entanto, é importante ressaltar que a precisão e a eficácia das previsões dependem do contexto específico e dos dados disponíveis. Portanto, é sempre recomendável realizar uma análise mais aprofundada e considerar outros fatores relevantes.

A matriz de confusão é uma ferramenta comumente utilizada para avaliar a qualidade de previsões em problemas de classificação, onde se categorizam dados em classes distintas. No caso apresentado, como estamos lidando com previsões de valores numéricos contínuos, a matriz de confusão não é diretamente aplicável.

Para melhorar os resultados e torná-los mais fidedignos, algumas sugestões podem ser consideradas:

Utilizar mais dados históricos: Se possível, coletar e incorporar mais anos de dados históricos para treinar o modelo de previsão. Quanto mais dados disponíveis, maior a probabilidade de obter previsões mais precisas.

Considerar fatores externos: Analisar se existem fatores externos que influenciam o número de alunos, como políticas governamentais, mudanças demográficas, tendências socioeconômicas, entre outros. Incorporar esses fatores no modelo pode melhorar a precisão das previsões.

Avaliar diferentes modelos: Experimentar diferentes técnicas de previsão disponíveis no Excel ou em outras ferramentas para identificar o modelo mais adequado ao conjunto de dados e ao objetivo específico da previsão.

Realizar validação cruzada: Dividir os dados disponíveis em conjuntos de treinamento e teste e realizar validação cruzada para avaliar a performance do modelo em diferentes cenários. Isso ajuda a identificar possíveis problemas de overfitting e a obter uma estimativa mais confiável da acurácia das previsões.

Monitorar e ajustar o modelo: À medida que novos dados se tornam disponíveis, é importante monitorar regularmente as previsões e ajustar o modelo conforme necessário. Isso permite adaptar o modelo às mudanças e garantir que as previsões permaneçam precisas ao longo do tempo.

É importante considerar o possível impacto da pandemia nos dados fornecidos de previsão de alunos. A pandemia da COVID-19 teve um efeito significativo no setor educacional em todo o mundo, levando ao fechamento temporário de escolas, adoção de ensino remoto e mudanças nas dinâmicas de matrícula dos alunos.

No contexto das previsões de alunos, a pandemia pode ter causado interrupções e alterações no número de matrículas, o que pode afetar a precisão das previsões feitas com base nos dados históricos anteriores à pandemia. Todavia, considerando o recorte de dados utilizados, não foi possível identificar se a diminuição do número de alunos em 2021 foi reflexo da pandemia. Caso fosse identificado que o número de alunos foi impactado por esse período, esses dados deveriam ser trabalhados de uma forma diferente (outliers).

Em resumo, as métricas fornecidas e as previsões obtidas sugerem que o modelo utilizado no Excel para prever o número de alunos apresenta resultados promissores. No entanto, é sempre importante analisar as métricas em conjunto com outros fatores e buscar maneiras de melhorar a precisão e a eficácia das previsões, levando em consideração as especificidades do problema em questão.
