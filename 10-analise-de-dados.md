# Análise de dados

> Planilhas, interpretação de métricas, estatística, relatórios e pesquisa de mercado com dados.

**42 prompts** nesta categoria — 2 do repositório original PromptChains (marcados com 🔁) e 40 novos.

**Como usar:** copie o bloco inteiro de um prompt, substitua os campos entre colchetes `[...]` pelas suas informações e cole no ChatGPT, Claude, Gemini ou em uma extensão de fila de prompts (como o ChatGPT Queue). Cada trecho separado por `~` é uma etapa: em uma extensão de fila, as etapas são enviadas uma a uma automaticamente; sem extensão, envie uma etapa por vez, na ordem.

[← Voltar ao índice geral](README.md)

## Índice

**[Planilhas](#planilhas)**

1. [Explicar e criar fórmulas de planilha](#1-explicar-e-criar-fórmulas-de-planilha)
2. [Planilha de controle sob medida](#2-planilha-de-controle-sob-medida)
3. [Limpeza e padronização de dados](#3-limpeza-e-padronização-de-dados)
4. [Tabela dinâmica e resumos](#4-tabela-dinâmica-e-resumos)
5. [Cruzar bases com PROCV, PROCX e ÍNDICE/CORRESP](#5-cruzar-bases-com-procv-procx-e-índicecorresp)
6. [Automação de planilhas com scripts e macros](#6-automação-de-planilhas-com-scripts-e-macros)
7. [Dashboard dentro da planilha](#7-dashboard-dentro-da-planilha)
8. [Validação e formatação condicional](#8-validação-e-formatação-condicional)
9. [Modelo de projeção em planilha](#9-modelo-de-projeção-em-planilha)

**[Interpretação de métricas](#interpretação-de-métricas)**

10. [Métricas de marketing digital](#10-métricas-de-marketing-digital)
11. [Indicadores de e-commerce](#11-indicadores-de-e-commerce)
12. [Métricas de SaaS e assinaturas](#12-métricas-de-saas-e-assinaturas)
13. [Métricas de produto e análise de coorte](#13-métricas-de-produto-e-análise-de-coorte)
14. [Pesquisa de satisfação e NPS](#14-pesquisa-de-satisfação-e-nps)
15. [Análise de teste A/B](#15-análise-de-teste-ab)
16. [Investigação de queda ou pico em uma métrica](#16-investigação-de-queda-ou-pico-em-uma-métrica)
17. [Métricas do funil comercial](#17-métricas-do-funil-comercial)

**[Análise exploratória e estatística](#análise-exploratória-e-estatística)**

18. [Análise exploratória de uma base de dados](#18-análise-exploratória-de-uma-base-de-dados)
19. [Estatística descritiva explicada](#19-estatística-descritiva-explicada)
20. [Correlação e regressão](#20-correlação-e-regressão)
21. [Segmentação de clientes (RFM)](#21-segmentação-de-clientes-rfm)
22. [Previsão de séries temporais](#22-previsão-de-séries-temporais)
23. [Análise de questionário ou pesquisa](#23-análise-de-questionário-ou-pesquisa)
24. [SQL para análise de dados](#24-sql-para-análise-de-dados)
25. [Escolha do gráfico certo](#25-escolha-do-gráfico-certo)

**[Relatórios com dados](#relatórios-com-dados)**

26. [Relatório mensal de desempenho](#26-relatório-mensal-de-desempenho)
27. [Storytelling com dados](#27-storytelling-com-dados)
28. [Explicar dados para quem não é técnico](#28-explicar-dados-para-quem-não-é-técnico)
29. [Dicionário de dados e definição de métricas](#29-dicionário-de-dados-e-definição-de-métricas)
30. [Relatório de pesquisa quantitativa](#30-relatório-de-pesquisa-quantitativa)

**[Pesquisa e inteligência de mercado](#pesquisa-e-inteligência-de-mercado)**

31. [Pesquisa de empresas de capital aberto beneficiadas pela IA](#31-pesquisa-de-empresas-de-capital-aberto-beneficiadas-pela-ia) 🔁
32. [Pesquisa de mercado extensa sobre uma empresa de capital aberto](#32-pesquisa-de-mercado-extensa-sobre-uma-empresa-de-capital-aberto) 🔁
33. [Análise de concorrência com dados públicos](#33-análise-de-concorrência-com-dados-públicos)
34. [Análise de tendências de busca](#34-análise-de-tendências-de-busca)
35. [Pesquisa e comparação de preços](#35-pesquisa-e-comparação-de-preços)
36. [Análise de avaliações e comentários de clientes](#36-análise-de-avaliações-e-comentários-de-clientes)
37. [Análise com dados públicos oficiais](#37-análise-com-dados-públicos-oficiais)

**[Projetos de dados](#projetos-de-dados)**

38. [Análise de churn (cancelamento)](#38-análise-de-churn-cancelamento)
39. [Dimensionamento de mercado (TAM, SAM e SOM)](#39-dimensionamento-de-mercado-tam-sam-e-som)
40. [Análise de cesta de compras](#40-análise-de-cesta-de-compras)
41. [Projeto de dados de ponta a ponta](#41-projeto-de-dados-de-ponta-a-ponta)
42. [Auditoria de qualidade de dados](#42-auditoria-de-qualidade-de-dados)

---


## Planilhas

### 1. Explicar e criar fórmulas de planilha

**Objetivo:** resolver um cálculo no Excel ou Google Sheets e entender a fórmula.

```
NECESSIDADE=[o que precisa ser calculado], ESTRUTURA=[colunas, abas e exemplos de dados], FERRAMENTA=[Excel ou Google Sheets, versão], IDIOMA_DA_FERRAMENTA=[português ou inglês]
Reescreva NECESSIDADE como uma regra lógica passo a passo.~
Proponha a fórmula mais simples que resolve, com os nomes de função em IDIOMA_DA_FERRAMENTA.~
Explique cada parte da fórmula.~
Mostre o resultado esperado em 3 linhas de exemplo de ESTRUTURA.~
Ofereça uma alternativa (ex.: com funções mais novas ou mais compatíveis).~
Aponte erros comuns (#N/D, #VALOR!, referências relativas) e como tratá-los.~
Sugira como deixar a planilha à prova de erros (validação, tabelas nomeadas).
```

### 2. Planilha de controle sob medida

**Objetivo:** criar uma planilha organizada para controlar qualquer processo.

```
O_QUE_CONTROLAR=[ex.: estoque, pedidos, clientes, tarefas, estudos, gastos], INFORMACOES=[dados que precisam ser registrados], USUARIOS=[quem vai preencher], RELATORIOS=[o que você quer saber a partir dos dados]
Defina as abas necessárias (cadastro, lançamentos, listas auxiliares, resumo).~
Defina as colunas de cada aba com tipo de dado e regra de preenchimento.~
Crie as listas suspensas e as validações para evitar erros de USUARIOS.~
Escreva as fórmulas da aba de resumo para responder a RELATORIOS.~
Sugira formatação condicional para alertas (atrasos, estoque baixo, metas).~
Escreva as instruções de uso na primeira aba.~
Entregue a estrutura em formato de tabela pronta para montar.
```

### 3. Limpeza e padronização de dados

**Objetivo:** transformar uma base bagunçada em dados confiáveis para análise.

```
AMOSTRA=[exemplo das primeiras linhas dos dados], PROBLEMAS_CONHECIDOS=[duplicados, formatos diferentes, campos vazios], FERRAMENTA=[Excel, Sheets, Python, Power Query]
Analise AMOSTRA e liste todos os problemas de qualidade encontrados.~
Defina o padrão desejado para cada coluna (datas, textos, números, categorias).~
Crie o passo a passo de limpeza em FERRAMENTA, em ordem.~
Escreva as fórmulas, consultas ou o código de cada passo.~
Defina regras para valores ausentes e outliers.~
Crie verificações finais de qualidade (contagens, totais, duplicados).~
Documente as transformações para repetir no futuro.
```

### 4. Tabela dinâmica e resumos

**Objetivo:** resumir uma base grande em poucos cliques para responder perguntas.

```
DADOS=[colunas disponíveis e exemplo], PERGUNTAS=[o que quer descobrir], FERRAMENTA=[Excel ou Google Sheets]
Para cada item de PERGUNTAS, defina linhas, colunas, valores e filtros da tabela dinâmica.~
Explique o passo a passo de criação em FERRAMENTA.~
Sugira campos calculados úteis (percentual do total, variação, média por item).~
Sugira o gráfico dinâmico mais adequado para cada tabela.~
Interprete um exemplo de resultado.~
Liste cuidados para manter a tabela atualizada quando os dados mudarem.
```

### 5. Cruzar bases com PROCV, PROCX e ÍNDICE/CORRESP

**Objetivo:** juntar informações de tabelas diferentes sem erro.

```
TABELA_A=[colunas e exemplo], TABELA_B=[colunas e exemplo], CHAVE=[campo em comum], OBJETIVO=[o que quer trazer de uma tabela para outra]
Verifique se CHAVE é única e padronizada nas duas tabelas e como corrigir se não for.~
Escreva a solução com PROCV e explique suas limitações.~
Escreva a solução com PROCX ou ÍNDICE/CORRESP.~
Mostre como tratar chaves não encontradas.~
Mostre como buscar com mais de um critério.~
Sugira a alternativa com Power Query ou consulta SQL para bases grandes.
```

### 6. Automação de planilhas com scripts e macros

**Objetivo:** eliminar tarefas repetitivas em planilhas.

```
TAREFA_REPETITIVA=[o que você faz manualmente], FERRAMENTA=[Google Sheets com Apps Script ou Excel com VBA ou Office Scripts], GATILHO=[quando deve rodar: botão, horário, edição, formulário]
Descreva TAREFA_REPETITIVA como algoritmo.~
Escreva o script completo e comentado em FERRAMENTA.~
Configure GATILHO e explique o passo a passo.~
Adicione tratamento de erros e registro de execução.~
Explique como testar com segurança em uma cópia.~
Liste permissões e limitações da ferramenta.
```

### 7. Dashboard dentro da planilha

**Objetivo:** criar um painel visual de indicadores sem sair do Excel ou do Sheets.

```
DADOS=[base disponível], INDICADORES=[números que quer acompanhar], PUBLICO=[quem vai ver], FERRAMENTA=[Excel ou Sheets]
Defina a pergunta que cada item de INDICADORES responde.~
Monte a aba de cálculos separada da aba visual.~
Escreva as fórmulas de cada indicador.~
Escolha o gráfico ideal para cada indicador.~
Adicione filtros de período e categoria (segmentações ou listas suspensas).~
Descreva o layout do painel para PUBLICO.~
Crie um checklist de atualização.
```

### 8. Validação e formatação condicional

**Objetivo:** fazer a planilha avisar erros e destacar o que importa automaticamente.

```
PLANILHA=[descrição das colunas], REGRAS_DE_NEGOCIO=[o que é válido e o que é alerta], USUARIOS=[quem preenche]
Defina validações de dados para cada coluna (listas, intervalos, datas, textos).~
Escreva mensagens de ajuda e de erro amigáveis.~
Crie regras de formatação condicional com fórmulas para REGRAS_DE_NEGOCIO.~
Defina a paleta de cores dos alertas (sem exagero).~
Proteja células com fórmulas para USUARIOS não apagarem.~
Explique como aplicar tudo passo a passo.
```

### 9. Modelo de projeção em planilha

**Objetivo:** montar uma projeção com premissas editáveis e cenários.

```
O_QUE_PROJETAR=[vendas, receita, custos, crescimento de usuários], PREMISSAS=[taxas, preços, volumes], HORIZONTE=[meses ou anos], CENARIOS=[pessimista, base, otimista]
Separe a planilha em premissas, cálculos e resultados.~
Liste as premissas com valores para cada um dos CENARIOS.~
Escreva as fórmulas da projeção mês a mês para HORIZONTE.~
Crie o seletor de cenário.~
Crie a tabela de sensibilidade das 2 premissas mais importantes.~
Crie o gráfico de comparação dos cenários.~
Documente as premissas e suas fontes.
```

## Interpretação de métricas

### 10. Métricas de marketing digital

**Objetivo:** entender o que os números das campanhas dizem e o que fazer com eles.

```
METRICAS=[impressões, alcance, CTR, CPC, CPM, conversões, CPA, ROAS, receita], PERIODO=[período], META=[objetivo da campanha], HISTORICO=[períodos anteriores, se houver]
Explique cada métrica de METRICAS em linguagem simples e como ela é calculada.~
Calcule as métricas derivadas que faltarem.~
Compare com HISTORICO e com referências de mercado.~
Identifique o elo mais fraco do funil (atração, clique, conversão, valor).~
Explique o que está indo bem e o que está indo mal em relação a META.~
Recomende 5 ações em ordem de prioridade.
```

### 11. Indicadores de e-commerce

**Objetivo:** diagnosticar a saúde de uma loja virtual pelos números.

```
DADOS=[visitas, taxa de conversão, ticket médio, pedidos, receita, abandono de carrinho, recompra, devoluções, CAC], PERIODO=[período], SEGMENTO=[segmento da loja]
Monte a árvore de receita: visitas × conversão × ticket médio.~
Calcule cada indicador e compare com referências de SEGMENTO.~
Identifique qual alavanca tem mais potencial de melhora.~
Simule o impacto de melhorar 10% em cada alavanca.~
Analise os indicadores de retenção e de lucratividade.~
Monte o plano de ação priorizado.
```

### 12. Métricas de SaaS e assinaturas

**Objetivo:** entender MRR, churn, LTV e outros números de negócios recorrentes.

```
DADOS=[MRR inicial, novos, expansão, contração, cancelamentos, clientes, CAC, margem], PERIODO=[meses]
Calcule a movimentação de MRR (novo, expansão, contração, cancelamento) e o MRR final.~
Calcule churn de clientes, churn de receita e retenção líquida de receita.~
Calcule ARPA, LTV, CAC e a relação LTV/CAC.~
Calcule o payback do CAC.~
Interprete cada número com referências do mercado.~
Aponte o maior risco e a maior oportunidade.
```

### 13. Métricas de produto e análise de coorte

**Objetivo:** entender se os usuários continuam usando o produto ao longo do tempo.

```
DADOS=[cadastros por período e atividade posterior], EVENTO_ATIVO=[o que conta como usuário ativo], PRODUTO=[descrição]
Explique o que é análise de coorte e por que ela é melhor que médias gerais.~
Monte a tabela de coortes de retenção a partir de DADOS.~
Calcule DAU, MAU e a razão DAU/MAU.~
Identifique o ponto de queda mais forte na retenção.~
Levante hipóteses do momento "aha" de PRODUTO que retém usuários.~
Proponha experimentos para melhorar a retenção.
```

### 14. Pesquisa de satisfação e NPS

**Objetivo:** analisar respostas de clientes e transformar em melhorias.

```
RESPOSTAS=[notas e comentários], PERGUNTAS=[perguntas da pesquisa], SEGMENTOS=[tipos de cliente, se houver]
Calcule o NPS (promotores menos detratores) geral e por SEGMENTOS.~
Classifique os comentários por tema e sentimento.~
Identifique os principais motivos de detração e de promoção.~
Cruze temas com notas para ver o que mais pesa.~
Selecione comentários representativos de cada tema.~
Proponha ações para os 3 principais problemas e um plano de retorno aos clientes.
```

### 15. Análise de teste A/B

**Objetivo:** saber se a diferença entre duas versões é real ou sorte.

```
VERSAO_A=[visitantes e conversões], VERSAO_B=[visitantes e conversões], METRICA=[métrica principal], DURACAO=[dias de teste]
Calcule a taxa de conversão de cada versão e a diferença relativa.~
Calcule a significância estatística e o intervalo de confiança.~
Explique o resultado em linguagem simples.~
Verifique se o tamanho de amostra e DURACAO foram suficientes.~
Aponte riscos de interpretação (testes parados cedo, sazonalidade, múltiplas métricas).~
Recomende: implementar, continuar testando ou descartar.
```

### 16. Investigação de queda ou pico em uma métrica

**Objetivo:** descobrir por que um número mudou de repente.

```
METRICA=[métrica afetada], MUDANCA=[quanto e quando mudou], DADOS_DISPONIVEIS=[segmentações possíveis: canal, dispositivo, região, produto], EVENTOS=[lançamentos, campanhas, mudanças técnicas no período]
Confirme se a mudança é real ou um problema de medição.~
Liste hipóteses internas e externas.~
Defina a ordem de segmentação de DADOS_DISPONIVEIS para isolar a origem.~
Cruze a mudança com EVENTOS.~
Escreva as consultas ou filtros necessários para testar cada hipótese.~
Escreva o relatório da causa provável e das ações.
```

### 17. Métricas do funil comercial

**Objetivo:** entender a eficiência do time de vendas etapa por etapa.

```
FUNIL=[número de leads, oportunidades, propostas e vendas por etapa], CICLO=[tempo médio por etapa], TICKET=[valor médio], VENDEDORES=[dados por vendedor, se houver]
Calcule as taxas de conversão entre cada etapa.~
Calcule a velocidade de vendas.~
Identifique o maior gargalo do funil.~
Compare o desempenho entre VENDEDORES.~
Calcule quantos leads são necessários para bater a meta.~
Proponha ações por etapa.
```

## Análise exploratória e estatística

### 18. Análise exploratória de uma base de dados

**Objetivo:** conhecer uma base nova e encontrar os primeiros insights.

```
DESCRICAO_DA_BASE=[colunas, tipos, número de linhas e amostra], OBJETIVO=[pergunta de negócio], FERRAMENTA=[Python com pandas, R, Excel]
Descreva cada coluna e levante dúvidas sobre o significado dos dados.~
Escreva o código ou os passos para verificar ausentes, duplicados, tipos e outliers.~
Calcule estatísticas descritivas das variáveis principais.~
Proponha os gráficos de distribuição e de relação entre variáveis.~
Liste 10 perguntas que os dados podem responder sobre OBJETIVO.~
Escreva o código das análises das 3 perguntas mais importantes.~
Resuma os insights e as próximas análises.
```

### 19. Estatística descritiva explicada

**Objetivo:** entender média, mediana, desvio padrão e companhia aplicados aos seus dados.

```
DADOS=[lista de valores ou resumo], CONTEXTO=[o que os dados representam]
Calcule média, mediana, moda, mínimo, máximo, amplitude, quartis, desvio padrão e coeficiente de variação.~
Explique o que cada medida diz sobre CONTEXTO.~
Indique se a média é representativa ou se a mediana é melhor.~
Identifique valores atípicos pelo método do intervalo interquartil.~
Descreva o formato da distribuição.~
Escreva uma conclusão de 3 frases para alguém sem conhecimento estatístico.
```

### 20. Correlação e regressão

**Objetivo:** medir a relação entre variáveis e estimar efeitos.

```
VARIAVEL_ALVO=[o que se quer explicar], VARIAVEIS_EXPLICATIVAS=[possíveis causas], DADOS=[descrição ou amostra], FERRAMENTA=[Excel, Python, R]
Calcule e interprete as correlações entre as variáveis.~
Explique a diferença entre correlação e causalidade com um exemplo de CONTEXTO.~
Ajuste uma regressão linear e escreva o código ou os passos em FERRAMENTA.~
Interprete os coeficientes, o R² e os valores-p em linguagem simples.~
Verifique os pressupostos do modelo.~
Use o modelo para uma previsão de exemplo e informe as limitações.
```

### 21. Segmentação de clientes (RFM)

**Objetivo:** dividir clientes em grupos para ações de marketing diferentes.

```
DADOS=[cliente, data e valor das compras], NEGOCIO=[tipo de negócio], FERRAMENTA=[Excel, Python, SQL]
Calcule recência, frequência e valor monetário de cada cliente.~
Atribua notas de 1 a 5 em cada dimensão por quintis.~
Crie os segmentos (campeões, fiéis, em risco, hibernando, novos, perdidos) com regras claras.~
Escreva o código ou as fórmulas em FERRAMENTA.~
Descreva o perfil e o tamanho de cada segmento.~
Proponha uma ação de marketing para cada segmento.
```

### 22. Previsão de séries temporais

**Objetivo:** prever vendas, demanda ou outra métrica ao longo do tempo.

```
SERIE=[dados históricos por dia, semana ou mês], HORIZONTE=[quanto tempo prever], EVENTOS=[promoções, feriados, mudanças], FERRAMENTA=[Excel, Python, R]
Analise tendência, sazonalidade e ruído de SERIE.~
Proponha 3 métodos de previsão adequados (média móvel, suavização exponencial, modelo sazonal) e justifique.~
Escreva o código ou os passos em FERRAMENTA.~
Separe um período para validação e calcule o erro de cada método.~
Gere a previsão para HORIZONTE com intervalo de confiança.~
Explique como incorporar EVENTOS e quando refazer a previsão.
```

### 23. Análise de questionário ou pesquisa

**Objetivo:** tabular e analisar respostas de um formulário.

```
PERGUNTAS=[perguntas e tipos de resposta], RESPOSTAS=[dados ou resumo], AMOSTRA=[número e perfil dos respondentes], OBJETIVO=[o que se queria descobrir]
Avalie a representatividade de AMOSTRA e as limitações.~
Tabule as perguntas fechadas com frequências e percentuais.~
Cruze as perguntas mais relevantes por perfil.~
Categorize as respostas abertas por tema.~
Sugira os gráficos de cada resultado.~
Escreva as conclusões ligadas a OBJETIVO.
```

### 24. SQL para análise de dados

**Objetivo:** escrever consultas SQL que respondem perguntas de negócio.

```
ESQUEMA=[tabelas, colunas e relações], PERGUNTAS=[perguntas de negócio], BANCO=[PostgreSQL, MySQL, BigQuery etc.]
Para cada item de PERGUNTAS, explique a lógica antes de escrever a consulta.~
Escreva a consulta em BANCO usando CTEs para legibilidade.~
Use funções de janela quando fizer sentido (ranking, acumulado, variação).~
Explique o resultado esperado de cada consulta.~
Aponte armadilhas (duplicação em junções, nulos, fuso horário).~
Sugira índices ou otimizações para bases grandes.
```

### 25. Escolha do gráfico certo

**Objetivo:** visualizar dados de forma honesta e fácil de entender.

```
DADOS=[descrição dos dados], MENSAGEM=[o que o gráfico precisa mostrar], PUBLICO=[quem vai ver], MEIO=[slide, relatório, painel, rede social]
Classifique MENSAGEM: comparação, evolução, composição, distribuição ou relação.~
Recomende o tipo de gráfico ideal e 1 alternativa.~
Defina título-afirmação, eixos, rótulos e cores.~
Liste o que remover para reduzir poluição visual.~
Aponte práticas que distorcem a leitura (eixo cortado, 3D, pizza com muitas fatias).~
Descreva o gráfico final para MEIO.
```

## Relatórios com dados

### 26. Relatório mensal de desempenho

**Objetivo:** produzir um relatório de resultados claro, comparativo e com recomendações.

```
AREA=[marketing, vendas, operação, produto], DADOS_DO_MES=[indicadores], METAS=[metas], MES_ANTERIOR=[dados do mês anterior]
Escreva o resumo executivo com os 3 destaques do mês.~
Monte a tabela de indicadores com realizado, meta, variação e status.~
Explique as variações relevantes com causas prováveis.~
Destaque vitórias e problemas.~
Sugira os gráficos para cada seção.~
Escreva as recomendações e o foco do próximo mês.
```

### 27. Storytelling com dados

**Objetivo:** transformar números em uma narrativa que convence e leva à ação.

```
DADOS=[principais números e análises], PUBLICO=[quem vai receber], DECISAO=[o que você quer que o público faça]
Defina a ideia central em uma frase com o "e daí?" para PUBLICO.~
Estruture a narrativa em contexto, conflito, descoberta e resolução.~
Selecione apenas os dados que sustentam a narrativa.~
Escreva os títulos de cada slide ou seção como afirmações.~
Proponha as visualizações com destaque para o ponto principal.~
Escreva o fechamento com DECISAO clara.
```

### 28. Explicar dados para quem não é técnico

**Objetivo:** comunicar análises complexas sem jargões.

```
ANALISE=[resultado técnico], PUBLICO=[perfil do público], CONTEXTO=[decisão envolvida]
Traduza cada termo técnico de ANALISE para linguagem comum.~
Use analogias e exemplos concretos.~
Arredonde números e use comparações compreensíveis.~
Explique o grau de incerteza sem confundir.~
Escreva a explicação em 5 tópicos.~
Prepare respostas para as perguntas prováveis de PUBLICO.
```

### 29. Dicionário de dados e definição de métricas

**Objetivo:** garantir que todo mundo calcule os números do mesmo jeito.

```
METRICAS=[métricas usadas na empresa], FONTES=[sistemas e tabelas], CONFUSOES=[divergências que já aconteceram]
Para cada métrica, escreva nome, definição, fórmula, fonte, frequência, responsável e exemplo.~
Resolva CONFUSOES definindo a versão oficial.~
Documente as tabelas e colunas de FONTES.~
Defina regras de nomenclatura.~
Crie o processo para criar ou alterar uma métrica.
```

### 30. Relatório de pesquisa quantitativa

**Objetivo:** apresentar os resultados de uma pesquisa com rigor e clareza.

```
PESQUISA=[objetivo e método], AMOSTRA=[tamanho e perfil], RESULTADOS=[tabelas e números], PUBLICO=[quem vai ler]
Escreva o sumário executivo com as principais descobertas.~
Descreva metodologia, amostra, margem de erro e limitações.~
Organize RESULTADOS por tema com gráficos sugeridos.~
Destaque os cruzamentos mais reveladores.~
Escreva as conclusões e recomendações.~
Monte o anexo com o questionário e as tabelas completas.
```

## Pesquisa e inteligência de mercado

### 31. Pesquisa de empresas de capital aberto beneficiadas pela IA
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** levantar, em lotes de 10, empresas listadas que ganham com a IA, com vantagens, avaliações e links. Conteúdo informativo, não é recomendação de investimento.

```
Usando sua capacidade de busca na web, quero que você pesquise as informações mais recentes sobre empresas de capital aberto que estão se beneficiando do crescimento da IA. Inclua uma coluna de URL onde eu possa saber mais sobre cada empresa, suas vantagens competitivas e as recomendações de analistas. Retorne isso em uma tabela no próprio chat. Vamos pesquisar em lotes de 10; quando eu disser "Mais", você encontra mais 10. Mantenha as informações breves e todas dentro da tabela. Exemplo: | Nome da empresa | Ticker | Vantagens competitivas | Recomendação dos analistas | URL | |--------------|--------------|------------------------------------------|------------------|----------------------------------------| | Empresa A | ABC | Tecnologia de IA líder, forte P&D | Compra forte | Link | | Empresa B | XYZ | Dominante em software de IA, muitas patentes | Compra moderada | Link | Forneça as informações mais recentes disponíveis. ~Mais ~ Mais ~ Mais
```

### 32. Pesquisa de mercado extensa sobre uma empresa de capital aberto
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** analisar finanças, competição, gestão, riscos, ações e ESG de uma empresa listada. Conteúdo informativo, não é recomendação de investimento.

```
TICKER=[código da ação], EMPRESA=[nome da empresa], SETOR=[setor de atuação] Forneça uma visão geral de EMPRESA (TICKER), incluindo seu modelo de negócio principal, produtos ou serviços-chave e posição no setor de SETOR.~Analise as demonstrações financeiras de EMPRESA dos últimos 5 anos. Calcule e interprete os principais indicadores financeiros, incluindo P/L, crescimento do LPA, relação dívida/patrimônio, liquidez corrente e retorno sobre o patrimônio. Identifique tendências relevantes ou sinais de alerta.~Examine as fontes de receita e as margens de lucro de EMPRESA. Detalhe a receita por linha de produto ou serviço e por região geográfica, se aplicável. Analise a estabilidade e o potencial de crescimento de cada fonte de receita.~Avalie a posição competitiva de EMPRESA em SETOR. Identifique os principais concorrentes, a participação de mercado de EMPRESA e seus diferenciais ou vantagens competitivas.~Analise a equipe de gestão de EMPRESA. Avalie a experiência e o histórico dos principais executivos, sua estrutura de remuneração e qualquer movimentação relevante de negociação por insiders.~Investigue a estratégia de crescimento de EMPRESA. Examine expansões recentes e planejadas, fusões e aquisições, investimentos em P&D e lançamentos de novos produtos ou serviços.~Avalie os riscos e desafios de EMPRESA. Considere riscos do setor, questões regulatórias, disrupções potenciais e vulnerabilidades específicas da empresa.~Analise o desempenho da ação de EMPRESA nos últimos 5 anos. Compare com os índices de mercado relevantes e com os principais concorrentes. Identifique eventos significativos que influenciaram o preço da ação.~Examine as opiniões e os preços-alvo de analistas para TICKER. Resuma os argumentos otimistas e pessimistas para a ação.~Investigue as práticas de governança corporativa de EMPRESA. Avalie a independência do conselho, os direitos dos acionistas e qualquer histórico de controvérsias ou questões legais.~Analise o histórico e a política de dividendos de EMPRESA, se aplicável. Calcule o dividend yield e o payout e avalie a sustentabilidade dos pagamentos.~Examine as práticas e notas ambientais, sociais e de governança (ESG) de EMPRESA. Avalie como esses fatores podem impactar o desempenho futuro e a percepção dos investidores.~Realize uma análise SWOT (forças, fraquezas, oportunidades e ameaças) de EMPRESA com base em todas as informações reunidas.~Forneça um resumo final da pesquisa, incluindo as principais descobertas, possíveis sinais de alerta e uma avaliação geral do potencial de investimento de EMPRESA. Inclua uma faixa de valuation sugerida para TICKER com base na análise.
```

### 33. Análise de concorrência com dados públicos

**Objetivo:** comparar concorrentes com números e evidências, não só impressões.

```
CONCORRENTES=[lista de empresas], MERCADO=[mercado], FONTES_PERMITIDAS=[sites, redes, avaliações, relatórios públicos], CRITERIOS=[preço, produto, presença digital, atendimento]
Defina os indicadores mensuráveis para cada item de CRITERIOS.~
Use a busca na web para coletar os dados de cada concorrente em FONTES_PERMITIDAS, citando a fonte.~
Monte a tabela comparativa com notas e evidências.~
Identifique padrões e lacunas de mercado.~
Crie um mapa de posicionamento com 2 eixos relevantes.~
Liste as oportunidades de diferenciação e o que monitorar mensalmente.
```

### 34. Análise de tendências de busca

**Objetivo:** entender o interesse do público ao longo do tempo e por região.

```
TERMOS=[termos ou produtos a comparar], REGIAO=[país ou estado], PERIODO=[período], OBJETIVO=[lançamento, conteúdo, estoque, investimento]
Explique como coletar os dados no Google Trends para TERMOS, REGIAO e PERIODO.~
Interprete a curva de cada termo: tendência, sazonalidade e picos.~
Compare o interesse relativo entre TERMOS e regiões.~
Liste as consultas relacionadas em ascensão e o que indicam.~
Traduza os achados em decisões para OBJETIVO.~
Defina um calendário de oportunidades.
```

### 35. Pesquisa e comparação de preços

**Objetivo:** mapear preços de mercado para precificar melhor.

```
PRODUTO=[produto ou serviço], CANAIS=[lojas, marketplaces, sites de concorrentes], REGIAO=[região], MEU_PRECO=[preço atual]
Defina a cesta de produtos comparáveis e os critérios de equivalência.~
Use a busca na web para levantar preços em CANAIS e REGIAO, registrando fonte e data.~
Calcule média, mediana, mínimo, máximo e dispersão.~
Posicione MEU_PRECO na distribuição.~
Considere frete, parcelamento e promoções na comparação.~
Recomende o posicionamento de preço e a frequência de monitoramento.
```

### 36. Análise de avaliações e comentários de clientes

**Objetivo:** extrair insights de reviews de você e dos concorrentes.

```
AVALIACOES=[textos das avaliações], FONTES=[loja, Google, app, marketplace], EMPRESAS=[sua empresa e concorrentes]
Classifique cada avaliação por sentimento e tema (produto, entrega, atendimento, preço).~
Calcule a frequência e o sentimento médio por tema e empresa.~
Liste os elogios e as reclamações mais citados.~
Identifique o que os clientes valorizam nos concorrentes e não encontram em você.~
Extraia frases reais úteis para a comunicação, com autorização quando necessário.~
Proponha melhorias priorizadas.
```

### 37. Análise com dados públicos oficiais

**Objetivo:** usar dados do IBGE, governo e outras fontes abertas para embasar decisões.

```
PERGUNTA=[o que quer descobrir: tamanho do público, renda, crescimento de uma região], REGIAO=[local], NEGOCIO=[contexto]
Indique as bases públicas adequadas para PERGUNTA (IBGE, Caged, Datasus, Inep, Banco Central, portais de dados abertos).~
Explique como acessar e filtrar os dados.~
Defina os indicadores a extrair.~
Mostre como cruzar os dados para estimar a resposta.~
Interprete os resultados para NEGOCIO.~
Liste as limitações e a data de atualização de cada fonte.
```

## Projetos de dados

### 38. Análise de churn (cancelamento)

**Objetivo:** entender quem cancela, por quê e como prever.

```
DADOS=[clientes, datas de entrada e saída, plano, uso, atendimentos], NEGOCIO=[tipo], FERRAMENTA=[Excel, Python, SQL]
Calcule a taxa de churn por período e por segmento.~
Compare o perfil de quem cancelou com o de quem ficou.~
Identifique os sinais de alerta que antecedem o cancelamento.~
Proponha um modelo simples de pontuação de risco e escreva o código ou as fórmulas.~
Estime o impacto financeiro do churn.~
Proponha ações de retenção por nível de risco.
```

### 39. Dimensionamento de mercado (TAM, SAM e SOM)

**Objetivo:** estimar o tamanho do mercado com metodologia transparente.

```
PRODUTO=[produto], CLIENTE=[cliente-alvo], REGIAO=[região], PRECO=[preço médio], FONTES=[dados disponíveis]
Explique a diferença entre TAM, SAM e SOM.~
Calcule o TAM de cima para baixo com dados de mercado, citando fontes.~
Calcule o TAM de baixo para cima (número de clientes × PRECO × frequência).~
Defina o SAM com os recortes de REGIAO e CLIENTE.~
Estime o SOM realista para 3 anos com premissas explícitas.~
Compare as abordagens e explique as divergências.
```

### 40. Análise de cesta de compras

**Objetivo:** descobrir quais produtos são comprados juntos para criar combos e recomendações.

```
PEDIDOS=[pedido e itens], LOJA=[tipo de loja], FERRAMENTA=[Python, SQL, Excel]
Prepare os dados no formato de transações.~
Calcule suporte, confiança e lift dos pares de produtos.~
Escreva o código ou as consultas em FERRAMENTA.~
Liste as 10 associações mais fortes e relevantes.~
Interprete os resultados para LOJA.~
Proponha combos, vendas cruzadas e disposição de produtos.
```

### 41. Projeto de dados de ponta a ponta

**Objetivo:** ir de uma pergunta de negócio até uma recomendação baseada em dados.

```
PERGUNTA_DE_NEGOCIO=[pergunta], DADOS_DISPONIVEIS=[fontes], PRAZO=[tempo], PUBLICO=[quem vai usar o resultado]
Transforme PERGUNTA_DE_NEGOCIO em perguntas analíticas mensuráveis.~
Mapeie quais DADOS_DISPONIVEIS respondem cada pergunta e o que falta.~
Planeje as etapas: coleta, limpeza, exploração, análise, visualização e comunicação.~
Defina as hipóteses e como testá-las.~
Escreva o plano de análise com cronograma em PRAZO.~
Defina o formato da entrega para PUBLICO e os critérios de sucesso.
```

### 42. Auditoria de qualidade de dados

**Objetivo:** avaliar se os dados de uma empresa são confiáveis para decisões.

```
SISTEMAS=[fontes de dados], DADOS_CRITICOS=[dados mais importantes], PROBLEMAS_RELATADOS=[reclamações sobre números]
Defina as dimensões de qualidade (completude, precisão, consistência, atualidade, unicidade).~
Crie testes para cada dimensão em DADOS_CRITICOS.~
Investigue as causas de PROBLEMAS_RELATADOS.~
Classifique os problemas por impacto.~
Proponha correções e controles preventivos.~
Defina responsáveis e um painel de qualidade de dados.
```
