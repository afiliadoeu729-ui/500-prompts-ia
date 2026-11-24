# Vendas e negociação

> Prospecção, atendimento, qualificação, objeções, negociação, fechamento e gestão comercial.

**40 prompts** nesta categoria — 3 do repositório original PromptChains (marcados com 🔁) e 37 novos.

**Como usar:** copie o bloco inteiro de um prompt, substitua os campos entre colchetes `[...]` pelas suas informações e cole no ChatGPT, Claude, Gemini ou em uma extensão de fila de prompts (como o ChatGPT Queue). Cada trecho separado por `~` é uma etapa: em uma extensão de fila, as etapas são enviadas uma a uma automaticamente; sem extensão, envie uma etapa por vez, na ordem.

[← Voltar ao índice geral](README.md)

## Índice

**[Prospecção](#prospecção)**

1. [Enriquecer leads para o CRM](#1-enriquecer-leads-para-o-crm) 🔁
2. [Lista de prospecção a partir do perfil de cliente ideal](#2-lista-de-prospecção-a-partir-do-perfil-de-cliente-ideal)
3. [Cadência de prospecção multicanal](#3-cadência-de-prospecção-multicanal)
4. [Cold e-mail que gera resposta](#4-cold-e-mail-que-gera-resposta)
5. [Roteiro de ligação fria](#5-roteiro-de-ligação-fria)
6. [Social selling no LinkedIn](#6-social-selling-no-linkedin)
7. [Prospecção pelo WhatsApp com consentimento](#7-prospecção-pelo-whatsapp-com-consentimento)
8. [Prospecção de empresas locais](#8-prospecção-de-empresas-locais)
9. [Reativação de clientes inativos](#9-reativação-de-clientes-inativos)

**[Atendimento e qualificação](#atendimento-e-qualificação)**

10. [Qualificação de leads com BANT e SPIN](#10-qualificação-de-leads-com-bant-e-spin)
11. [Reunião de descoberta](#11-reunião-de-descoberta)
12. [Demonstração de produto](#12-demonstração-de-produto)
13. [Atendimento consultivo em loja ou balcão](#13-atendimento-consultivo-em-loja-ou-balcão)
14. [Pós-venda e onboarding do cliente](#14-pós-venda-e-onboarding-do-cliente)
15. [Gestão de contas-chave](#15-gestão-de-contas-chave)
16. [Upsell e cross-sell para clientes atuais](#16-upsell-e-cross-sell-para-clientes-atuais)

**[Objeções](#objeções)**

17. [Banco de respostas a objeções](#17-banco-de-respostas-a-objeções)
18. [Objeção "está caro"](#18-objeção-está-caro)
19. [Objeção "vou pensar"](#19-objeção-vou-pensar)
20. [Objeção "já tenho fornecedor"](#20-objeção-já-tenho-fornecedor)
21. [Simulação de objeções (role-play)](#21-simulação-de-objeções-role-play)

**[Negociação e fechamento](#negociação-e-fechamento)**

22. [Propostas eficazes para freelancers (Upwork, Fiverr, Workana etc.)](#22-propostas-eficazes-para-freelancers-upwork-fiverr-workana-etc) 🔁
23. [Estratégia de vendas](#23-estratégia-de-vendas) 🔁
24. [Proposta comercial B2B com retorno sobre investimento](#24-proposta-comercial-b2b-com-retorno-sobre-investimento)
25. [Técnicas de fechamento](#25-técnicas-de-fechamento)
26. [Preparação para uma negociação](#26-preparação-para-uma-negociação)
27. [Negociação com fornecedores](#27-negociação-com-fornecedores)
28. [Acompanhamento de proposta sem resposta](#28-acompanhamento-de-proposta-sem-resposta)

**[Gestão comercial](#gestão-comercial)**

29. [Playbook de vendas](#29-playbook-de-vendas)
30. [Metas e plano de comissionamento](#30-metas-e-plano-de-comissionamento)
31. [Revisão do funil e previsão de vendas](#31-revisão-do-funil-e-previsão-de-vendas)
32. [Treinamento de vendedores](#32-treinamento-de-vendedores)
33. [Organização do CRM e do funil](#33-organização-do-crm-e-do-funil)
34. [Análise de ganhos e perdas](#34-análise-de-ganhos-e-perdas)

**[Vendas por canal](#vendas-por-canal)**

35. [Vendas pelo Instagram](#35-vendas-pelo-instagram)
36. [Vendas em marketplaces](#36-vendas-em-marketplaces)
37. [Venda de alto valor em chamada (closer)](#37-venda-de-alto-valor-em-chamada-closer)
38. [Venda complexa com vários decisores](#38-venda-complexa-com-vários-decisores)
39. [Programa de revendedores e parceiros](#39-programa-de-revendedores-e-parceiros)
40. [Vendas em feiras e eventos](#40-vendas-em-feiras-e-eventos)

---


## Prospecção

### 1. Enriquecer leads para o CRM
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** pesquisar, um a um, informações públicas e profissionais de uma lista de contatos B2B, respeitando a LGPD.

```
Tarefa de enriquecimento de leads
Bem-vindo à tarefa de enriquecimento de leads! Seu objetivo é enriquecer uma lista de endereços de e-mail reunindo informações detalhadas e relevantes sobre cada um. Esse processo é essencial para construir uma compreensão completa de cada lead, o que pode melhorar significativamente as estratégias de engajamento e segmentação. Veja o passo a passo:

Instruções passo a passo:
Lista de e-mails:

Vou fornecer uma lista completa de endereços de e-mail. Essa lista é seu ponto de partida e contém os leads que precisam ser enriquecidos.
Processamento sequencial:

Comece pelo primeiro endereço de e-mail da lista. Quando eu disser "próximo", passe para o endereço seguinte. Esse método garante uma abordagem estruturada e organizada, permitindo uma coleta de dados sistemática.
Coleta de informações:

Para cada endereço de e-mail, sua tarefa é buscar e compilar as seguintes informações relevantes. Esses dados ajudarão a montar um retrato completo de cada lead:
Nome: Identifique a pessoa ou organização associada ao e-mail. Isso costuma ser encontrado em redes profissionais ou diretórios de empresas.
Cargo ou função: Determine o cargo ou função atual da pessoa. O LinkedIn é um recurso valioso para essa informação.
Perfis em redes sociais: Localize perfis profissionais em plataformas como LinkedIn, X ou Facebook. Esses perfis podem revelar interesses e atividades profissionais.
Informações da empresa: Reúna detalhes sobre a empresa associada, como setor, porte e pessoas-chave.
Informações de contato publicamente disponíveis: Podem incluir telefones comerciais, e-mails secundários ou endereços comerciais. Garanta que esses dados sejam publicamente acessíveis, em conformidade com as normas de privacidade.
Notícias ou artigos recentes: Procure notícias, artigos ou comunicados recentes envolvendo a pessoa ou sua organização. Esse contexto é valioso para entender o foco e as conquistas atuais.
Fontes de dados:
Fontes confiáveis: Priorize informações de fontes confiáveis e oficiais para garantir a precisão. LinkedIn, sites oficiais de empresas, Google e redes profissionais são ótimos pontos de partida.
Mecanismos de busca: Use os mecanismos de busca de forma eficaz, com consultas específicas que ajudem a encontrar as informações necessárias.
Conformidade:
Normas legais e de privacidade: Garanta que toda a coleta de informações esteja em conformidade com as normas legais e de privacidade aplicáveis, como a LGPD, o GDPR e a CCPA. Use apenas dados profissionais e públicos, com finalidade comercial legítima, e evite métodos que possam violar direitos de privacidade ou envolver coleta não autorizada de dados.
Tratamento de ambiguidades:
Múltiplos resultados: Se houver vários resultados para um e-mail, use pistas de contexto, como a empresa ou o cargo, para escolher o mais relevante.
Nenhuma informação encontrada: Se nenhuma informação relevante for encontrada após uma busca completa, registre a busca como malsucedida e passe para o próximo e-mail. Documentar isso ajuda a manter um registro das tentativas e resultados.
Formato de saída:
Apresentação estruturada: Apresente as informações reunidas em um formato estruturado, como uma tabela ou um arquivo JSON. O formato deve incluir campos claramente identificados para cada dado, facilitando a revisão e o uso.
Tratamento de erros:
Buscas malsucedidas: Registre todos os casos em que a busca não teve sucesso ou ficou incompleta. Esse registro ajuda a revisar o processo e identificar melhorias.
Limites de requisição e considerações éticas:
Evite consultas excessivas: Respeite os termos de serviço dos provedores de dados. Consultas excessivas podem levar a restrições ou bloqueios, por isso é essencial respeitar esses limites.
Diretrizes éticas: Siga diretrizes éticas na coleta de dados, garantindo que todas as informações sejam obtidas de forma responsável e respeitosa.
Vamos começar esta jornada de enriquecimento. Comece examinando o primeiro endereço de e-mail e, quando estiver pronto para avançar, basta eu dizer "próximo". Sua abordagem cuidadosa e diligente aumentará muito o valor desses leads, criando uma base sólida para o engajamento e as ações estratégicas.

[Lista de e-mails]

~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~próximo~
```

### 2. Lista de prospecção a partir do perfil de cliente ideal

**Objetivo:** definir quem abordar e montar uma lista qualificada.

```
SOLUCAO=[o que você vende], MELHORES_CLIENTES=[características dos clientes atuais mais lucrativos], REGIAO=[área de atuação], FONTES=[LinkedIn, Google Maps, associações, eventos, bases públicas]
Analise MELHORES_CLIENTES e defina o perfil de cliente ideal: setor, porte, região, momento e sinais de compra.~
Defina as personas de decisão e de influência dentro dessas empresas.~
Liste gatilhos que indicam boa hora para abordar (contratações, expansão, troca de gestão, notícias).~
Explique como buscar empresas e contatos em FONTES, respeitando a LGPD e os termos de uso.~
Crie os critérios de pontuação de cada conta (A, B, C).~
Monte o modelo de planilha da lista com os campos necessários.~
Defina a meta semanal de contas pesquisadas e abordadas.
```

### 3. Cadência de prospecção multicanal

**Objetivo:** organizar uma sequência de contatos por e-mail, telefone e LinkedIn.

```
PERSONA=[cargo e setor], SOLUCAO=[o que vende], DOR_PRINCIPAL=[problema que resolve], PROVA=[caso ou resultado real], DURACAO=[dias da cadência]
Desenhe a cadência de 8 a 12 toques ao longo de DURACAO, alternando canais.~
Escreva cada e-mail (assunto e corpo com até 100 palavras), cada um com um ângulo diferente.~
Escreva o roteiro das ligações e a mensagem de caixa postal.~
Escreva os convites e as mensagens do LinkedIn.~
Escreva a mensagem de encerramento da cadência ("último contato").~
Defina as regras de saída (respondeu, recusou, pediu para não contatar) e os indicadores da cadência.
```

### 4. Cold e-mail que gera resposta

**Objetivo:** escrever e-mails frios curtos, relevantes e sem cara de spam.

```
DESTINATARIO=[cargo e empresa], GANCHO=[motivo específico para contatar agora], SOLUCAO=[o que oferece], PROVA=[resultado real], CTA=[pedido simples]
Escreva 10 assuntos curtos e não promocionais.~
Escreva 3 versões de e-mail com até 90 palavras: pergunta, observação personalizada e caso de cliente.~
Personalize a primeira linha a partir de GANCHO.~
Termine com um CTA de baixo compromisso.~
Escreva 2 follow-ups.~
Liste as boas práticas de entregabilidade e de conformidade com a LGPD (base legal, opção de descadastro).
```

### 5. Roteiro de ligação fria

**Objetivo:** abordar por telefone com confiança e marcar reuniões.

```
PERSONA=[cargo], SOLUCAO=[o que vende], DOR=[problema], OBJETIVO_DA_LIGACAO=[marcar reunião, qualificar, apresentar]
Escreva a abertura dos primeiros 15 segundos com permissão para continuar.~
Escreva a declaração de motivo da ligação focada em DOR.~
Escreva 4 perguntas de qualificação.~
Escreva respostas para as 6 objeções mais comuns ao telefone.~
Escreva o fechamento para OBJETIVO_DA_LIGACAO com proposta de data.~
Escreva o roteiro para passar pela secretária ou recepção.~
Crie a simulação: faça o papel do cliente e aguarde minhas respostas.
```

### 6. Social selling no LinkedIn

**Objetivo:** gerar oportunidades pelo LinkedIn com relacionamento e conteúdo.

```
SOLUCAO=[o que vende], PERSONA=[cargo-alvo], SETOR=[setor], TEMPO=[minutos por dia]
Otimize o perfil do vendedor para ser útil a PERSONA, e não um currículo.~
Defina a rotina diária em TEMPO: conexões, comentários, conteúdo e mensagens.~
Escreva 5 convites de conexão personalizados.~
Escreva a sequência de mensagens após a conexão (valor, conversa, convite).~
Crie 10 ideias de posts que atraem PERSONA.~
Defina os indicadores (aceites, respostas, reuniões).
```

### 7. Prospecção pelo WhatsApp com consentimento

**Objetivo:** usar o WhatsApp para vender sem ser invasivo e respeitando as regras.

```
NEGOCIO=[tipo], ORIGEM_DOS_CONTATOS=[como os contatos chegaram: formulário, indicação, evento], OFERTA=[o que oferece]
Explique os cuidados de consentimento e privacidade para contatar pelo WhatsApp de acordo com ORIGEM_DOS_CONTATOS.~
Escreva a primeira mensagem curta e personalizada.~
Escreva a sequência de 3 mensagens com valor antes da oferta.~
Escreva a mensagem de oferta.~
Escreva respostas para "quem te passou meu número?" e "não tenho interesse".~
Defina o uso de etiquetas e de horários adequados.
```

### 8. Prospecção de empresas locais

**Objetivo:** conquistar clientes comerciais da sua cidade.

```
SERVICO=[o que oferece], CIDADE=[cidade e bairros], SEGMENTOS=[tipos de negócio-alvo], DIFERENCIAL=[seu diferencial]
Liste como mapear empresas de SEGMENTOS em CIDADE (mapas, associações comerciais, feiras).~
Defina os critérios de priorização.~
Escreva o roteiro de visita presencial.~
Escreva a mensagem de contato inicial por telefone e WhatsApp.~
Crie um material de apoio de 1 página.~
Defina a meta semanal e o controle de visitas.
```

### 9. Reativação de clientes inativos

**Objetivo:** trazer de volta clientes que pararam de comprar.

```
CLIENTES_INATIVOS=[perfil e tempo sem comprar], HISTORICO=[o que compravam], MOTIVOS_PROVAVEIS=[motivos de saída], OFERTA=[condição de retorno]
Segmente CLIENTES_INATIVOS por tempo sem compra e valor histórico.~
Escreva mensagens de reativação para cada segmento, sem oferta no primeiro contato.~
Escreva a pesquisa rápida para entender o motivo da saída.~
Escreva a mensagem com OFERTA para quem não respondeu.~
Defina canais e intervalos.~
Defina como medir a taxa de reativação.
```

## Atendimento e qualificação

### 10. Qualificação de leads com BANT e SPIN

**Objetivo:** descobrir rapidamente se um lead tem potencial e entender sua real necessidade.

```
SOLUCAO=[o que vende], TICKET=[valor médio], PERFIL_DE_LEAD=[quem chega], CICLO=[ciclo de venda]
Explique os critérios BANT (orçamento, autoridade, necessidade, prazo) aplicados a SOLUCAO.~
Escreva perguntas naturais para descobrir cada critério sem interrogar.~
Escreva perguntas SPIN (situação, problema, implicação, necessidade de solução) para PERFIL_DE_LEAD.~
Crie a pontuação de qualificação e o que fazer em cada faixa.~
Escreva como desqualificar com educação.~
Monte o formulário de registro no CRM.
```

### 11. Reunião de descoberta

**Objetivo:** conduzir a primeira reunião para entender o cliente e avançar a venda.

```
CLIENTE=[empresa e participantes], CONTEXTO=[o que já se sabe], SOLUCAO=[o que vende], DURACAO=[minutos]
Pesquise e resuma o que é útil saber sobre CLIENTE antes da reunião.~
Escreva a agenda e a abertura (objetivo, tempo, combinado final).~
Escreva 15 perguntas de descoberta em ordem lógica.~
Defina como resumir o que foi entendido e confirmar as dores.~
Escreva o fechamento com próximo passo concreto e data.~
Crie o modelo de anotação da reunião.~
Escreva o e-mail de resumo pós-reunião.
```

### 12. Demonstração de produto

**Objetivo:** mostrar o produto conectando funcionalidades às dores do cliente.

```
PRODUTO=[produto], CLIENTE=[perfil e dores descobertas], DECISORES=[quem assiste], DURACAO=[minutos]
Selecione as 3 funcionalidades que resolvem as dores de CLIENTE.~
Estruture a demo em história: situação atual, como fica com PRODUTO e resultado.~
Escreva o roteiro com falas e telas.~
Prepare momentos de interação e perguntas de verificação.~
Prepare respostas para perguntas técnicas prováveis.~
Escreva o fechamento com próximos passos.~
Liste o que evitar em demos.
```

### 13. Atendimento consultivo em loja ou balcão

**Objetivo:** atender clientes presenciais entendendo a necessidade e aumentando a conversão.

```
LOJA=[tipo de loja e produtos], PERFIS_DE_CLIENTE=[quem entra na loja], TICKET_MEDIO=[valor]
Escreva a abordagem inicial sem pressão.~
Escreva perguntas para entender necessidade, uso e orçamento.~
Mostre como apresentar no máximo 3 opções.~
Escreva sugestões de complemento que façam sentido.~
Escreva respostas para "só estou olhando" e "vou dar uma volta".~
Escreva o fechamento e o pós-venda (cadastro, contato, avaliação).
```

### 14. Pós-venda e onboarding do cliente

**Objetivo:** garantir que o cliente tenha sucesso logo no início e continue comprando.

```
PRODUTO=[produto ou serviço], CLIENTE=[perfil], PRIMEIRO_RESULTADO=[o que o cliente precisa alcançar primeiro], PRAZO=[dias]
Desenhe a jornada de onboarding até PRIMEIRO_RESULTADO.~
Escreva a mensagem de boas-vindas e os próximos passos.~
Crie o roteiro da reunião de início.~
Defina os pontos de contato nas primeiras semanas.~
Defina os sinais de risco e como agir.~
Escreva o pedido de avaliação e de indicação após o primeiro resultado.
```

### 15. Gestão de contas-chave

**Objetivo:** cuidar e fazer crescer os clientes mais importantes.

```
CONTA=[cliente], RECEITA_ATUAL=[valor], CONTATOS=[pessoas e papéis], OPORTUNIDADES=[áreas ainda não atendidas], RISCOS=[ameaças]
Monte o mapa de relacionamento com CONTATOS (influência, posição e relação).~
Analise a saúde da conta e RISCOS.~
Defina os objetivos do cliente para o ano.~
Liste OPORTUNIDADES de expansão com valor estimado.~
Monte o plano de conta com ações trimestrais.~
Prepare a pauta da revisão executiva com o cliente.
```

### 16. Upsell e cross-sell para clientes atuais

**Objetivo:** aumentar a receita de quem já compra, oferecendo o que realmente ajuda.

```
CLIENTES=[perfil e o que compram], CATALOGO=[outros produtos ou planos], SINAIS=[comportamentos que indicam necessidade]
Mapeie a próxima compra lógica para cada perfil de CLIENTES.~
Defina gatilhos de oferta a partir de SINAIS.~
Escreva as mensagens de oferta para cada gatilho.~
Escreva o roteiro de conversa de expansão.~
Defina condições especiais para clientes atuais.~
Defina as metas e indicadores de expansão.
```

## Objeções

### 17. Banco de respostas a objeções

**Objetivo:** ter respostas prontas e empáticas para as objeções mais comuns.

```
PRODUTO=[produto], PRECO=[preço], PUBLICO=[cliente], OBJECOES=[objeções que você ouve]
Complete OBJECOES com as objeções típicas do mercado (preço, tempo, confiança, necessidade, concorrente, autoridade).~
Para cada objeção, identifique a preocupação real por trás.~
Escreva a resposta usando o método ouvir, validar, perguntar e responder.~
Escreva uma pergunta que transforme a objeção em conversa.~
Indique a prova que ajuda em cada caso.~
Organize tudo em uma tabela para consulta rápida.
```

### 18. Objeção "está caro"

**Objetivo:** defender o valor sem baixar o preço de imediato.

```
PRODUTO=[produto], PRECO=[preço], CONCORRENTES=[preços concorrentes], VALOR=[resultados que entrega], MARGEM_DE_NEGOCIACAO=[o que pode ceder]
Liste os 5 significados possíveis de "está caro" e a pergunta para descobrir qual é.~
Escreva respostas que reforcem VALOR (retorno, custo de não resolver, custo por dia).~
Escreva a comparação justa com CONCORRENTES.~
Escreva alternativas antes do desconto (parcelamento, versão menor, escopo).~
Defina quando e como usar MARGEM_DE_NEGOCIACAO, sempre com contrapartida.~
Simule a conversa comigo.
```

### 19. Objeção "vou pensar"

**Objetivo:** descobrir o que está por trás do "vou pensar" e ajudar o cliente a decidir.

```
CONTEXTO_DA_VENDA=[o que foi apresentado], CLIENTE=[perfil], PRAZO_REAL=[existe urgência real?]
Explique as razões mais comuns por trás de "vou pensar".~
Escreva 5 perguntas respeitosas para descobrir a dúvida real.~
Escreva respostas para cada dúvida provável.~
Escreva como combinar um próximo passo concreto se o cliente realmente precisar de tempo.~
Escreva a mensagem de acompanhamento.~
Liste o que não fazer (pressão excessiva, urgência falsa).
```

### 20. Objeção "já tenho fornecedor"

**Objetivo:** abrir espaço com quem já está satisfeito com outra empresa.

```
SOLUCAO=[o que vende], DIFERENCIAIS=[diferenciais reais], CONCORRENTE_PROVAVEL=[fornecedor atual típico]
Escreva respostas que respeitem a escolha atual e despertem curiosidade.~
Escreva perguntas para descobrir pontos de insatisfação.~
Proponha uma comparação ou teste de baixo risco.~
Mostre como se posicionar como segunda opção.~
Defina o acompanhamento de longo prazo para quando o cenário mudar.
```

### 21. Simulação de objeções (role-play)

**Objetivo:** treinar respostas a objeções em uma simulação realista.

```
PRODUTO=[produto], PERFIL_DO_CLIENTE=[tipo de cliente e personalidade], DIFICULDADE=[fácil, médio, difícil]
Assuma o papel de PERFIL_DO_CLIENTE em nível de DIFICULDADE.~
Inicie a conversa com uma objeção e aguarde minha resposta.~
Reaja de forma realista às minhas respostas, trazendo novas objeções.~
Depois de 6 trocas, saia do personagem e avalie meu desempenho.~
Aponte as melhores e as piores respostas e sugira melhorias.~
Proponha uma nova rodada mais difícil.
```

## Negociação e fechamento

### 22. Propostas eficazes para freelancers (Upwork, Fiverr, Workana etc.)
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** escrever propostas personalizadas para vagas de freela, com valor, prazo e chamada para ação.

```
DESCRICAO_DO_PROJETO=[cole o anúncio do projeto], VALOR_DA_PROPOSTA=[seu preço], EXPERIENCIA_RELEVANTE=[suas habilidades e projetos compatíveis], PRAZO=[prazo de entrega]~Analise DESCRICAO_DO_PROJETO e identifique: 1) Requisitos-chave 2) Dores do cliente 3) Escopo do projeto 4) Sinais de alerta ou pontos que precisam de esclarecimento~Gere um primeiro parágrafo atraente que: 1) Mencione um detalhe específico do anúncio 2) Demonstre compreensão imediata das necessidades 3) Estabeleça especialidade relevante a partir de EXPERIENCIA_RELEVANTE~Crie a seção do meio abordando: 1) Sua abordagem específica para o projeto 2) Exemplos de trabalhos semelhantes 3) Por que você é a pessoa certa 4) PRAZO e entregas claras 5) Perguntas de esclarecimento apresentadas como observações profissionais~Escreva o parágrafo de fechamento incluindo: 1) VALOR_DA_PROPOSTA com o detalhamento das entregas 2) Chamada para ação com os próximos passos 3) Disponibilidade para conversar~Formate a proposta completa com espaçamento e estrutura adequados, mantendo-a com menos de 2.000 caracteres. Adicione 2 ou 3 itens de portfólio ou amostras de trabalho como referências numeradas~Revise o texto e identifique frases que poderiam ser mais personalizadas ou impactantes
```

### 23. Estratégia de vendas
> 🔁 Original do repositório PromptChains (traduzido e adaptado)

**Objetivo:** definir objetivos, segmentos, processo, táticas, previsão e ferramentas de vendas.

```
Defina os objetivos de vendas para [produto/serviço]~Identifique os segmentos de clientes-alvo~Descreva o processo e o ciclo de vendas~Desenvolva táticas e técnicas de vendas~Crie uma previsão de vendas~Sugira ferramentas e recursos para a equipe de vendas
```

### 24. Proposta comercial B2B com retorno sobre investimento

**Objetivo:** mostrar ao cliente, com números, por que a compra se paga.

```
CLIENTE=[empresa e contexto], DORES=[problemas levantados na descoberta], SOLUCAO=[o que será entregue], INVESTIMENTO=[preço e condições], DADOS_DO_CLIENTE=[números do cliente que permitem calcular ganho]
Escreva o resumo executivo centrado no resultado para CLIENTE.~
Descreva a situação atual e o custo de não agir com base em DORES.~
Descreva SOLUCAO, escopo, entregas e cronograma.~
Calcule o retorno sobre o investimento e o payback com DADOS_DO_CLIENTE, deixando as premissas explícitas.~
Apresente INVESTIMENTO em opções (bom, melhor, completo).~
Liste os próximos passos e a validade da proposta.~
Revise para que o decisor entenda a proposta em 2 minutos.
```

### 25. Técnicas de fechamento

**Objetivo:** conduzir o cliente à decisão de forma natural e ética.

```
PRODUTO=[produto], ESTAGIO=[momento da negociação], SINAIS_DE_COMPRA=[sinais observados], PERFIL_DO_CLIENTE=[estilo de decisão]
Liste os sinais de compra e como reconhecê-los.~
Explique 6 técnicas de fechamento (resumo de benefícios, alternativa, próximo passo, teste, prazo real, pergunta direta) com exemplos para PRODUTO.~
Indique as técnicas mais adequadas para PERFIL_DO_CLIENTE e ESTAGIO.~
Escreva as frases de fechamento.~
Explique o que fazer depois do "sim" e depois do "não".
```

### 26. Preparação para uma negociação

**Objetivo:** chegar à mesa com estratégia, limites e alternativas claros.

```
NEGOCIACAO=[o que está sendo negociado], OUTRA_PARTE=[quem e seus interesses prováveis], MEUS_OBJETIVOS=[o que quero], MINHA_ALTERNATIVA=[o que faço se não houver acordo], VARIAVEIS=[preço, prazo, volume, condições]
Defina MINHA_ALTERNATIVA (BATNA) e estime a da OUTRA_PARTE.~
Defina meu ponto de abertura, meu alvo e meu limite.~
Estime a zona de possível acordo.~
Liste os interesses por trás das posições dos dois lados.~
Monte a lista de trocas possíveis entre VARIAVEIS (o que cedo e o que peço em troca).~
Antecipe as táticas da OUTRA_PARTE e como responder.~
Escreva o roteiro da abertura da negociação.
```

### 27. Negociação com fornecedores

**Objetivo:** conseguir melhores preços e condições de quem vende para você.

```
FORNECEDOR=[empresa e o que fornece], VOLUME=[quanto compra], CONDICOES_ATUAIS=[preço, prazo, frete], ALTERNATIVAS=[outros fornecedores], OBJETIVO=[o que quer melhorar]
Pesquise referências de mercado para o item fornecido.~
Calcule o valor do seu contrato para FORNECEDOR.~
Defina pedidos prioritários e as concessões possíveis.~
Escreva o roteiro da negociação.~
Escreva o e-mail de pedido de revisão de condições.~
Liste cláusulas importantes a incluir no acordo.
```

### 28. Acompanhamento de proposta sem resposta

**Objetivo:** retomar propostas paradas e descobrir se a venda está viva.

```
PROPOSTA=[o que foi enviado e quando], CLIENTE=[contato e empresa], ULTIMA_INTERACAO=[o que foi conversado]
Escreva o primeiro acompanhamento acrescentando valor.~
Escreva o segundo acompanhamento com pergunta direta sobre o status.~
Escreva a mensagem de "rompimento" educada para obter uma resposta definitiva.~
Escreva o roteiro de ligação de acompanhamento.~
Defina os intervalos entre os contatos.~
Explique como registrar o motivo de perda no CRM.
```

## Gestão comercial

### 29. Playbook de vendas

**Objetivo:** documentar o processo comercial para toda a equipe vender do mesmo jeito.

```
EMPRESA=[descrição], PRODUTOS=[portfólio], PERSONAS=[clientes], PROCESSO_ATUAL=[como se vende hoje], EQUIPE=[papéis comerciais]
Escreva a visão geral: mercado, proposta de valor e diferenciais.~
Documente PERSONAS e suas dores.~
Documente as etapas do processo, com critérios de entrada e saída.~
Inclua roteiros, modelos de e-mail e perguntas para cada etapa.~
Inclua o banco de objeções e de casos de sucesso.~
Defina as regras de uso do CRM.~
Defina indicadores e metas por papel de EQUIPE.
```

### 30. Metas e plano de comissionamento

**Objetivo:** criar metas justas e comissões que motivam o comportamento certo.

```
META_DA_EMPRESA=[meta total], EQUIPE=[vendedores e papéis], HISTORICO=[resultados anteriores], MARGENS=[margens por produto], ORCAMENTO_DE_REMUNERACAO=[limite]
Distribua META_DA_EMPRESA por vendedor, mês e produto, considerando HISTORICO.~
Proponha 3 modelos de comissão (percentual fixo, escalonado, por margem) com prós e contras.~
Simule a remuneração em 3 cenários de desempenho.~
Verifique o custo dentro de ORCAMENTO_DE_REMUNERACAO.~
Inclua incentivos para os comportamentos desejados (margem, retenção, novos clientes).~
Escreva as regras do plano de forma clara.
```

### 31. Revisão do funil e previsão de vendas

**Objetivo:** prever o fechamento do mês com base no funil.

```
OPORTUNIDADES=[lista com valor, etapa, data prevista e última interação], TAXAS_HISTORICAS=[conversão por etapa], META=[meta do período]
Aplique TAXAS_HISTORICAS a OPORTUNIDADES para calcular a previsão ponderada.~
Classifique as oportunidades em compromisso, provável e otimista.~
Identifique oportunidades paradas ou com data irreal.~
Calcule a lacuna em relação a META e a cobertura de funil.~
Defina as ações para fechar a lacuna.~
Monte a pauta da reunião semanal de funil.
```

### 32. Treinamento de vendedores

**Objetivo:** desenvolver a equipe comercial com prática e acompanhamento.

```
EQUIPE=[perfil e experiência], LACUNAS=[o que mais falta: prospecção, descoberta, objeções, fechamento], PRODUTO=[produto], TEMPO=[horas disponíveis]
Crie um diagnóstico rápido das habilidades de EQUIPE.~
Monte um programa de treinamento de 4 semanas focado em LACUNAS.~
Crie exercícios práticos e simulações para cada módulo.~
Crie a ficha de avaliação de ligações e reuniões.~
Defina a rotina de acompanhamento (coaching semanal).~
Defina como medir a evolução.
```

### 33. Organização do CRM e do funil

**Objetivo:** deixar o CRM simples, confiável e útil para a gestão.

```
CRM=[ferramenta], PROCESSO=[etapas de venda], EQUIPE=[quem usa], PROBLEMAS=[dados faltando, funil bagunçado]
Defina as etapas do funil no CRM com critérios objetivos de passagem.~
Defina os campos obrigatórios por etapa.~
Crie as regras de higiene (atualização, oportunidades paradas, motivos de perda).~
Sugira automações de tarefas e lembretes.~
Crie os relatórios essenciais para gestão.~
Escreva o guia de uso para EQUIPE.
```

### 34. Análise de ganhos e perdas

**Objetivo:** aprender com as vendas ganhas e perdidas para vender mais.

```
NEGOCIOS=[lista de vendas ganhas e perdidas com motivos, valores, etapas e concorrentes], PERIODO=[período]
Calcule a taxa de ganho geral e por segmento, produto e vendedor.~
Classifique os motivos de perda e de ganho.~
Identifique em que etapa as perdas acontecem.~
Analise a perda para concorrentes.~
Escreva o roteiro de entrevista com clientes ganhos e perdidos.~
Proponha mudanças no processo, na oferta e no treinamento.
```

## Vendas por canal

### 35. Vendas pelo Instagram

**Objetivo:** transformar seguidores em clientes com conteúdo, direct e fechamento.

```
NEGOCIO=[o que vende], PUBLICO=[público], TICKET=[valor médio], FLUXO_ATUAL=[como vende hoje pelo Instagram]
Desenhe o caminho do seguidor até a compra.~
Defina o conteúdo de venda semanal (provas, bastidores, ofertas, respostas a dúvidas).~
Escreva os roteiros de atendimento no direct, do primeiro contato ao pagamento.~
Escreva respostas rápidas para as perguntas mais comuns.~
Organize o catálogo, os destaques e o link na bio para vender.~
Defina indicadores (mensagens, conversão, ticket).
```

### 36. Vendas em marketplaces

**Objetivo:** vender mais em Mercado Livre, Shopee, Amazon e similares.

```
PRODUTOS=[produtos], MARKETPLACES=[plataformas], CONCORRENCIA=[situação], MARGEM=[margem atual]
Calcule o preço considerando comissões, frete e impostos em cada um dos MARKETPLACES.~
Escreva títulos otimizados para a busca interna.~
Escreva descrições e fichas técnicas completas.~
Defina a estratégia de fotos.~
Defina as ações para melhorar reputação e avaliações.~
Defina o uso de anúncios patrocinados e promoções da plataforma.~
Crie o painel de acompanhamento por produto.
```

### 37. Venda de alto valor em chamada (closer)

**Objetivo:** conduzir uma chamada de vendas de serviços ou programas de alto valor.

```
OFERTA=[serviço ou programa], PRECO=[valor], PERFIL_DO_LEAD=[quem agenda], DURACAO=[minutos]
Escreva o roteiro da chamada: conexão, diagnóstico, aprofundamento da dor, visão de futuro, apresentação, investimento e fechamento.~
Escreva as perguntas de diagnóstico.~
Escreva a transição para a apresentação da OFERTA.~
Escreva a apresentação do investimento e das formas de pagamento.~
Escreva as respostas às objeções típicas de alto valor.~
Liste os limites éticos (sem pressão abusiva, sem promessas de resultado garantido).
```

### 38. Venda complexa com vários decisores

**Objetivo:** conduzir vendas B2B longas com comitê de compra.

```
CONTA=[empresa], SOLUCAO=[o que vende], DECISORES=[pessoas envolvidas], CICLO=[tempo esperado], CONCORRENTES=[quem disputa]
Mapeie o comitê de compra: decisor, influenciadores, usuários, financeiro, jurídico e possíveis opositores.~
Identifique o que cada um valoriza e teme.~
Prepare um defensor interno com materiais de apoio.~
Planeje a sequência de reuniões e entregáveis ao longo de CICLO.~
Antecipe etapas de compras, jurídico e segurança.~
Monte o plano de ação da conta com riscos e próximos passos.
```

### 39. Programa de revendedores e parceiros

**Objetivo:** vender por meio de parceiros que levam seu produto a novos clientes.

```
PRODUTO=[produto], PERFIL_DE_PARCEIRO=[revendedores, agências, consultores, afiliados], MARGEM=[margem disponível], REGIOES=[mercados]
Defina o modelo de parceria (revenda, indicação, afiliação) e as regras.~
Defina comissões ou descontos compatíveis com MARGEM.~
Crie os critérios de seleção de parceiros.~
Escreva a apresentação do programa.~
Crie o kit do parceiro (materiais, treinamento, suporte).~
Defina metas, níveis e acompanhamento.
```

### 40. Vendas em feiras e eventos

**Objetivo:** aproveitar eventos para gerar contatos e vendas.

```
EVENTO=[nome e público], OBJETIVO=[vendas no local, leads, parcerias], ESTANDE=[estrutura], EQUIPE=[pessoas]
Defina as metas do evento.~
Planeje a comunicação antes do evento para atrair visitantes.~
Escreva a abordagem no estande e o roteiro de qualificação rápida.~
Crie a ação de captação de contatos com consentimento.~
Defina a divisão de tarefas de EQUIPE.~
Escreva o acompanhamento pós-evento por segmento de contato.
```
