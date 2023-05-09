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

INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR, POR ORGANIZAÇÃO ACADÊMICA E CATEGORIA ADMINISTRATIVA – 2021 

PERCENTUAL DO NÚMERO DE INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR, POR CATEGORIA ADMINISTRATIVA – 2021 

NÚMERO DE INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR E MATRÍCULAS DE GRADUAÇÃO, SEGUNDO A ORGANIZAÇÃO ACADÊMICA – 2021 

DISTRIBUIÇÃO DAS IES E MATRÍCULAS DE GRADUAÇÃO POR ORGANIZAÇÃO ACADÊMICA – BRASIL – 2021 

PERFIL DO DOCENTE DE INSTITUIÇÃO DE EDUCAÇÃO SUPERIOR, POR CATEGORIA ADMINISTRATIVA (PÚBLICA E PRIVADA) – 2021 

PERFIL DO VÍNCULO DISCENTE DE GRADUAÇÃO, POR MODALIDADE DE ENSINO (PRESENCIAL E A DISTÂNCIA) – 2021 

NÚMERO DE VAGAS DE CURSOS DE GRADUAÇÃO, POR TIPO DE VAGA E CATEGORIA ADMINISTRATIVA – 2021 

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR MODALIDADE DE ENSINO – 2017-2021 

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR CATEGORIA ADMINISTRATIVA – 2017-2021 

NÚMERO DE INGRESSOS EM CURSOS DE GRADUAÇÃO, POR GRAU ACADÊMICO – 2017-2021 


ETAPA DE ETL

Para etapa de ETL, utilizamos o data factory, ferramenta disponibilizada pela Azure para integração e construção de processos de ETL sem a necessidade de criar codigos. Durante o pipeline de ETL, os dados de destino sao armazenados e transformados. Com isso, foi possivel, além de agregar os dados nos anos referentes à base, tratar as datas e os quantitativos, transformando as colunas do tipo string para  int ou float, com o objetivo de possibilitar o manuseio e posteriores cálculos que fossem necessários. Cabe ainda ressaltar que, para tanto, foi necessario também criar um blob storage para armazenar os arquivos que passsariam pelo processo de transformação.
