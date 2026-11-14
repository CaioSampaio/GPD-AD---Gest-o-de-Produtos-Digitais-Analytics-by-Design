# Avaliação exploratória de usabilidade | ConfyCity

**Valmir conseguiu comparar rotas e concluir uma viagem demonstrativa. A consulta que motivaria seu uso, Suzano → Campo Belo, ficou fora da cobertura do protótipo.** O exemplo mostrou como o ConfyCity pode ajudar a ponderar tempo, lotação e custo. Também revelou que o atraso de uma ocorrência pode mudar a melhor escolha sem aparecer no tempo exibido no cartão principal.

A avaliação foi realizada no protótipo público do ConfyCity em 14 de novembro de 2026, com base nos três arquivos anexados. As observações vêm de interações no navegador. As interpretações são da perspectiva da persona sintética, e as hipóteses precisam ser verificadas com passageiros reais.

## 1. Persona e critérios de avaliação

Valmir Vasko tem 56 anos, mora em Suzano e trabalha como controlador de acesso no Campo Belo. Pega trens lotados, corre para conseguir embarcar no horário e se ressente do cansaço da rotina. Quer dormir mais e passar mais tempo com a família. O perfil registra que ele consulta notícias antes de sair, o que torna relevante testar se encontraria rapidamente as condições do transporte.

Usei **07h30 como horário de teste**, pois o arquivo não informa sua hora de saída. Para a simulação, considerei satisfatória uma experiência em que Valmir pudesse buscar o trajeto habitual, identificar ocorrências e comparar, com poucos passos, quanto tempo e dinheiro uma opção menos lotada custaria. A tolerância a minutos extras e a forma como ele interpreta sinais de conforto são hipóteses.

## 2. Registro da navegação

| Página ou fluxo | Objetivo e ações realizadas | Resultado observado e dificuldade |
| --- | --- | --- |
| **Planejar** | Busquei com os campos vazios, consultei a situação das linhas e testei preencher e inverter origem e destino. | O formulário indicou os três campos obrigatórios e levou o foco à origem. A inversão trocou os campos. A situação das linhas apareceu na inicial com horário fictício de atualização. |
| **Suzano → Campo Belo** | Digitei os dois locais e busquei às 07h30. Em seguida, acionei **Usar trajeto de exemplo**. | A tela informou que o trajeto estava fora da demonstração, listou os quatro exemplos cobertos e abriu Itaquera → Paulista. A tarefa principal de Valmir parou nesse ponto. |
| **Comparar e ver detalhes** | Consultei os quatro trajetos de exemplo, abri os detalhes das 11 opções e testei ordenar por duração, custo e lotação. Selecionei uma rota e depois outra. | Os cartões exibiram duração, custo, baldeações e lotação. A ordem respondeu aos controles. A segunda seleção substituiu a primeira, e o botão de continuação passou a apontar para a última rota escolhida. |
| **Ocorrências** | Em Itaquera → Paulista, abri o aviso da Linha 3 e troquei para a opção B. Em Barra Funda → Pinheiros, abri o aviso da Linha 4 e mantive a opção afetada. | As duas decisões tiveram confirmação. No primeiro caso, os **47 min** do cartão passaram a **cerca de 59 min** com o impacto possível, diante de **55 min** da alternativa. Essa diferença só apareceu ao abrir o aviso. |
| **Viagem e chegada** | Iniciei a opção B, avancei, voltei uma etapa e abri **Ver na estação** no aviso de interdição da saída Consolação. Retornei à viagem e concluí. | O acompanhamento retomou no mesmo trecho, e a tela de chegada resumiu a rota e registrou o alerta. A planta aberta mostrou a saída para a Av. Paulista, sem explicitar a relação dela com a saída interditada. |
| **Estações e acessibilidade** | Visitei República, Luz, Paulista, Brás, Sé, Pinheiros e Vila Mariana. Na Paulista, ativei o caminho com elevador e avancei na instrução. | A instrução passou a indicar elevador. Os estados de acessibilidade distinguiram disponibilidade no exemplo, restrição e informação indisponível. Nas telas visitadas não encontrei um controle de áudio. |
| **Alertas** | Testei edição do horário, confirmei um alerta demonstrativo de chuva com sábado incluído e tentei enviar com todos os dias desmarcados. | O alerta apareceu na lista local. O formulário bloqueou o envio sem dias e explicou como corrigir. O campo aceitou `06:50` por digitação sequencial. A interface informou que o alerta não dispara notificações. |
| **Salvas e falta de conexão** | Salvei a opção B, reabri a rota e simulei falta de conexão. Tentei uma nova busca e reativei a conexão simulada. | A consulta preservou as etapas, o custo e a duração da última busca. Lotação, ocorrências e clima ficaram indisponíveis. A nova busca mostrou uma mensagem de falha e abriu os resultados após a reativação. |
| **Relatos** | Enviei o formulário vazio e depois registrei, separadamente, lotação alta e atraso na Luz. | O formulário pediu o tipo de relato quando estava vazio. Os dois registros apareceram na seção local, separada dos relatos fictícios de outras pessoas. |
| **Comércios, clima e Mais** | Combinei destino, interesse e acesso sem degraus. Abri a previsão, os atalhos de acessibilidade e o tema escuro. | Os filtros chegaram a **0 de 5** e exibiram mensagem de lista vazia. A previsão distinguiu períodos do dia e sinalizou ausência de dados à noite. O tema escuro alternou e foi revertido. |

## 3. Avaliação pelas metas de usabilidade

| Meta | Observação | Interpretação pela persona | Hipótese a validar |
| --- | --- | --- | --- |
| **Facilidade de aprendizagem** | Origem, destino, horário e situação das linhas estavam na inicial. O primeiro erro levou o foco ao campo que precisava de correção. | Valmir teria um ponto de partida claro antes de sair de casa. | Passageiros em primeiro uso conseguem encontrar os avisos e explicar o que muda entre duas opções sem ajuda. |
| **Eficiência** | Os critérios de ordenação reorganizaram os cartões. O tempo ajustado pela ocorrência exigiu abrir outra tela. | Sob pressão de horário, Valmir poderia escolher pelo primeiro cartão e descobrir o atraso depois. | Mostrar o tempo ajustado no cartão melhora a decisão e reduz a necessidade de abrir detalhes. |
| **Facilidade de memorização** | Foi possível retornar à opção B pelo menu **Salvas**, na mesma sessão. | O menu pode reduzir o esforço de repetir a busca do trajeto habitual. | Após alguns dias, passageiros voltam a encontrar a rota e o alerta sem instruções. |
| **Segurança e recuperação** | O protótipo indicou campos faltantes, explicou a cobertura e permitiu recuperar a busca após a falha simulada. O aviso de interdição abriu uma planta com contexto parcial. | É mais fácil saber quando corrigir uma entrada ou quando falta informação. Durante uma interdição, ainda seria preciso confirmar por onde sair. | Passageiros conseguem distinguir dado fictício, desatualizado e indisponível e identificar uma ação adequada em cada caso. |
| **Satisfação** | Os cartões explicitaram ganhos e perdas. O trajeto habitual ficou sem resultado. | A comparação pode aliviar a incerteza quando existe cobertura. Para Valmir, a falta da própria rota limita o valor imediato. | A utilidade percebida depende de cobertura do trajeto habitual, atualização compreensível e uma alternativa compatível com o horário de chegada. |

## 4. Framework de Feedback

| Quadrante | Página ou fluxo | Evidência observada | Percepção da persona | Impacto | Recomendação |
| --- | --- | --- | --- | --- | --- |
| **O que funciona** | Comparar | A opção B tinha lotação moderada e custava o mesmo que a A, com 8 minutos a mais na comparação-base. | Valmir consegue identificar o que ganharia em espaço e quanto isso custaria em tempo. | Alto | Preservar as diferenças explícitas entre as rotas. |
| **O que funciona** | Ocorrências | A tela mostrou o impacto em minutos, ofereceu alternativa e confirmou a troca. | O aviso ajuda Valmir a decidir o que fazer com a informação. | Alto | Manter a comparação perto da ação de trocar ou manter. |
| **O que funciona** | Salvas | A rota preservou etapas e marcou dados variáveis como indisponíveis no modo offline simulado. | Valmir pode recuperar o caminho e saber quais condições precisa confirmar. | Médio | Preservar a indicação de quando a consulta foi salva. |
| **O que pode ser melhorado** | Busca habitual | Suzano → Campo Belo ficou sem opções. A cobertura só foi detalhada depois do envio. | Valmir investe tempo na consulta e precisa mudar de trajeto para entender a proposta. | Alto | Incluir o corredor da persona na demonstração e informar a cobertura junto ao formulário. |
| **O que pode ser melhorado** | Comparar | A opção afetada apareceu primeiro por duração-base com 47 min, embora a ocorrência estimasse cerca de 59 min e a alternativa tivesse 55 min. | Sob pressão, Valmir pode interpretar o primeiro cartão como a melhor opção para chegar a tempo. | Alto | Mostrar o tempo-base e o tempo ajustado no cartão. Explicitar qual valor governa a ordenação. |
| **O que pode ser melhorado** | Seleção de rota | A segunda seleção substituiu a primeira. O rótulo **Selecionar** não informa a finalidade da ação. | Valmir poderia tentar marcar duas opções para confrontá-las e perder a primeira seleção. | Médio | Se a ação serve para escolher uma rota, usar **Escolher esta rota**. |
| **Dúvidas que surgiram** | Estação Paulista | **Ver na estação** abriu a planta da Paulista, com instruções para a Av. Paulista. | “Essa é a saída alternativa à Consolação? Como chego até ela?” | Alto | Levar diretamente à instrução alternativa e manter o aviso visível. |
| **Dúvidas que surgiram** | Lotação estimada | A escala tinha três níveis e a interface informou que ela não garante assento. | “Moderada onde e a que horas? Vou conseguir embarcar nesse trecho?” | Médio | Associar a estimativa ao trecho e ao horário de embarque, com fonte e atualização. |
| **Novas ideias** | Comparação de alternativas | Os cartões expõem os mesmos critérios, mas a seleção é única. | Valmir poderia confrontar a rota rápida e a menos lotada sem percorrer novamente os cartões. | Médio | Testar uma tabela compacta para duas opções e uma preferência de máximo de minutos extras. |
| **Novas ideias** | Trajeto habitual | A inicial mostra situação por linha, e a rota habitual pode ser representada por uma rota salva. | Valmir poderia usar uma única consulta antes de sair para decidir se mantém o plano. | Alto | Testar um atalho **Como está meu trajeto?**, com avisos relevantes, hora da atualização e alternativa quando houver. |

## 5. Quadrante visual

![Framework de Feedback do ConfyCity para a persona sintética Valmir Vasko](<Prompt Validação Persona Sintética - ConfyCity Quadrante Feedback.png>)

### Conteúdo do quadrante

**O que funciona**
- Tempo, custo e lotação lado a lado nos cartões.
- Ocorrência explica o impacto e oferece alternativa.
- Rota salva preserva etapas na simulação offline.

**O que pode ser melhorado**
- Suzano → Campo Belo ficou fora da cobertura.
- Rota com ocorrência lidera por duração-base.
- Selecionar outra rota substitui a anterior.

**Dúvidas que surgiram**
- O atraso já está no tempo do cartão?
- O que é lotação moderada no meu embarque?
- Qual saída devo usar após a interdição?

**Novas ideias**
- Comparar duas rotas em uma tabela compacta.
- Definir o máximo de minutos extras aceitável.
- Consultar a situação do trajeto habitual.

*Teste exploratório em navegador · 14 de novembro de 2026*

## 6. Conclusão

Valmir encontraria uma proposta fácil de entender e, no exemplo, conseguiria tomar uma decisão entre tempo e lotação, trocar de rota e chegar ao fim da simulação. Seu caso cotidiano terminaria na tela sem resultados.

| Três pontos positivos | Três principais problemas |
| --- | --- |
| Comparação clara de tempo, custo, baldeações e lotação. | Suzano → Campo Belo fora da cobertura. |
| Ocorrência com estimativa de impacto, alternativa e confirmação da decisão. | Duração-base pode liderar a ordenação mesmo quando a ocorrência muda a escolha. |
| Rota salva com etapas preservadas e indicação explícita de dados indisponíveis. | Aviso de saída interditada abre uma planta que deixa a alternativa implícita. |

### Melhorias prioritárias, na ordem proposta

1. Incluir Suzano → Campo Belo e um cenário de volta na demonstração para avaliar as decisões de Valmir nos dois sentidos.
2. Levar o impacto da ocorrência ao cartão e tornar o critério de ordenação explícito.
3. Vincular cada interdição à saída alternativa e às instruções correspondentes.

### Fluxos e condições sem teste completo

O percurso de Valmir ficou sem resultados. A conclusão da viagem foi testada de ponta a ponta na opção B de Itaquera → Paulista. As outras opções tiveram busca e detalhes inspecionados. Não houve teste de áudio, perda real de conexão, notificações reais, envio colaborativo entre dispositivos, atualização de dados por operadores, uso no celular ou retorno após um intervalo. Também não acionei exclusões nem restauração de dados.

### Hipóteses para validar com passageiros reais

- Quanto tempo extra aceitariam por menor lotação na ida e na volta?
- Conseguiriam escolher a opção mais rápida quando um atraso muda a comparação?
- Que evidência de atualização e origem do dado seria suficiente para confiar na previsão?
- Após alguns dias, voltariam a encontrar a rota e os alertas sem ajuda?

### Considerando as características desta persona, a solução parece atender às suas necessidades? Por quê?

**Parcialmente.** O protótipo demonstra como Valmir poderia comparar conforto e tempo e reagir a um atraso. Para atender à rotina dele, precisa cobrir Suzano → Campo Belo, mostrar o impacto das ocorrências onde ele escolhe a rota e dar informação confiável antes de sair de casa.
