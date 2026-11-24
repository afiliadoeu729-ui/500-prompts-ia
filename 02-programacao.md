# Programação

> Desenvolvimento, debugging, código, qualidade, testes e documentação.

**42 prompts** nesta categoria — 2 do repositório original PromptChains (marcados com 🔁) e 40 novos.

**Como usar:** copie o bloco inteiro de um prompt, substitua os campos entre colchetes `[...]` pelas suas informações e cole no ChatGPT, Claude, Gemini ou em uma extensão de fila de prompts (como o ChatGPT Queue). Cada trecho separado por `~` é uma etapa: em uma extensão de fila, as etapas são enviadas uma a uma automaticamente; sem extensão, envie uma etapa por vez, na ordem.

[← Voltar ao índice geral](README.md)

## Índice

**[Desenvolvimento](#desenvolvimento)**

1. [Arquitetura de uma aplicação nova](#1-arquitetura-de-uma-aplicação-nova)
2. [Funcionalidade de ponta a ponta](#2-funcionalidade-de-ponta-a-ponta)
3. [API REST bem projetada](#3-api-rest-bem-projetada)
4. [Modelagem de banco de dados](#4-modelagem-de-banco-de-dados)
5. [Componente de front-end reutilizável](#5-componente-de-front-end-reutilizável)
6. [MVP de aplicativo mobile](#6-mvp-de-aplicativo-mobile)
7. [CRUD full stack completo](#7-crud-full-stack-completo)
8. [Autenticação e autorização seguras](#8-autenticação-e-autorização-seguras)
9. [Integração com API de terceiros e webhooks](#9-integração-com-api-de-terceiros-e-webhooks)
10. [Script de automação de tarefas repetitivas](#10-script-de-automação-de-tarefas-repetitivas)
11. [Ferramenta de linha de comando (CLI)](#11-ferramenta-de-linha-de-comando-cli)
12. [Migração de framework ou de versão](#12-migração-de-framework-ou-de-versão)

**[Debugging](#debugging)**

13. [Otimizar e explicar código](#13-otimizar-e-explicar-código) 🔁
14. [Suporte técnico de TI](#14-suporte-técnico-de-ti) 🔁
15. [Depuração a partir de mensagem de erro](#15-depuração-a-partir-de-mensagem-de-erro)
16. [Bug intermitente e condição de corrida](#16-bug-intermitente-e-condição-de-corrida)
17. [Diagnóstico de lentidão e desempenho](#17-diagnóstico-de-lentidão-e-desempenho)
18. [Vazamento de memória](#18-vazamento-de-memória)
19. [Incidente em produção e post-mortem](#19-incidente-em-produção-e-post-mortem)
20. [Consulta SQL com erro ou resultado errado](#20-consulta-sql-com-erro-ou-resultado-errado)

**[Qualidade, testes e revisão](#qualidade-testes-e-revisão)**

21. [Revisão de código (code review)](#21-revisão-de-código-code-review)
22. [Testes unitários com boa cobertura](#22-testes-unitários-com-boa-cobertura)
23. [Testes de ponta a ponta (E2E)](#23-testes-de-ponta-a-ponta-e2e)
24. [Refatoração de código legado](#24-refatoração-de-código-legado)
25. [Auditoria de segurança (OWASP)](#25-auditoria-de-segurança-owasp)
26. [Acessibilidade em interfaces web](#26-acessibilidade-em-interfaces-web)
27. [Pipeline de CI/CD](#27-pipeline-de-cicd)
28. [Containerização com Docker](#28-containerização-com-docker)
29. [Otimização de banco de dados e índices](#29-otimização-de-banco-de-dados-e-índices)

**[Documentação](#documentação)**

30. [README profissional](#30-readme-profissional)
31. [Documentação de API (OpenAPI)](#31-documentação-de-api-openapi)
32. [Registro de decisão de arquitetura (ADR)](#32-registro-de-decisão-de-arquitetura-adr)
33. [Comentários e docstrings](#33-comentários-e-docstrings)
34. [Guia de onboarding para novos desenvolvedores](#34-guia-de-onboarding-para-novos-desenvolvedores)
35. [Notas de versão e changelog](#35-notas-de-versão-e-changelog)
36. [Diagramas de sistema em Mermaid](#36-diagramas-de-sistema-em-mermaid)

**[Aprendizado e produtividade do desenvolvedor](#aprendizado-e-produtividade-do-desenvolvedor)**

37. [Aprender uma nova linguagem construindo um projeto](#37-aprender-uma-nova-linguagem-construindo-um-projeto)
38. [Explicar um conceito de programação em camadas](#38-explicar-um-conceito-de-programação-em-camadas)
39. [Resolver desafio de algoritmo passo a passo](#39-resolver-desafio-de-algoritmo-passo-a-passo)
40. [Converter código entre linguagens](#40-converter-código-entre-linguagens)
41. [Criar e explicar expressões regulares](#41-criar-e-explicar-expressões-regulares)
42. [Estimativa e quebra de tarefas técnicas](#42-estimativa-e-quebra-de-tarefas-técnicas)

---


## Desenvolvimento

### 1. Arquitetura de uma aplicação nova

**Objetivo:** sair da ideia para uma arquitetura técnica clara antes de escrever a primeira linha.

```
PROJETO=[descrição do sistema], USUARIOS=[quem usa e quantos], REQUISITOS=[funcionalidades principais], RESTRICOES=[prazo, orçamento, equipe, stack obrigatória]
Transforme PROJETO e REQUISITOS em uma lista de requisitos funcionais e não funcionais (desempenho, segurança, disponibilidade, escala), classificados por prioridade.~
Identifique as entidades principais do domínio e como se relacionam.~
Proponha 2 arquiteturas possíveis (ex.: monólito modular e serviços separados) com prós, contras e custo de manutenção para RESTRICOES.~
Recomende uma stack (linguagem, framework, banco, hospedagem, filas, cache) justificando cada escolha para USUARIOS.~
Desenhe a estrutura de pastas e módulos do projeto.~
Descreva os fluxos críticos (ex.: cadastro, pagamento) em sequência de chamadas entre componentes.~
Liste os riscos técnicos e como mitigar cada um.~
Divida a construção em marcos (MVP, versão 1, escala) com estimativa de esforço.~
Gere um diagrama de arquitetura em Mermaid e um resumo de 1 página para compartilhar com a equipe.
```

### 2. Funcionalidade de ponta a ponta

**Objetivo:** planejar e implementar uma feature completa com back-end, front-end e testes.

```
FUNCIONALIDADE=[o que precisa ser feito], STACK=[tecnologias do projeto], CODIGO_RELEVANTE=[trechos do código atual], CRITERIOS=[critérios de aceite]
Reescreva FUNCIONALIDADE como história de usuário e detalhe os CRITERIOS em cenários "dado, quando, então".~
Analise CODIGO_RELEVANTE e identifique onde a funcionalidade se encaixa e quais padrões do projeto devem ser seguidos.~
Liste as alterações necessárias em banco de dados, back-end, front-end e configurações.~
Implemente a camada de dados (migração e modelo).~
Implemente a lógica de negócio e os endpoints, com validação de entrada e tratamento de erros.~
Implemente a interface, incluindo estados de carregamento, vazio e erro.~
Escreva os testes automatizados que cobrem os CRITERIOS e os casos de borda.~
Revise todo o código gerado buscando falhas de segurança, duplicações e inconsistências com o padrão do projeto.~
Escreva a descrição do pull request com resumo, como testar e pontos de atenção.
```

### 3. API REST bem projetada

**Objetivo:** desenhar e implementar uma API consistente, segura e documentada.

```
DOMINIO=[sobre o que é a API], RECURSOS=[entidades principais], CONSUMIDORES=[app, site, parceiros], LINGUAGEM=[linguagem e framework]
Defina os recursos e os endpoints com métodos HTTP, rotas, parâmetros e códigos de status em uma tabela.~
Padronize convenções: nomes, paginação, filtros, ordenação, formato de erro e versionamento.~
Escreva os contratos de requisição e resposta em JSON para cada endpoint.~
Defina autenticação e autorização adequadas a CONSUMIDORES, além de limitação de requisições.~
Implemente os endpoints principais em LINGUAGEM, com validação e tratamento de erros centralizado.~
Escreva testes de integração para os fluxos principais.~
Gere a especificação OpenAPI correspondente.~
Liste melhorias futuras (cache, idempotência, webhooks) e um checklist de publicação em produção.
```

### 4. Modelagem de banco de dados

**Objetivo:** criar um modelo de dados normalizado, eficiente e fácil de evoluir.

```
SISTEMA=[descrição do sistema], REGRAS=[regras de negócio importantes], BANCO=[PostgreSQL, MySQL, MongoDB etc.], VOLUME=[volume de dados esperado]
Liste as entidades, atributos e tipos de dados a partir de SISTEMA e REGRAS.~
Defina os relacionamentos (1:1, 1:N, N:N) e as chaves primárias e estrangeiras.~
Normalize o modelo até a 3ª forma normal e indique onde a desnormalização é justificável para VOLUME.~
Escreva o script de criação das tabelas em BANCO, com restrições, valores padrão e campos de auditoria.~
Recomende índices com base nas consultas mais frequentes e explique cada um.~
Escreva 10 consultas de exemplo que o sistema vai precisar.~
Gere o diagrama entidade-relacionamento em Mermaid.~
Descreva a estratégia de migrações, backup e retenção de dados.
```

### 5. Componente de front-end reutilizável

**Objetivo:** construir um componente de interface acessível, tipado e testado.

```
COMPONENTE=[ex.: tabela com filtros, modal, upload de arquivos], FRAMEWORK=[React, Vue, Svelte, Angular], ESTILO=[CSS, Tailwind, styled-components], REQUISITOS=[comportamentos esperados]
Defina a API do componente: propriedades, eventos, estados internos e variações.~
Liste os estados visuais (padrão, foco, desabilitado, carregando, erro, vazio) e os requisitos de acessibilidade (teclado, leitores de tela, contraste).~
Implemente o componente em FRAMEWORK com tipagem.~
Aplique o estilo com ESTILO, garantindo responsividade.~
Escreva testes de comportamento e de acessibilidade.~
Crie exemplos de uso (documentação estilo Storybook).~
Revise desempenho: renderizações desnecessárias, memoização e tamanho do pacote.~
Entregue o código final organizado em arquivos com instruções de uso.
```

### 6. MVP de aplicativo mobile

**Objetivo:** planejar e construir a primeira versão de um app com o mínimo necessário para validar.

```
IDEIA=[o que o app faz], PUBLICO=[usuário], TECNOLOGIA=[React Native, Flutter, nativo], PRAZO=[semanas disponíveis]
Liste todas as funcionalidades imagináveis para IDEIA e classifique pelo método MoSCoW. Defina o escopo do MVP.~
Desenhe o fluxo de telas do MVP e descreva cada tela.~
Defina a arquitetura do app (navegação, estado, armazenamento local, comunicação com o servidor).~
Escolha o back-end (próprio ou serviço pronto) e justifique para PRAZO.~
Gere o código base: estrutura de pastas, navegação e as 3 telas principais em TECNOLOGIA.~
Implemente autenticação e persistência de dados.~
Crie o plano de testes com usuários reais e as métricas de validação.~
Liste os passos para publicar nas lojas de aplicativos e um cronograma semanal até PRAZO.
```

### 7. CRUD full stack completo

**Objetivo:** gerar um cadastro completo (criar, listar, editar, excluir) do banco à tela.

```
ENTIDADE=[ex.: clientes, produtos], CAMPOS=[campos e regras de validação], STACK=[tecnologias de back-end e front-end], BANCO=[banco de dados]
Defina o modelo de ENTIDADE com CAMPOS, tipos e validações.~
Escreva a migração ou o script de criação da tabela em BANCO.~
Implemente as rotas de criar, listar (com paginação, busca e filtro), detalhar, editar e excluir.~
Implemente validações no servidor com mensagens de erro claras.~
Construa as telas de listagem, formulário e confirmação de exclusão.~
Adicione validação no formulário e feedback visual para o usuário.~
Escreva testes para as regras de validação e para as rotas.~
Revise o código e entregue a estrutura final de arquivos com instruções para rodar localmente.
```

### 8. Autenticação e autorização seguras

**Objetivo:** implementar login, sessões e permissões seguindo boas práticas de segurança.

```
APLICACAO=[tipo de aplicação], STACK=[tecnologias], METODOS=[e-mail e senha, login social, link mágico, 2FA], PERFIS=[papéis de usuário e permissões]
Compare abordagens (sessão com cookie, JWT, provedor externo) para APLICACAO e recomende uma.~
Desenhe os fluxos: cadastro, login, recuperação de senha, logout e verificação de e-mail.~
Implemente o armazenamento seguro de senhas e a proteção contra força bruta.~
Implemente o modelo de permissões para PERFIS (RBAC) e o middleware de autorização.~
Configure cookies, CORS, CSRF e cabeçalhos de segurança corretamente.~
Implemente METODOS adicionais escolhidos.~
Escreva testes para tentativas de acesso indevido e escalonamento de privilégio.~
Entregue um checklist de segurança de autenticação para revisão antes de ir para produção.
```

### 9. Integração com API de terceiros e webhooks

**Objetivo:** conectar seu sistema a um serviço externo de forma resiliente.

```
SERVICO=[ex.: gateway de pagamento, CRM, ERP], OBJETIVO=[o que a integração deve fazer], DOCUMENTACAO=[trechos ou link da documentação], STACK=[tecnologias]
Resuma da DOCUMENTACAO os endpoints, a autenticação, os limites de requisição e os eventos de webhook relevantes para OBJETIVO.~
Desenhe o fluxo de dados entre seu sistema e SERVICO, incluindo cenários de falha.~
Implemente um cliente de API isolado com tratamento de erros, tentativas com espera progressiva e tempo limite.~
Implemente o recebimento de webhooks com validação de assinatura e idempotência.~
Defina como armazenar o estado da sincronização e reconciliar divergências.~
Proteja credenciais com variáveis de ambiente ou cofre de segredos.~
Escreva testes com simulação do serviço externo.~
Crie um guia de monitoramento e de resolução de falhas da integração.
```

### 10. Script de automação de tarefas repetitivas

**Objetivo:** automatizar uma tarefa manual com um script robusto e fácil de rodar.

```
TAREFA=[o que você faz manualmente], ENTRADAS=[arquivos, planilhas, pastas, APIs], SAIDA=[resultado esperado], LINGUAGEM=[Python, Node, Bash, PowerShell], FREQUENCIA=[com que frequência roda]
Descreva TAREFA como um passo a passo algorítmico e identifique pontos de decisão.~
Escolha as bibliotecas adequadas em LINGUAGEM e justifique.~
Escreva o script completo, com funções separadas, parâmetros configuráveis e registro de logs.~
Adicione tratamento de erros para ENTRADAS ausentes ou mal formatadas.~
Inclua modo de simulação (executa sem alterar nada) para testes seguros.~
Explique como agendar o script de acordo com FREQUENCIA no sistema operacional usado.~
Escreva instruções de instalação e uso para quem não é programador.~
Sugira melhorias futuras e como medir o tempo economizado.
```

### 11. Ferramenta de linha de comando (CLI)

**Objetivo:** criar uma CLI profissional, com comandos, ajuda e distribuição.

```
FERRAMENTA=[o que a CLI faz], COMANDOS=[comandos e opções desejados], LINGUAGEM=[linguagem], PUBLICO=[quem vai usar]
Projete a interface: comandos, subcomandos, argumentos, opções e valores padrão, seguindo convenções de CLI.~
Escreva a mensagem de ajuda de cada comando.~
Implemente a estrutura da CLI em LINGUAGEM com uma biblioteca adequada.~
Implemente cada comando com validação de entradas e mensagens de erro úteis.~
Adicione saída colorida, barra de progresso e modo silencioso onde fizer sentido.~
Implemente arquivo de configuração e variáveis de ambiente.~
Escreva testes dos comandos principais.~
Prepare o empacotamento e a publicação no gerenciador de pacotes, além de um README de uso para PUBLICO.
```

### 12. Migração de framework ou de versão

**Objetivo:** atualizar uma base de código com segurança, sem quebrar o que funciona.

```
PROJETO=[descrição do projeto], DE=[versão ou framework atual], PARA=[versão ou framework de destino], TAMANHO=[tamanho da base e da equipe], COBERTURA_TESTES=[situação atual dos testes]
Liste as mudanças incompatíveis entre DE e PARA que afetam PROJETO.~
Faça um inventário das áreas do código mais impactadas e estime o esforço.~
Avalie COBERTURA_TESTES e defina quais testes criar antes de migrar.~
Escolha a estratégia (migração total, incremental ou convivência temporária) e justifique para TAMANHO.~
Crie o plano em fases, com critérios de conclusão de cada fase.~
Mostre exemplos de antes e depois para os 5 padrões de código mais comuns a serem alterados.~
Defina o plano de reversão e de monitoramento após a publicação.~
Entregue um checklist de migração e o comunicado para a equipe.
```

## Debugging

### 13. Otimizar e explicar código
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** entender, corrigir e otimizar um trecho de código.

```
Analise o seguinte trecho de código: [insira o código]~Explique o funcionamento do código linha por linha~Identifique bugs e ineficiências~Sugira otimizações de desempenho e legibilidade~Forneça uma versão otimizada com comentários explicativos
```

### 14. Suporte técnico de TI
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** diagnosticar e resolver um problema técnico em linguagem simples.

```
Analise o seguinte problema técnico: [descreva o problema]~Identifique as causas potenciais~Sugira métodos de solução de problemas passo a passo~Forneça uma solução clara em termos simples~Recomende medidas preventivas para problemas futuros
```

### 15. Depuração a partir de mensagem de erro

**Objetivo:** encontrar a causa raiz de um erro a partir do stack trace e do código.

```
ERRO=[mensagem de erro e stack trace completos], CODIGO=[trechos relevantes], AMBIENTE=[linguagem, versões, sistema operacional], CONTEXTO=[o que você fez antes do erro e o que já tentou]
Explique em linguagem simples o que ERRO significa e em que linha ou camada ele se origina.~
Liste as 5 causas mais prováveis, em ordem de probabilidade, considerando CODIGO, AMBIENTE e CONTEXTO.~
Para cada causa, indique como confirmar ou descartar (o que imprimir, inspecionar ou testar).~
Com base na causa mais provável, proponha a correção com o código alterado.~
Explique por que a correção resolve a causa raiz, e não apenas o sintoma.~
Escreva um teste que teria detectado esse erro.~
Sugira mudanças para evitar erros semelhantes (validações, tipos, logs).~
Resuma o diagnóstico em um parágrafo para registrar no histórico do projeto.
```

### 16. Bug intermitente e condição de corrida

**Objetivo:** caçar bugs que aparecem só às vezes, típicos de concorrência e estado compartilhado.

```
SINTOMA=[comportamento observado], FREQUENCIA=[com que frequência ocorre], CODIGO=[trechos envolvidos], ARQUITETURA=[threads, async, filas, múltiplas instâncias]
Liste as categorias de bugs intermitentes (concorrência, cache, tempo, rede, dados, ambiente) e avalie quais combinam com SINTOMA e FREQUENCIA.~
Analise CODIGO buscando estado compartilhado, operações não atômicas, ordens de execução não garantidas e ausência de bloqueios.~
Descreva um cenário concreto, passo a passo, em que a condição de corrida aconteceria.~
Proponha como reproduzir o bug de forma confiável (testes de estresse, atrasos artificiais, logs com marcação de tempo).~
Apresente 2 soluções (ex.: bloqueio, transação, fila, idempotência) com seus custos.~
Implemente a solução recomendada.~
Escreva um teste que force a concorrência para validar a correção.~
Liste o que monitorar em produção para confirmar que o problema acabou.
```

### 17. Diagnóstico de lentidão e desempenho

**Objetivo:** descobrir o gargalo de uma aplicação lenta e acelerar com evidências.

```
APLICACAO=[tipo e stack], SINTOMA=[o que está lento e quanto tempo leva], DADOS=[logs, métricas, consultas ou código relevante], META=[tempo de resposta desejado]
Monte uma lista de hipóteses de gargalo por camada (front-end, rede, servidor, banco, serviços externos).~
Indique quais ferramentas e medições usar para confirmar cada hipótese.~
Analise DADOS e aponte os gargalos com maior evidência.~
Para cada gargalo, proponha a otimização (consulta, índice, cache, paginação, processamento assíncrono, compressão).~
Mostre o código ou a consulta otimizada.~
Estime o ganho de cada otimização e priorize pela relação esforço e impacto.~
Defina como medir antes e depois para comprovar a melhora em relação a META.~
Crie alertas de desempenho para evitar regressões.
```

### 18. Vazamento de memória

**Objetivo:** identificar o que está consumindo memória sem liberar e corrigir.

```
LINGUAGEM=[linguagem e runtime], SINTOMA=[crescimento de memória, travamentos, reinícios], CODIGO=[trechos suspeitos], PADRAO_DE_USO=[como e por quanto tempo o processo roda]
Explique como funciona o gerenciamento de memória em LINGUAGEM e as causas mais comuns de vazamento nela.~
Analise CODIGO buscando referências que não são liberadas (listeners, caches sem limite, closures, conexões abertas, variáveis globais).~
Indique as ferramentas de perfil de memória adequadas e o passo a passo para capturar e comparar snapshots.~
Descreva como reproduzir o vazamento com um teste de carga simulando PADRAO_DE_USO.~
Proponha e implemente as correções.~
Sugira limites e políticas (tamanho máximo de cache, tempo de expiração, pools).~
Explique como validar a correção acompanhando a memória ao longo do tempo.~
Liste boas práticas para a equipe evitar novos vazamentos.
```

### 19. Incidente em produção e post-mortem

**Objetivo:** conter, resolver e aprender com uma falha em produção.

```
INCIDENTE=[o que aconteceu e quando], IMPACTO=[usuários e funcionalidades afetados], DADOS=[logs, métricas, alterações recentes], EQUIPE=[quem está envolvido]
Classifique a gravidade do INCIDENTE e defina as ações imediatas de contenção (reverter, desligar funcionalidade, escalar recursos).~
Escreva a comunicação inicial para usuários e para a equipe interna.~
Analise DADOS e monte a linha do tempo do incidente.~
Aplique a técnica dos 5 porquês para chegar à causa raiz.~
Proponha a correção definitiva e as ações preventivas, com responsável e prazo.~
Identifique o que funcionou e o que falhou na detecção e na resposta.~
Escreva o documento de post-mortem sem culpados: resumo, impacto, linha do tempo, causa, ações e aprendizados.~
Escreva a comunicação final de encerramento do incidente.
```

### 20. Consulta SQL com erro ou resultado errado

**Objetivo:** corrigir uma consulta que falha ou devolve dados incorretos.

```
CONSULTA=[SQL atual], ESQUEMA=[tabelas e colunas envolvidas], RESULTADO_ESPERADO=[o que deveria retornar], RESULTADO_ATUAL=[o que retorna ou o erro], BANCO=[sistema de banco de dados]
Explique o que CONSULTA faz cláusula por cláusula.~
Compare RESULTADO_ATUAL e RESULTADO_ESPERADO e levante hipóteses (junção errada, duplicação, NULL, agrupamento, filtro, tipo de dado).~
Sugira consultas de diagnóstico menores para isolar o problema.~
Reescreva a consulta corrigida.~
Explique a correção e os casos de borda considerados.~
Analise o plano de execução esperado e sugira índices se necessário.~
Ofereça uma versão mais legível usando CTEs.~
Escreva 3 dados de teste que comprovem que a consulta está correta.
```

## Qualidade, testes e revisão

### 21. Revisão de código (code review)

**Objetivo:** revisar código como um engenheiro sênior, com feedback priorizado e acionável.

```
CODIGO=[código ou diff], CONTEXTO=[o que a alteração pretende fazer], PADROES=[padrões e convenções da equipe], LINGUAGEM=[linguagem]
Resuma o que o CODIGO faz e se ele cumpre o CONTEXTO.~
Aponte problemas de correção lógica e casos de borda não tratados.~
Aponte riscos de segurança (injeção, exposição de dados, validações ausentes).~
Avalie desempenho e uso de recursos.~
Avalie legibilidade, nomes, tamanho de funções e aderência a PADROES.~
Avalie testes: o que falta cobrir.~
Classifique cada comentário como bloqueante, importante ou sugestão, sempre com a linha e uma proposta de solução.~
Escreva os comentários em tom respeitoso e didático, e um resumo final com o veredito.
```

### 22. Testes unitários com boa cobertura

**Objetivo:** gerar uma suíte de testes que pega bugs de verdade, não só aumenta a porcentagem.

```
CODIGO=[função, classe ou módulo], LINGUAGEM=[linguagem], FRAMEWORK_TESTE=[ex.: Jest, Pytest, JUnit], DEPENDENCIAS=[dependências externas usadas]
Liste os comportamentos que CODIGO deve garantir.~
Liste os casos de teste: caminho feliz, entradas inválidas, limites, valores nulos, erros de DEPENDENCIAS.~
Defina o que simular (mocks) e o que testar de forma real.~
Escreva os testes em FRAMEWORK_TESTE com nomes descritivos e o padrão "preparar, agir, verificar".~
Adicione testes parametrizados para reduzir repetição.~
Aponte trechos de CODIGO difíceis de testar e sugira refatorações para melhorar a testabilidade.~
Estime a cobertura e indique o que ainda está descoberto.~
Explique como rodar os testes e integrá-los ao pipeline.
```

### 23. Testes de ponta a ponta (E2E)

**Objetivo:** automatizar os fluxos mais críticos do usuário no navegador.

```
APLICACAO=[descrição e URL de teste], FLUXOS=[fluxos críticos: cadastro, compra etc.], FERRAMENTA=[Playwright, Cypress, Selenium], DADOS_TESTE=[como criar dados de teste]
Priorize FLUXOS por risco de negócio e frequência de uso.~
Escreva os cenários em linguagem natural para cada fluxo, incluindo variações de erro.~
Defina a estratégia de seletores estáveis e a organização em page objects.~
Implemente os testes em FERRAMENTA.~
Implemente a preparação e a limpeza de DADOS_TESTE para testes independentes.~
Trate esperas e instabilidades sem usar pausas fixas.~
Configure a execução no pipeline com capturas de tela e vídeos em caso de falha.~
Crie um guia para a equipe manter e ampliar os testes.
```

### 24. Refatoração de código legado

**Objetivo:** melhorar código antigo sem mudar o comportamento.

```
CODIGO=[código legado], LINGUAGEM=[linguagem], PROBLEMAS=[o que incomoda: tamanho, duplicação, acoplamento], RESTRICOES=[o que não pode mudar]
Identifique os "maus cheiros" de código presentes em CODIGO, com a linha e o motivo.~
Escreva testes de caracterização que travem o comportamento atual antes de refatorar.~
Planeje a refatoração em passos pequenos e seguros, em ordem.~
Aplique os passos: extrair funções, renomear, remover duplicação, separar responsabilidades.~
Aplique padrões de projeto apenas onde simplificam, explicando o porquê.~
Mostre a versão final lado a lado com a original.~
Confirme que os testes de caracterização continuam passando e que RESTRICOES foram respeitadas.~
Liste melhorias que ficaram para uma próxima etapa.
```

### 25. Auditoria de segurança (OWASP)

**Objetivo:** encontrar vulnerabilidades comuns em uma aplicação web e corrigi-las.

```
APLICACAO=[descrição], CODIGO=[trechos críticos: autenticação, entradas, consultas, uploads], STACK=[tecnologias], DADOS_SENSIVEIS=[que dados pessoais ou financeiros são tratados]
Analise CODIGO contra cada item do OWASP Top 10, indicando se há risco, a evidência e a gravidade.~
Verifique validação de entrada, consultas parametrizadas, escape de saída e uploads.~
Verifique autenticação, gestão de sessões e controle de acesso.~
Verifique exposição de segredos, configurações padrão e dependências desatualizadas.~
Avalie o tratamento de DADOS_SENSIVEIS quanto a criptografia, retenção e conformidade com a LGPD.~
Para cada vulnerabilidade, proponha a correção com código.~
Priorize as correções por risco e esforço.~
Entregue um relatório de segurança e um checklist para novas funcionalidades.
```

### 26. Acessibilidade em interfaces web

**Objetivo:** tornar uma interface usável por pessoas com deficiência, seguindo as WCAG.

```
INTERFACE=[HTML, componente ou descrição da tela], PUBLICO=[usuários], NIVEL=[A, AA ou AAA]
Avalie INTERFACE em relação aos princípios das WCAG (perceptível, operável, compreensível, robusto) no NIVEL desejado.~
Verifique estrutura semântica, títulos, landmarks e ordem de leitura.~
Verifique a navegação por teclado, o foco visível e as armadilhas de foco.~
Verifique contraste de cores, tamanho de texto e dependência de cor para transmitir informação.~
Verifique textos alternativos, rótulos de formulário, mensagens de erro e atributos ARIA.~
Corrija o código com as melhorias.~
Liste testes manuais com leitor de tela e ferramentas automáticas.~
Entregue um checklist de acessibilidade para a equipe usar em toda nova tela.
```

### 27. Pipeline de CI/CD

**Objetivo:** automatizar testes, build e deploy a cada alteração de código.

```
PROJETO=[tipo e stack], REPOSITORIO=[GitHub, GitLab, Bitbucket], AMBIENTES=[desenvolvimento, homologação, produção], HOSPEDAGEM=[onde roda]
Desenhe o fluxo do pipeline: gatilhos, etapas, ambientes e aprovações.~
Escreva o arquivo de configuração do pipeline para REPOSITORIO com instalação, lint, testes e build.~
Adicione cache de dependências e execução paralela para acelerar.~
Configure o deploy automático para cada um dos AMBIENTES em HOSPEDAGEM.~
Configure o gerenciamento de segredos e variáveis por ambiente.~
Adicione verificações de segurança de dependências e de qualidade de código.~
Defina a estratégia de reversão rápida.~
Documente o pipeline e as regras de branch para a equipe.
```

### 28. Containerização com Docker

**Objetivo:** empacotar a aplicação em containers leves, seguros e reproduzíveis.

```
APLICACAO=[stack e serviços], SERVICOS_APOIO=[banco, cache, filas], AMBIENTE_ALVO=[local, servidor, nuvem, Kubernetes]
Escreva um Dockerfile multi-stage otimizado para APLICACAO, com imagem base enxuta e usuário sem privilégios.~
Explique cada instrução e as escolhas de cache de camadas.~
Escreva o arquivo .dockerignore.~
Escreva o docker-compose com APLICACAO e SERVICOS_APOIO, volumes, redes e variáveis de ambiente.~
Adicione verificações de saúde e políticas de reinício.~
Mostre como rodar migrações e seeds no ambiente de containers.~
Liste boas práticas de segurança e tamanho de imagem.~
Explique como levar a configuração para AMBIENTE_ALVO.
```

### 29. Otimização de banco de dados e índices

**Objetivo:** acelerar consultas lentas e reduzir carga do banco.

```
BANCO=[sistema e versão], CONSULTAS_LENTAS=[consultas e tempos], ESQUEMA=[tabelas e índices atuais], VOLUME=[quantidade de registros]
Analise cada consulta de CONSULTAS_LENTAS e explique por que está lenta.~
Interprete o plano de execução (EXPLAIN) esperado para cada uma.~
Proponha índices novos ou compostos, justificando a ordem das colunas.~
Reescreva as consultas para melhor desempenho.~
Identifique índices duplicados ou sem uso.~
Avalie se cabe particionamento, materialização ou cache, considerando VOLUME.~
Defina como medir antes e depois.~
Entregue o script de alterações e um plano para aplicá-lo sem indisponibilidade.
```

## Documentação

### 30. README profissional

**Objetivo:** criar um README que faz qualquer pessoa entender e rodar o projeto em minutos.

```
PROJETO=[nome e descrição], STACK=[tecnologias], ESTRUTURA=[estrutura de pastas], COMANDOS=[comandos para instalar, rodar e testar], PUBLICO=[usuários, contribuidores ou ambos]
Escreva o título, a descrição em uma frase e os selos recomendados.~
Escreva a seção "Por que este projeto existe" e as principais funcionalidades.~
Escreva os pré-requisitos e o passo a passo de instalação a partir de COMANDOS.~
Escreva exemplos de uso com trechos de código e saídas esperadas.~
Documente as variáveis de ambiente e a configuração.~
Explique ESTRUTURA de forma resumida.~
Escreva as seções de testes, deploy, contribuição, licença e contato.~
Revise para clareza e entregue o README completo em Markdown.
```

### 31. Documentação de API (OpenAPI)

**Objetivo:** documentar uma API de forma completa, com exemplos e especificação técnica.

```
API=[descrição], ENDPOINTS=[rotas e código ou descrições], AUTENTICACAO=[como autenticar], CONSUMIDORES=[desenvolvedores internos ou externos]
Escreva a introdução da API: propósito, URL base, versionamento e limites de uso.~
Documente AUTENTICACAO com exemplo passo a passo.~
Para cada endpoint, documente descrição, parâmetros, corpo, respostas e erros, com exemplos em JSON.~
Escreva exemplos de chamada em cURL, JavaScript e Python.~
Documente o padrão de erros e os códigos de status.~
Escreva um guia de início rápido para CONSUMIDORES fazerem a primeira chamada em 5 minutos.~
Gere a especificação OpenAPI 3 em YAML.~
Revise consistência entre a especificação e os exemplos.
```

### 32. Registro de decisão de arquitetura (ADR)

**Objetivo:** documentar uma decisão técnica com contexto e alternativas para o futuro.

```
DECISAO=[o que está sendo decidido], CONTEXTO=[situação, restrições e motivação], OPCOES=[alternativas consideradas]
Reescreva CONTEXTO de forma objetiva, incluindo forças em jogo e restrições.~
Para cada uma das OPCOES, descreva prós, contras, riscos e custo.~
Monte uma matriz de decisão com critérios ponderados.~
Registre a decisão e a justificativa.~
Liste as consequências positivas, negativas e neutras.~
Defina em que condições a decisão deve ser revista.~
Formate tudo no modelo ADR (título, status, contexto, decisão, consequências).~
Escreva um resumo de 3 linhas para o canal da equipe.
```

### 33. Comentários e docstrings

**Objetivo:** documentar o código de forma útil, sem comentários óbvios.

```
CODIGO=[código], LINGUAGEM=[linguagem], PADRAO=[ex.: JSDoc, Google docstrings, Javadoc]
Identifique as partes de CODIGO que precisam de documentação (API pública, lógica não óbvia, decisões de negócio).~
Escreva docstrings no PADRAO para funções, classes e módulos, com parâmetros, retorno, exceções e exemplos.~
Adicione comentários apenas onde explicam o "porquê", não o "o quê".~
Remova ou reescreva comentários redundantes ou desatualizados.~
Sugira renomeações que dispensem comentários.~
Entregue o código documentado completo.~
Mostre como gerar a documentação automaticamente a partir das docstrings.
```

### 34. Guia de onboarding para novos desenvolvedores

**Objetivo:** fazer um novo dev contribuir em dias, não semanas.

```
PROJETO=[descrição do sistema], STACK=[tecnologias], PROCESSOS=[fluxo de trabalho da equipe: branches, revisão, deploy], CONTATOS=[quem procurar para quê]
Escreva a visão geral do produto e do negócio em linguagem simples.~
Explique a arquitetura com um diagrama e a função de cada parte.~
Escreva o passo a passo para preparar o ambiente local, com problemas comuns e soluções.~
Documente PROCESSOS e as convenções de código.~
Crie um glossário de termos do domínio e siglas internas.~
Monte o plano dos primeiros 10 dias com tarefas progressivas.~
Liste "primeiras tarefas" boas para um iniciante no projeto.~
Organize CONTATOS e canais de comunicação e entregue o guia completo.
```

### 35. Notas de versão e changelog

**Objetivo:** transformar commits em notas de versão claras para usuários e para a equipe.

```
COMMITS=[lista de commits ou PRs], VERSAO=[número da versão], PUBLICO=[usuários finais, clientes ou desenvolvedores]
Agrupe COMMITS em categorias: novidades, melhorias, correções, mudanças incompatíveis e segurança.~
Reescreva cada item em linguagem de benefício para PUBLICO.~
Destaque mudanças incompatíveis com instruções de migração.~
Defina VERSAO seguindo versionamento semântico e justifique.~
Escreva o changelog técnico em formato padronizado.~
Escreva a nota de versão para usuários, curta e amigável.~
Escreva um anúncio para e-mail ou redes sociais destacando as 3 maiores novidades.
```

### 36. Diagramas de sistema em Mermaid

**Objetivo:** gerar diagramas versionáveis a partir da descrição ou do código.

```
SISTEMA=[descrição ou código], TIPOS=[arquitetura, sequência, entidade-relacionamento, fluxo, estados], PUBLICO=[técnico ou não técnico]
Identifique os componentes, atores e fluxos principais de SISTEMA.~
Gere um diagrama de arquitetura de alto nível em Mermaid.~
Gere diagramas de sequência para os 2 fluxos mais importantes.~
Gere o diagrama entidade-relacionamento, se houver dados.~
Gere um diagrama de estados para a entidade com ciclo de vida mais complexo.~
Escreva uma legenda e uma explicação curta para cada diagrama, adequada a PUBLICO.~
Revise os diagramas buscando inconsistências com SISTEMA.
```

## Aprendizado e produtividade do desenvolvedor

### 37. Aprender uma nova linguagem construindo um projeto

**Objetivo:** aprender na prática, com um projeto guiado em etapas.

```
LINGUAGEM=[linguagem a aprender], EXPERIENCIA=[linguagens que você já domina], TEMPO=[horas por semana], OBJETIVO=[ex.: back-end, dados, mobile]
Compare LINGUAGEM com EXPERIENCIA, destacando semelhanças, diferenças e armadilhas para quem vem dessas linguagens.~
Proponha 3 projetos alinhados a OBJETIVO e escolha o mais didático.~
Divida o projeto em 8 etapas, cada uma introduzindo novos conceitos da linguagem.~
Para a etapa 1, explique os conceitos, mostre o código e proponha um exercício.~
Repita para as etapas seguintes conforme eu avançar.~
Em cada etapa, aponte o jeito idiomático de escrever em LINGUAGEM.~
Monte um cronograma realista de acordo com TEMPO.~
Liste recursos oficiais e projetos open source para continuar evoluindo.
```

### 38. Explicar um conceito de programação em camadas

**Objetivo:** entender um conceito do básico ao avançado, com analogias e código.

```
CONCEITO=[ex.: closures, recursão, injeção de dependência, async/await], NIVEL=[iniciante, intermediário, avançado], LINGUAGEM=[linguagem dos exemplos]
Explique CONCEITO em uma frase simples e com uma analogia do dia a dia.~
Explique o problema que CONCEITO resolve e o que acontecia antes dele.~
Mostre um exemplo mínimo em LINGUAGEM, comentado linha por linha.~
Mostre um exemplo realista de uso em um projeto.~
Liste os erros mais comuns e equívocos sobre CONCEITO.~
Aprofunde para NIVEL avançado: funcionamento interno e quando não usar.~
Proponha 3 exercícios de dificuldade crescente com gabarito.~
Faça 5 perguntas para eu testar meu entendimento.
```

### 39. Resolver desafio de algoritmo passo a passo

**Objetivo:** treinar raciocínio algorítmico, da força bruta à solução ótima.

```
PROBLEMA=[enunciado], LINGUAGEM=[linguagem], RESTRICOES=[limites de entrada e tempo]
Reescreva PROBLEMA com suas palavras e liste entradas, saídas e casos de borda.~
Resolva 2 exemplos à mão.~
Proponha a solução de força bruta e sua complexidade.~
Identifique o padrão que permite otimizar (dois ponteiros, janela deslizante, hash, programação dinâmica, grafos, etc.).~
Implemente a solução otimizada em LINGUAGEM, comentada.~
Analise a complexidade de tempo e espaço e confirme que atende RESTRICOES.~
Escreva testes cobrindo os casos de borda.~
Sugira 3 problemas parecidos para fixar o padrão.
```

### 40. Converter código entre linguagens

**Objetivo:** traduzir código mantendo o comportamento e adotando o estilo idiomático do destino.

```
CODIGO=[código original], ORIGEM=[linguagem de origem], DESTINO=[linguagem de destino], CONTEXTO=[onde o código vai rodar]
Explique o que CODIGO faz e liste as dependências e recursos específicos de ORIGEM.~
Mapeie os equivalentes em DESTINO (bibliotecas, tipos, tratamento de erros, concorrência).~
Traduza o código para DESTINO de forma idiomática, não literal.~
Aponte diferenças de comportamento (números, strings, datas, nulos) e como foram tratadas.~
Escreva testes que comprovem que as duas versões se comportam igual.~
Explique como configurar o projeto em DESTINO para CONTEXTO.~
Liste melhorias que DESTINO permite e que não existiam em ORIGEM.
```

### 41. Criar e explicar expressões regulares

**Objetivo:** gerar regex corretas, testadas e explicadas.

```
NECESSIDADE=[o que precisa ser encontrado, validado ou substituído], EXEMPLOS_VALIDOS=[exemplos que devem casar], EXEMPLOS_INVALIDOS=[exemplos que não devem casar], LINGUAGEM=[onde a regex será usada]
Analise os exemplos e descreva o padrão em palavras.~
Escreva a expressão regular compatível com LINGUAGEM.~
Explique cada parte da expressão em uma tabela.~
Teste mentalmente contra EXEMPLOS_VALIDOS e EXEMPLOS_INVALIDOS e mostre o resultado de cada um.~
Liste casos de borda que podem falhar e ajuste a expressão.~
Avalie riscos de desempenho (retrocesso catastrófico).~
Mostre o código de uso em LINGUAGEM e uma alternativa sem regex, se for mais simples.
```

### 42. Estimativa e quebra de tarefas técnicas

**Objetivo:** transformar um pedido vago em tarefas estimadas e planejadas.

```
DEMANDA=[descrição do que foi pedido], CONTEXTO_TECNICO=[sistema atual e equipe], PRAZO_DESEJADO=[prazo pedido]
Liste as dúvidas e premissas que precisam ser esclarecidas sobre DEMANDA.~
Quebre DEMANDA em épicos, histórias e tarefas técnicas.~
Estime cada tarefa em três cenários (otimista, provável, pessimista) e calcule a estimativa ponderada.~
Identifique dependências e o caminho crítico.~
Liste riscos que podem aumentar o prazo.~
Compare a estimativa com PRAZO_DESEJADO e proponha opções (reduzir escopo, adicionar pessoas, fasear).~
Escreva a resposta para o solicitante explicando prazo, premissas e trade-offs.
```
