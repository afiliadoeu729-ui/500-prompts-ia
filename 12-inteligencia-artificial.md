# Inteligência artificial

> Engenharia de prompts, automações, agentes de IA, estratégia e aprendizado de IA.

**42 prompts** nesta categoria — 1 do repositório original PromptChains (marcados com 🔁) e 41 novos.

**Como usar:** copie o bloco inteiro de um prompt, substitua os campos entre colchetes `[...]` pelas suas informações e cole no ChatGPT, Claude, Gemini ou em uma extensão de fila de prompts (como o ChatGPT Queue). Cada trecho separado por `~` é uma etapa: em uma extensão de fila, as etapas são enviadas uma a uma automaticamente; sem extensão, envie uma etapa por vez, na ordem.

[← Voltar ao índice geral](README.md)

## Índice

**[Engenharia de prompts](#engenharia-de-prompts)**

1. [Otimizar e refinar um prompt personalizado](#1-otimizar-e-refinar-um-prompt-personalizado) 🔁
2. [Prompt de sistema para um assistente especializado](#2-prompt-de-sistema-para-um-assistente-especializado)
3. [Prompt com exemplos (few-shot)](#3-prompt-com-exemplos-few-shot)
4. [Criar sua própria cadeia de prompts](#4-criar-sua-própria-cadeia-de-prompts)
5. [Saída estruturada em JSON](#5-saída-estruturada-em-json)
6. [Testes e avaliação de prompts](#6-testes-e-avaliação-de-prompts)
7. [Modelo de prompt reutilizável](#7-modelo-de-prompt-reutilizável)
8. [A IA me entrevista antes de responder](#8-a-ia-me-entrevista-antes-de-responder)
9. [Reduzir erros e invenções da IA](#9-reduzir-erros-e-invenções-da-ia)
10. [Verificação de respostas da IA](#10-verificação-de-respostas-da-ia)
11. [Prompt de papel especialista (persona)](#11-prompt-de-papel-especialista-persona)
12. [Raciocínio passo a passo para problemas difíceis](#12-raciocínio-passo-a-passo-para-problemas-difíceis)

**[Automações com IA](#automações-com-ia)**

13. [Mapear o que automatizar com IA](#13-mapear-o-que-automatizar-com-ia)
14. [Fluxo no-code com IA (Zapier, Make, n8n)](#14-fluxo-no-code-com-ia-zapier-make-n8n)
15. [Triagem automática de e-mails com IA](#15-triagem-automática-de-e-mails-com-ia)
16. [Chatbot de perguntas frequentes](#16-chatbot-de-perguntas-frequentes)
17. [Linha de produção de conteúdo com IA](#17-linha-de-produção-de-conteúdo-com-ia)
18. [Classificação e enriquecimento em massa em planilhas](#18-classificação-e-enriquecimento-em-massa-em-planilhas)
19. [Relatórios automáticos com IA](#19-relatórios-automáticos-com-ia)
20. [Integração com API de modelo de linguagem](#20-integração-com-api-de-modelo-de-linguagem)
21. [Processamento de documentos com IA](#21-processamento-de-documentos-com-ia)

**[Agentes de IA](#agentes-de-ia)**

22. [Projeto de um agente de IA](#22-projeto-de-um-agente-de-ia)
23. [Instruções para agente de atendimento ao cliente](#23-instruções-para-agente-de-atendimento-ao-cliente)
24. [Agente de pesquisa](#24-agente-de-pesquisa)
25. [Agente de pré-vendas (SDR)](#25-agente-de-pré-vendas-sdr)
26. [Sistema com vários agentes](#26-sistema-com-vários-agentes)
27. [Segurança e limites para agentes de IA](#27-segurança-e-limites-para-agentes-de-ia)
28. [Base de conhecimento para IA (RAG)](#28-base-de-conhecimento-para-ia-rag)
29. [Memória e contexto de um agente](#29-memória-e-contexto-de-um-agente)
30. [Agente pessoal de produtividade](#30-agente-pessoal-de-produtividade)

**[Estratégia e uso responsável de IA](#estratégia-e-uso-responsável-de-ia)**

31. [Estratégia de adoção de IA na empresa](#31-estratégia-de-adoção-de-ia-na-empresa)
32. [Governança e riscos de IA](#32-governança-e-riscos-de-ia)
33. [Escolher a ferramenta ou modelo de IA certo](#33-escolher-a-ferramenta-ou-modelo-de-ia-certo)
34. [Retorno sobre investimento de um projeto de IA](#34-retorno-sobre-investimento-de-um-projeto-de-ia)
35. [Capacitação da equipe em IA](#35-capacitação-da-equipe-em-ia)
36. [Casos de uso de IA por área](#36-casos-de-uso-de-ia-por-área)
37. [Copiloto pessoal: fluxos de trabalho diários com IA](#37-copiloto-pessoal-fluxos-de-trabalho-diários-com-ia)

**[Aprender IA](#aprender-ia)**

38. [Fundamentos de IA e modelos de linguagem](#38-fundamentos-de-ia-e-modelos-de-linguagem)
39. [Glossário de IA explicado](#39-glossário-de-ia-explicado)
40. [Avaliar notícias e promessas sobre IA](#40-avaliar-notícias-e-promessas-sobre-ia)
41. [Prompt, RAG ou ajuste fino: qual usar](#41-prompt-rag-ou-ajuste-fino-qual-usar)
42. [Projeto de portfólio com IA](#42-projeto-de-portfólio-com-ia)

---


## Engenharia de prompts

### 1. Otimizar e refinar um prompt personalizado
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** transformar uma ideia de prompt em uma versão clara, completa e eficaz.

```
Analise a seguinte ideia de prompt: [insira a ideia de prompt]~Reescreva o prompt para mais clareza e eficácia~Identifique melhorias ou acréscimos possíveis~Refine o prompt com base nas melhorias identificadas~Apresente o prompt final otimizado
```

### 2. Prompt de sistema para um assistente especializado

**Objetivo:** criar as instruções permanentes de um assistente de IA com papel, regras e formato.

```
FUNCAO=[o que o assistente faz], USUARIOS=[quem vai usar], CONHECIMENTO=[informações que ele precisa saber], LIMITES=[o que não deve fazer], TOM=[estilo de resposta]
Defina a missão do assistente em 2 frases.~
Liste as tarefas que ele deve executar e as que deve recusar ou encaminhar.~
Escreva as regras de comportamento em ordem de prioridade, explicando o porquê de cada uma.~
Defina como lidar com informações faltantes, pedidos ambíguos e erros.~
Defina o formato padrão das respostas e exemplos de resposta boa e ruim.~
Inclua CONHECIMENTO em uma seção de contexto organizada.~
Escreva o prompt de sistema completo com seções delimitadas.~
Crie 10 mensagens de teste, incluindo casos difíceis, para validar o comportamento.
```

### 3. Prompt com exemplos (few-shot)

**Objetivo:** ensinar a IA um padrão de resposta mostrando exemplos.

```
TAREFA=[classificar, reescrever, extrair, responder], ENTRADAS_EXEMPLO=[exemplos reais de entrada], SAIDA_DESEJADA=[como cada saída deve ficar]
Analise ENTRADAS_EXEMPLO e defina o padrão que a IA deve aprender.~
Selecione de 3 a 5 exemplos diversos, incluindo um caso de borda.~
Escreva a saída ideal para cada exemplo em SAIDA_DESEJADA.~
Monte o prompt com instrução, exemplos delimitados e a nova entrada.~
Explique como evitar que a IA copie os exemplos ao pé da letra.~
Teste mentalmente com 3 entradas novas e ajuste os exemplos.
```

### 4. Criar sua própria cadeia de prompts

**Objetivo:** transformar qualquer tarefa complexa em uma cadeia de prompts separada por ~, no estilo deste pacote.

```
TAREFA=[o que você quer produzir], ENTRADAS=[informações que o usuário vai fornecer], RESULTADO_FINAL=[formato da entrega], NIVEL_DE_DETALHE=[rápido ou profundo]
Liste as variáveis de entrada da tarefa no formato NOME_DA_VARIAVEL=[descrição].~
Decomponha TAREFA nas etapas que um especialista humano seguiria, da pesquisa à revisão.~
Garanta que as primeiras etapas construam contexto (análise, pesquisa, estrutura) antes da produção.~
Escreva cada etapa como uma instrução autocontida, com números, formatos e critérios de qualidade.~
Inclua uma etapa final de revisão e compilação em RESULTADO_FINAL.~
Monte a cadeia completa com as etapas separadas por ~.~
Revise a cadeia removendo etapas redundantes e verificando se cada uma usa as variáveis corretas.
```

### 5. Saída estruturada em JSON

**Objetivo:** fazer a IA responder sempre no formato exato que um sistema precisa ler.

```
DADOS_DE_ENTRADA=[tipo de texto a processar], CAMPOS=[campos a extrair, tipos e regras], USO=[onde o JSON será consumido]
Defina o esquema JSON com tipos, campos obrigatórios e valores permitidos.~
Defina o que fazer quando uma informação não existir no texto (nulo, vazio, valor padrão).~
Escreva o prompt com instrução, esquema e um exemplo completo.~
Inclua a regra de responder apenas com o JSON válido.~
Escreva o código de validação do JSON no lado de USO.~
Liste os erros comuns e como corrigi-los com novas tentativas automáticas.
```

### 6. Testes e avaliação de prompts

**Objetivo:** medir se um prompt funciona bem antes de usá-lo em escala.

```
PROMPT=[prompt atual], TAREFA=[o que ele deve fazer], CASOS_REAIS=[exemplos de uso], CRITERIOS=[o que é uma boa resposta]
Transforme CRITERIOS em uma rubrica de avaliação com notas de 1 a 5.~
Crie um conjunto de 20 casos de teste: comuns, difíceis, ambíguos e maliciosos.~
Defina a resposta esperada ou os requisitos para cada caso.~
Descreva como rodar os testes e registrar os resultados.~
Explique como usar outra IA como avaliadora e os cuidados com esse método.~
Analise as falhas mais prováveis de PROMPT e proponha a versão 2.~
Defina o critério para considerar o prompt pronto.
```

### 7. Modelo de prompt reutilizável

**Objetivo:** transformar um prompt que deu certo em um modelo para reutilizar sempre.

```
PROMPT_QUE_FUNCIONOU=[prompt e resposta que você gostou], VARIACOES=[situações em que quer reutilizar]
Identifique as partes fixas e as partes variáveis de PROMPT_QUE_FUNCIONOU.~
Transforme as partes variáveis em campos [ENTRE_COLCHETES] com descrição.~
Adicione instruções de formato e de qualidade que estavam implícitas.~
Teste o modelo em 3 VARIACOES e ajuste.~
Escreva instruções de uso do modelo.~
Sugira um nome e uma categoria para a sua biblioteca de prompts.
```

### 8. A IA me entrevista antes de responder

**Objetivo:** fazer a IA levantar os requisitos com perguntas antes de executar uma tarefa.

```
TAREFA=[o que você quer], CONTEXTO_INICIAL=[o pouco que você já sabe]
Antes de começar, liste as informações que faltam para executar TAREFA com excelência.~
Faça as perguntas mais importantes, no máximo 5 por vez, com opções de resposta quando possível, e aguarde minhas respostas.~
Resuma o que entendeu e confirme comigo.~
Proponha a abordagem e o formato da entrega.~
Execute a tarefa com base nas respostas.~
Liste as suposições que fez e o que mudaria se elas estiverem erradas.
```

### 9. Reduzir erros e invenções da IA

**Objetivo:** obter respostas mais confiáveis, com fontes e reconhecimento de incerteza.

```
PERGUNTA=[sua pergunta], MATERIAL_DE_REFERENCIA=[documentos ou fontes fornecidas, se houver], NIVEL_DE_RISCO=[baixo, médio, alto]
Responda somente com base em MATERIAL_DE_REFERENCIA quando ele for fornecido e diga explicitamente quando a resposta não estiver nele.~
Para cada afirmação importante, indique a fonte ou o trecho que a sustenta.~
Separe o que é fato, o que é inferência e o que é opinião.~
Indique o nível de confiança de cada parte da resposta.~
Liste o que deveria ser verificado por um humano, considerando NIVEL_DE_RISCO.~
Ao final, revise a própria resposta procurando afirmações sem evidência e corrija.
```

### 10. Verificação de respostas da IA

**Objetivo:** checar uma resposta gerada por IA antes de usá-la.

```
RESPOSTA_DA_IA=[texto a verificar], USO=[onde será usada], FONTES_DISPONIVEIS=[fontes para conferência]
Liste todas as afirmações verificáveis de RESPOSTA_DA_IA (datas, números, nomes, citações, leis).~
Classifique cada afirmação por risco caso esteja errada.~
Verifique as afirmações com FONTES_DISPONIVEIS ou com busca na web, citando a fonte.~
Marque cada uma como confirmada, incorreta ou não verificável.~
Reescreva a resposta corrigida.~
Liste os cuidados para USO.
```

### 11. Prompt de papel especialista (persona)

**Objetivo:** fazer a IA raciocinar como um especialista específico com critérios explícitos.

```
ESPECIALIDADE=[ex.: advogado tributarista, nutricionista esportivo, engenheiro de software sênior], SITUACAO=[o problema], PUBLICO_DA_RESPOSTA=[para quem é a resposta]
Descreva como um profissional de ESPECIALIDADE abordaria SITUACAO: perguntas que faria, dados que pediria e métodos que usaria.~
Faça essas perguntas e aguarde minhas respostas.~
Analise SITUACAO com os frameworks da área, explicando cada passo.~
Apresente opções com prós, contras e riscos.~
Adapte a linguagem para PUBLICO_DA_RESPOSTA.~
Indique quando a situação exige um profissional humano habilitado.
```

### 12. Raciocínio passo a passo para problemas difíceis

**Objetivo:** fazer a IA resolver problemas complexos de forma estruturada e verificável.

```
PROBLEMA=[descrição], RESTRICOES=[condições], CRITERIO_DE_SUCESSO=[como saber que está certo]
Reformule PROBLEMA e liste o que é dado, o que é pedido e as RESTRICOES.~
Proponha 2 ou 3 abordagens diferentes e escolha a mais promissora, justificando.~
Resolva passo a passo, mostrando os cálculos ou o raciocínio.~
Verifique a solução contra CRITERIO_DE_SUCESSO e contra as RESTRICOES.~
Resolva por outra abordagem para conferir, se possível.~
Apresente a resposta final de forma resumida.
```

## Automações com IA

### 13. Mapear o que automatizar com IA

**Objetivo:** encontrar as tarefas que mais valem a pena automatizar no seu trabalho ou empresa.

```
ROTINA=[tarefas que você ou a equipe fazem], VOLUME=[frequência e tempo gasto em cada uma], FERRAMENTAS=[sistemas que já usam], ORCAMENTO=[quanto pode investir]
Liste as tarefas de ROTINA e estime as horas por mês.~
Classifique cada tarefa por potencial de automação (repetitiva, baseada em regras, baseada em texto, exige julgamento).~
Indique o tipo de solução para cada uma: automação simples, IA generativa, agente ou nada.~
Estime a economia de tempo e a complexidade.~
Priorize em uma matriz de impacto e esforço.~
Descreva a solução das 3 prioridades usando FERRAMENTAS e ORCAMENTO.~
Liste os riscos e onde manter revisão humana.
```

### 14. Fluxo no-code com IA (Zapier, Make, n8n)

**Objetivo:** montar uma automação que conecta apps e usa IA no meio do caminho.

```
GATILHO=[o que inicia o fluxo], PASSOS=[o que deve acontecer], APPS=[aplicativos envolvidos], FERRAMENTA=[Zapier, Make, n8n, Power Automate]
Desenhe o fluxo completo do GATILHO ao resultado, com decisões e ramificações.~
Indique os módulos de FERRAMENTA necessários em cada passo.~
Escreva o prompt da etapa de IA com entrada, instrução e formato de saída estruturado.~
Defina o tratamento de erros e as notificações de falha.~
Defina onde há aprovação humana.~
Estime o consumo de operações e o custo mensal.~
Escreva o passo a passo de configuração e de teste.
```

### 15. Triagem automática de e-mails com IA

**Objetivo:** classificar, resumir e encaminhar e-mails automaticamente.

```
TIPOS_DE_EMAIL=[categorias que chegam], ACOES=[o que fazer com cada categoria], FERRAMENTA=[Gmail, Outlook, automação], VOLUME=[e-mails por dia]
Defina as categorias e os critérios de classificação de TIPOS_DE_EMAIL.~
Escreva o prompt de classificação com saída em JSON (categoria, prioridade, resumo, ação sugerida).~
Defina as ACOES automáticas para cada categoria (etiquetar, encaminhar, rascunhar resposta).~
Escreva os modelos de resposta que a IA vai personalizar.~
Defina as regras de segurança (nunca enviar sem revisão em casos sensíveis).~
Descreva a implementação em FERRAMENTA e como medir a precisão.
```

### 16. Chatbot de perguntas frequentes

**Objetivo:** criar um atendimento automático que responde dúvidas comuns e passa para humanos quando precisa.

```
NEGOCIO=[tipo], PERGUNTAS_FREQUENTES=[dúvidas e respostas], CANAL=[site, WhatsApp, Instagram], HORARIO_HUMANO=[quando há atendentes]
Organize PERGUNTAS_FREQUENTES em uma base de conhecimento por tema.~
Escreva o prompt de sistema do chatbot com tom, limites e regras de resposta.~
Defina quando e como transferir para um humano.~
Escreva a mensagem de boas-vindas e as respostas para fora de HORARIO_HUMANO.~
Crie 20 perguntas de teste, incluindo tentativas de tirar o bot do tema.~
Defina as métricas (resolução, transferência, satisfação) e a rotina de melhoria da base.
```

### 17. Linha de produção de conteúdo com IA

**Objetivo:** produzir conteúdo em escala com IA mantendo qualidade e voz da marca.

```
TIPO_DE_CONTEUDO=[posts, artigos, roteiros, descrições], VOLUME=[quantidade por semana], VOZ=[guia de voz da marca], FONTES=[de onde vêm as ideias e informações]
Desenhe as etapas: ideação, pesquisa, rascunho, revisão, adaptação e publicação.~
Defina o que a IA faz e o que o humano faz em cada etapa.~
Escreva os prompts de cada etapa, incluindo VOZ.~
Crie o checklist de revisão humana (fatos, tom, originalidade, direitos de uso).~
Defina as ferramentas e o fluxo de aprovação.~
Defina indicadores de qualidade e produtividade.
```

### 18. Classificação e enriquecimento em massa em planilhas

**Objetivo:** usar IA para categorizar ou resumir milhares de linhas.

```
PLANILHA=[colunas e exemplo de linhas], TAREFA=[classificar, extrair, resumir, traduzir, pontuar], CATEGORIAS=[categorias possíveis], FERRAMENTA=[Sheets com IA, Excel, Python com API]
Defina a saída exata desejada para cada linha.~
Escreva o prompt por linha com CATEGORIAS e exemplos.~
Escreva a fórmula, o script ou o código para processar as linhas em lotes em FERRAMENTA.~
Defina como lidar com respostas fora do padrão.~
Crie uma amostra de validação manual para medir a precisão.~
Estime custo e tempo de processamento.
```

### 19. Relatórios automáticos com IA

**Objetivo:** gerar relatórios recorrentes a partir de dados, com análise escrita pela IA.

```
DADOS=[fonte e métricas], PERIODICIDADE=[diário, semanal, mensal], PUBLICO=[quem recebe], FORMATO=[e-mail, documento, mensagem]
Defina as métricas e comparações que o relatório deve trazer.~
Desenhe o fluxo: coleta, cálculo, análise pela IA, montagem e envio.~
Escreva o prompt de análise que recebe os números e produz comentários objetivos sem inventar causas.~
Defina o modelo do relatório em FORMATO.~
Escreva o código ou a automação para agendar o envio.~
Defina as verificações para evitar números errados.
```

### 20. Integração com API de modelo de linguagem

**Objetivo:** usar um modelo de IA dentro do seu próprio código ou sistema.

```
LINGUAGEM=[Python, JavaScript etc.], PROVEDOR=[API do modelo escolhido], CASO_DE_USO=[o que a integração faz], VOLUME=[chamadas por dia]
Explique a arquitetura básica: chamada da API, prompt de sistema, mensagens e parâmetros.~
Escreva o código mínimo funcional em LINGUAGEM para CASO_DE_USO, lendo a chave de uma variável de ambiente.~
Adicione tratamento de erros, tentativas e limites de tempo.~
Adicione respostas em streaming, se fizer sentido.~
Implemente o controle de custos (limite de tokens, cache, modelo adequado ao VOLUME).~
Liste as boas práticas de segurança (não expor a chave, validar entradas, filtrar saídas).~
Escreva testes básicos.
```

### 21. Processamento de documentos com IA

**Objetivo:** extrair dados de contratos, notas, currículos ou formulários automaticamente.

```
DOCUMENTOS=[tipo e formato], CAMPOS=[informações a extrair], DESTINO=[planilha, sistema, banco], VOLUME=[quantidade]
Defina o esquema de saída com CAMPOS e regras.~
Descreva o fluxo: entrada do arquivo, leitura (texto ou OCR), extração pela IA, validação e envio para DESTINO.~
Escreva o prompt de extração com exemplos.~
Defina regras de validação automática (formatos, totais, campos obrigatórios).~
Defina quando um documento vai para revisão humana.~
Liste os cuidados de privacidade e de LGPD com DOCUMENTOS.
```

## Agentes de IA

### 22. Projeto de um agente de IA

**Objetivo:** desenhar um agente com objetivo, ferramentas, limites e critérios de sucesso.

```
OBJETIVO_DO_AGENTE=[o que ele deve conseguir], USUARIOS=[para quem], FERRAMENTAS_DISPONIVEIS=[busca, e-mail, planilhas, APIs, código], RISCOS=[o que pode dar errado]
Defina se o problema realmente exige um agente ou se um fluxo fixo resolve.~
Descreva o ciclo do agente: entender a tarefa, planejar, agir com ferramentas, verificar e entregar.~
Liste as ferramentas necessárias com descrição clara de cada uma.~
Defina os limites: ações que exigem aprovação humana, ações proibidas e orçamento de passos.~
Escreva as instruções do agente.~
Defina como ele lida com falhas, ambiguidades e informações faltantes.~
Crie os cenários de teste e as métricas de sucesso.
```

### 23. Instruções para agente de atendimento ao cliente

**Objetivo:** criar um agente que resolve solicitações de clientes com segurança.

```
EMPRESA=[descrição], SOLICITACOES=[tipos de pedidos], SISTEMAS=[o que o agente pode consultar ou alterar], POLITICAS=[regras de troca, reembolso, prazos]
Defina o escopo: o que o agente resolve sozinho e o que transfere.~
Escreva as instruções com tom, POLITICAS e passo a passo para cada tipo de SOLICITACOES.~
Defina as verificações de identidade antes de ações sensíveis.~
Defina as ações em SISTEMAS que exigem confirmação do cliente.~
Escreva as mensagens de transferência para humano.~
Crie 15 conversas de teste, incluindo clientes irritados e pedidos fora da política.
```

### 24. Agente de pesquisa

**Objetivo:** configurar um agente que pesquisa, cruza fontes e entrega relatórios confiáveis.

```
TEMA=[tema da pesquisa], PROFUNDIDADE=[rápida ou aprofundada], FONTES_PREFERIDAS=[tipos de fonte confiáveis], FORMATO=[relatório, tabela, resumo]
Defina como o agente transforma TEMA em perguntas de pesquisa.~
Defina a estratégia de busca e os critérios de qualidade de fonte.~
Defina como registrar cada achado com fonte e data.~
Defina como lidar com fontes conflitantes.~
Escreva as instruções completas do agente.~
Defina o FORMATO de entrega com seção de limitações e lista de fontes.
```

### 25. Agente de pré-vendas (SDR)

**Objetivo:** usar IA para pesquisar contas e preparar abordagens personalizadas, com revisão humana.

```
ICP=[perfil de cliente ideal], SOLUCAO=[o que vende], FONTES=[onde pesquisar], CANAIS=[e-mail, LinkedIn], REGRAS=[limites de contato e conformidade com a LGPD]
Defina o fluxo: receber a conta, pesquisar, pontuar aderência, redigir a abordagem e enviar para aprovação.~
Escreva as instruções de pesquisa da conta usando apenas dados públicos e profissionais.~
Escreva os critérios de pontuação com base em ICP.~
Escreva o prompt de redação da mensagem personalizada.~
Defina REGRAS de envio, frequência e descadastro.~
Defina as métricas e a revisão semanal de qualidade.
```

### 26. Sistema com vários agentes

**Objetivo:** dividir um trabalho complexo entre agentes especializados coordenados.

```
TRABALHO=[tarefa complexa], ETAPAS=[partes do trabalho], FERRAMENTAS=[ferramentas por etapa], QUALIDADE=[critérios de aceite]
Avalie se múltiplos agentes trazem ganho real em relação a um agente único.~
Defina os papéis (orquestrador, especialistas, revisor) e a responsabilidade de cada um.~
Defina o que cada agente recebe e entrega, com formatos estruturados.~
Escreva as instruções de cada agente.~
Defina como o orquestrador lida com falhas e conflitos.~
Defina a verificação final contra QUALIDADE e o custo estimado.
```

### 27. Segurança e limites para agentes de IA

**Objetivo:** proteger um agente contra erros, abusos e ações indesejadas.

```
AGENTE=[o que ele faz], ACOES_POSSIVEIS=[o que pode executar], DADOS=[a que dados tem acesso], USUARIOS=[quem interage]
Classifique ACOES_POSSIVEIS por risco e reversibilidade.~
Defina as ações que exigem confirmação humana.~
Defina o princípio de menor privilégio para DADOS e ferramentas.~
Liste os riscos de injeção de instruções em conteúdos externos e como mitigá-los.~
Defina os registros de auditoria e o monitoramento.~
Crie os testes de abuso e o plano de resposta a incidentes.
```

### 28. Base de conhecimento para IA (RAG)

**Objetivo:** fazer a IA responder com base nos documentos da empresa.

```
DOCUMENTOS=[tipos e volume de documentos], PERGUNTAS_TIPICAS=[o que os usuários perguntam], ATUALIZACAO=[frequência de mudança], FERRAMENTA=[plataforma ou stack]
Explique como funciona a geração aumentada por recuperação em linguagem simples.~
Defina como preparar DOCUMENTOS: limpeza, divisão em trechos e metadados.~
Defina a estratégia de busca (semântica, palavra-chave ou híbrida).~
Escreva o prompt que obriga a resposta a usar os trechos recuperados e citar a fonte.~
Defina o processo de ATUALIZACAO.~
Crie um conjunto de avaliação com PERGUNTAS_TIPICAS e respostas esperadas.
```

### 29. Memória e contexto de um agente

**Objetivo:** decidir o que o agente deve lembrar e como gerenciar o contexto.

```
AGENTE=[função], INTERACOES=[como e com que frequência é usado], INFORMACOES=[o que poderia ser lembrado], PRIVACIDADE=[restrições]
Classifique INFORMACOES em: necessárias na conversa, úteis entre conversas e que nunca devem ser guardadas.~
Defina o formato e a organização da memória de longo prazo.~
Defina regras de escrita, atualização e exclusão de memórias.~
Defina como resumir conversas longas sem perder decisões.~
Defina os controles do usuário sobre o que é lembrado, respeitando PRIVACIDADE.~
Teste com 5 cenários de uso.
```

### 30. Agente pessoal de produtividade

**Objetivo:** montar um assistente de IA que organiza sua rotina, e-mails e tarefas.

```
ROTINA=[como é seu dia], FERRAMENTAS=[agenda, e-mail, notas, tarefas], PREFERENCIAS=[como gosta de trabalhar], LIMITES=[o que o assistente não pode fazer sem você]
Liste as tarefas recorrentes que o assistente pode assumir.~
Escreva as instruções do assistente com PREFERENCIAS e LIMITES.~
Crie os rituais: resumo matinal, planejamento do dia, revisão semanal.~
Escreva os prompts de cada ritual.~
Defina as integrações com FERRAMENTAS.~
Defina como avaliar, após 2 semanas, se ele está economizando tempo.
```

## Estratégia e uso responsável de IA

### 31. Estratégia de adoção de IA na empresa

**Objetivo:** planejar como a empresa vai usar IA com resultado e segurança.

```
EMPRESA=[setor e tamanho], AREAS=[áreas da empresa], MATURIDADE=[uso atual de IA], OBJETIVOS=[eficiência, receita, experiência do cliente], RESTRICOES=[orçamento, dados, regulação]
Diagnostique MATURIDADE e os principais obstáculos.~
Liste casos de uso por item de AREAS com valor e viabilidade.~
Priorize de 3 a 5 casos de uso para os primeiros 6 meses.~
Defina os pilotos com indicadores de sucesso.~
Defina a governança: dados, segurança, aprovação e responsabilidades.~
Defina o plano de capacitação das pessoas.~
Monte o roadmap de 12 meses.
```

### 32. Governança e riscos de IA

**Objetivo:** criar regras para o uso de IA que protejam a empresa e as pessoas.

```
EMPRESA=[descrição], USOS_ATUAIS=[como a IA já é usada], DADOS_SENSIVEIS=[tipos de dado tratados], SETOR=[setor e regulação aplicável]
Mapeie USOS_ATUAIS e classifique por risco.~
Defina o que pode e o que não pode ser inserido em ferramentas de IA, considerando DADOS_SENSIVEIS e a LGPD.~
Defina as ferramentas aprovadas e o processo para aprovar novas.~
Defina as regras de revisão humana, transparência e propriedade intelectual.~
Escreva a política de uso de IA em linguagem simples.~
Defina o treinamento e o canal para dúvidas e incidentes.
```

### 33. Escolher a ferramenta ou modelo de IA certo

**Objetivo:** comparar opções de IA para uma tarefa específica com critérios objetivos.

```
TAREFA=[o que precisa ser feito], OPCOES=[ferramentas ou modelos considerados], CRITERIOS=[qualidade, custo, privacidade, integração, idioma, velocidade], VOLUME=[uso esperado]
Use a busca na web para levantar as informações atualizadas de cada item de OPCOES.~
Defina os pesos de CRITERIOS para TAREFA.~
Crie um teste prático com 5 entradas reais para comparar as opções.~
Monte a matriz de comparação com notas e evidências.~
Estime o custo mensal para VOLUME.~
Recomende a opção e um plano B.
```

### 34. Retorno sobre investimento de um projeto de IA

**Objetivo:** justificar um projeto de IA com números.

```
PROJETO=[descrição], PROCESSO_ATUAL=[tempo, custo e erros hoje], GANHO_ESPERADO=[redução de tempo ou aumento de receita], CUSTOS=[ferramentas, desenvolvimento, manutenção, treinamento]
Calcule o custo atual de PROCESSO_ATUAL por mês.~
Estime GANHO_ESPERADO em cenários conservador, base e otimista.~
Liste todos os CUSTOS, incluindo os ocultos (revisão humana, erros, governança).~
Calcule o retorno sobre o investimento e o payback em cada cenário.~
Liste os benefícios qualitativos.~
Defina os indicadores do piloto que vão confirmar ou refutar as estimativas.
```

### 35. Capacitação da equipe em IA

**Objetivo:** ensinar a equipe a usar IA no dia a dia com segurança e produtividade.

```
EQUIPE=[áreas e nível de familiaridade], FERRAMENTAS=[ferramentas aprovadas], TAREFAS_COMUNS=[tarefas do dia a dia], TEMPO=[horas disponíveis]
Crie um diagnóstico rápido de familiaridade com IA.~
Monte uma trilha de aprendizado em 4 módulos: fundamentos, escrita de prompts, casos de uso da área e uso responsável.~
Crie exercícios práticos com TAREFAS_COMUNS.~
Crie uma biblioteca inicial de prompts por área.~
Defina a figura de "embaixadores de IA" e a comunidade interna.~
Defina como medir a adoção e os ganhos.
```

### 36. Casos de uso de IA por área

**Objetivo:** descobrir como a IA pode ajudar cada área de um negócio.

```
NEGOCIO=[tipo de negócio], AREAS=[marketing, vendas, atendimento, finanças, RH, operações, jurídico, TI], FERRAMENTAS_ATUAIS=[ferramentas usadas]
Para cada área de AREAS, liste 5 casos de uso de IA concretos.~
Para cada caso, indique a tarefa atual, como a IA ajuda, o ganho estimado e o nível de risco.~
Indique os casos que funcionam com ferramentas prontas e os que exigem desenvolvimento.~
Selecione os 10 casos com melhor relação ganho e esforço.~
Escreva um prompt inicial para os 5 primeiros.
```

### 37. Copiloto pessoal: fluxos de trabalho diários com IA

**Objetivo:** incorporar IA na sua rotina de forma prática e consistente.

```
PROFISSAO=[o que você faz], ROTINA=[tarefas diárias e semanais], FERRAMENTAS_DE_IA=[ferramentas que você tem], DIFICULDADES=[onde perde mais tempo]
Liste as tarefas de ROTINA em que a IA pode acelerar ou melhorar o resultado.~
Para cada tarefa, desenhe o fluxo de uso: entrada, prompt, revisão e saída.~
Escreva os prompts prontos para as 10 tarefas mais frequentes.~
Defina o que nunca delegar à IA sem revisão.~
Crie um atalho ou uma biblioteca para acessar os prompts rapidamente.~
Defina como medir o tempo economizado.
```

## Aprender IA

### 38. Fundamentos de IA e modelos de linguagem

**Objetivo:** entender como a IA generativa funciona sem precisar de matemática avançada.

```
NIVEL=[iniciante, intermediário], OBJETIVO=[usar melhor, trabalhar com IA, curiosidade], AREA=[sua área de atuação]
Explique o que é inteligência artificial, aprendizado de máquina e modelos de linguagem, com analogias.~
Explique como um modelo de linguagem é treinado e como gera texto.~
Explique conceitos-chave: tokens, janela de contexto, temperatura, alucinação, ajuste fino e geração aumentada por recuperação.~
Explique o que a IA faz bem e o que faz mal hoje, com exemplos de AREA.~
Monte um plano de estudo de 4 semanas para OBJETIVO.~
Crie um teste de 10 perguntas para verificar meu entendimento.
```

### 39. Glossário de IA explicado

**Objetivo:** dominar os termos de IA que aparecem em notícias, vagas e reuniões.

```
CONTEXTO=[trabalho, estudos, negócios], NIVEL=[nível de profundidade]
Liste os 40 termos de IA mais importantes para CONTEXTO.~
Explique cada termo em uma frase simples e com um exemplo.~
Agrupe os termos por tema (modelos, dados, treinamento, uso, riscos, negócios).~
Indique os termos que costumam ser confundidos e a diferença entre eles.~
Gere flashcards em CSV para revisão.
```

### 40. Avaliar notícias e promessas sobre IA

**Objetivo:** separar avanços reais de exagero e marketing.

```
NOTICIA_OU_PROMESSA=[texto ou anúncio], CONTEXTO=[por que isso importa para você]
Resuma a afirmação central de NOTICIA_OU_PROMESSA.~
Identifique quem está fazendo a afirmação e seus interesses.~
Verifique se há evidências (estudos, demonstrações, testes independentes) usando a busca na web.~
Aponte sinais de exagero (generalizações, ausência de limitações, números sem fonte).~
Explique o que é realista esperar no curto prazo.~
Conclua o que isso significa para CONTEXTO.
```

### 41. Prompt, RAG ou ajuste fino: qual usar

**Objetivo:** escolher a técnica certa para adaptar a IA a uma necessidade.

```
NECESSIDADE=[o que precisa que a IA faça], DADOS=[dados disponíveis e volume], FREQUENCIA_DE_MUDANCA=[com que frequência a informação muda], ORCAMENTO=[recursos]
Explique as três abordagens (prompt bem feito, geração aumentada por recuperação e ajuste fino) com prós e contras.~
Avalie NECESSIDADE: o problema é de conhecimento, de formato ou de comportamento?~
Recomende a abordagem para DADOS, FREQUENCIA_DE_MUDANCA e ORCAMENTO.~
Descreva os passos de implementação da abordagem escolhida.~
Defina como avaliar se funcionou.
```

### 42. Projeto de portfólio com IA

**Objetivo:** construir um projeto prático de IA para aprender e mostrar no currículo.

```
NIVEL=[sem código, iniciante em programação, desenvolvedor], AREA_DE_INTERESSE=[área], TEMPO=[semanas disponíveis], OBJETIVO=[emprego, freela, aprendizado]
Proponha 5 ideias de projeto que resolvem problemas reais de AREA_DE_INTERESSE.~
Escolha a ideia mais adequada a NIVEL e TEMPO.~
Defina escopo, ferramentas e arquitetura simples.~
Divida o projeto em tarefas semanais.~
Defina como documentar e apresentar o projeto (README, vídeo, post).~
Liste as melhorias futuras que mostram evolução.
```
