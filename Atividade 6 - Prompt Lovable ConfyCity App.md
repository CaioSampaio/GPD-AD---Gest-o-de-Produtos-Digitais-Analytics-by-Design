# Prompt para Lovable — ConfyCity App

Copie o prompt abaixo para o Lovable. Ele descreve um **protótipo navegável**, não uma aplicação operacional.

```text
Crie um protótipo navegável mobile-first para o ConfyCity App, uma proposta de aplicativo de transporte público que ajuda passageiros a comparar rotas por conforto, duração, custo e condições do trajeto.

CONTEXTO E OBJETIVO
Entrevistas qualitativas do projeto relatam lotação, desconforto físico, imprevisibilidade e dificuldade para encontrar informações de transporte em um só lugar. Algumas pessoas entrevistadas indicaram que considerariam uma rota mais longa para viajar com mais conforto. Esses relatos são qualitativos e não representam todos os passageiros.

O objetivo deste protótipo é demonstrar a jornada completa do planejamento à chegada e testar se passageiros entendem as informações e conseguem escolher uma rota equilibrando conforto, tempo e custo.

ESCOPO
Inclua uma jornada clicável que permita:
1. Informar origem, destino e horário.
2. Comparar pelo menos duas alternativas considerando duração, custo, baldeações e lotação/conforto estimados.
3. Abrir detalhes de uma rota e entender os critérios e a origem demonstrativa das informações.
4. Consultar uma ocorrência simulada, comparar uma alternativa e escolher trocar ou manter a rota.
5. Percorrer etapas demonstrativas de uma estação e consultar informações de acessibilidade.
6. Consultar clima e comércios de interesse demonstrativos.
7. Configurar e consultar um alerta agendado demonstrativo.
8. Registrar um relato de lotação/ocorrência apenas como demonstração local.
9. Salvar e reabrir uma rota em uma experiência de consulta offline simulada.
10. Concluir a jornada com uma tela de chegada.

DADOS E LIMITES
- Use somente dados estáticos/mock criados para a demonstração. Identifique-os de forma persistente com um aviso visível: “Protótipo — dados simulados, não representam a operação real”.
- Rotas, tempos, custos, lotação, ocorrências, clima, acessibilidade, comércios, fontes e horários são exemplos fictícios. Não os apresente como informação atual ou fornecida por operadores.
- Escolha nomes de locais e estações coerentes com um exemplo de transporte na RMSP, mas deixe claro que os trajetos e valores são demonstrativos.
- Não conecte APIs, operadores, mapas externos, autenticação, banco de dados ou notificações push. Não solicite localização do dispositivo.
- Não afirme que há assento disponível ou que uma rota é segura. Apresente atributos ilustrativos e deixe a escolha com o usuário.
- Alertas e relatos apenas atualizam o estado local da interface. Mostre que não foram enviados nem gerarão notificações reais.
- Para rotas salvas, use estado local do protótipo; se houver persistência no navegador, limite-a aos dados demonstrativos.

JORNADA E TELAS
1. Início/planejamento:
   - Campos de origem, destino e horário, com exemplos preenchidos opcionalmente e botão “Buscar rotas”.
   - Acesso a “Rotas salvas”.
   - Valide campos obrigatórios e mostre mensagens junto aos campos com erro.
2. Resultados:
   - Exiba dois ou três cartões de rotas demonstrativas.
   - Compare duração, custo simulado, quantidade de baldeações e lotação/conforto em texto e ícone; não use somente cores.
   - Permita abrir detalhes, ordenar por menor duração/custo ou menor lotação estimada e selecionar uma alternativa.
   - Não declare uma opção universalmente melhor; destaque trade-offs.
3. Detalhes da rota:
   - Mostre etapas, conexões e informações comparáveis.
   - Exiba “estimativa demonstrativa”, fonte fictícia/ilustrativa e horário de atualização igualmente fictício.
   - Inclua acessibilidade disponível no exemplo, botão para salvar e ação de iniciar esta rota.
4. Ocorrência:
   - Em pelo menos uma rota, permita abrir um aviso de ocorrência simulada e seu possível impacto.
   - Compare com uma alternativa e ofereça “Trocar de rota” e “Manter rota”.
   - Ao trocar, atualize as etapas mostradas; mantenha o aviso de protótipo visível.
5. Acompanhamento e estação:
   - Mostre etapa atual e próximas etapas numa lista simples.
   - Inclua navegação esquemática da estação e informação de acessibilidade; identifique tudo como demonstrativo.
   - Mostre ações para consultar chuva no destino e comércios de interesse, sem sugerir integração real.
6. Alertas e relatos:
   - Permita selecionar um horário/categoria e confirmar um alerta de demonstração.
   - Permita escolher uma categoria de relato (por exemplo, lotação ou ocorrência) e confirmar localmente.
   - Após cada ação, explique que nada foi enviado e nenhuma notificação real será disparada.
7. Rotas salvas/offline:
   - Exiba trajetos salvos demonstrativos.
   - Ao abrir um trajeto, mostre que a experiência offline é uma simulação e indique claramente qualquer informação indisponível.
8. Chegada:
   - Mostre conclusão da rota demonstrativa e um botão para iniciar nova busca.

ESTADOS E ERROS
- Campos obrigatórios ausentes: destaque o campo e explique como corrigir.
- Busca sem resultados: explique que não há opção no conjunto de demonstração e permita editar a busca.
- Informação indisponível/desatualizada: identifique-a como tal; nunca a substitua por um valor inventado sem rótulo.
- Falha de conexão simulada: explique quais dados salvos ainda podem ser consultados.
- Ações de alerta/relato: apresentar confirmação local e aviso explícito de que não foram transmitidas.
- Permitir voltar às etapas anteriores sem apagar a busca.

DESIGN E ACESSIBILIDADE
- Adote uma direção visual urbana, acolhedora e leve. A identidade da marca usa ciano-aqua com tons pastéis claros; use o ciano-aqua como cor de destaque e reserve os tons pastéis para fundos e superfícies, sem sacrificar o contraste de textos e controles.
- Como não há arquivo de logo, use “ConfyCity” como marca tipográfica provisória. Não invente símbolo ou identidade visual definitiva.
- Use tipografia sem serifa arredondada e legível, cartões claros, cantos suaves e hierarquia visual consistente. Evite aparência infantil, excesso de ornamentos ou sombras pesadas.
- Ofereça tema claro e tema escuro com um alternador acessível e persistente durante a navegação. No tema escuro, adapte superfícies, texto e estados para manter contraste adequado; não use tons pastéis claros como texto sobre fundo claro.
- Priorize telas mobile, com layout responsivo para desktop.
- Use uma barra de navegação inferior fixa no mobile com ícone e rótulo, por exemplo: “Planejar”, “Alertas”, “Salvas” e “Mais”. Mantenha a jornada da rota em etapas e deixe claro como voltar ao planejamento. Em telas maiores, adapte a navegação sem perder os mesmos destinos.
- Na tela de resultados, priorize cartões comparativos de rotas; inclua um mapa esquemático/ilustrativo como complemento visual, não como foco nem como mapa conectado a serviço externo.
- Dê destaque visual aos trade-offs de duração, conforto e custo, evitando excesso de informação por tela.
- Use rótulos textuais junto a ícones; não dependa somente de cores para lotação, alertas ou acessibilidade.
- Mantenha contraste legível, tipografia confortável, controles com área de toque adequada, foco visível e navegação por teclado.
- Use estrutura semântica, mensagens claras, estados de foco/seleção/erro e alvos de toque adequados. Verifique a legibilidade nos dois temas e não use cor como único indicador.
- Inclua aviso persistente de dados simulados em todas as telas.

CRITÉRIOS DE ACEITE
- Um usuário consegue completar a busca, comparar rotas, abrir detalhes, escolher uma opção, responder a uma ocorrência simulada e chegar à tela final.
- Em cada alternativa, duração, custo, baldeações e estimativa de conforto podem ser comparados.
- A interface deixa claro em todas as telas que os dados são simulados e não representam operação real.
- O usuário pode manter ou trocar a rota após ver uma ocorrência.
- Navegação de estação, acessibilidade, clima/comércio, alertas, relatos e rotas salvas podem ser acessados durante a demonstração.
- Alertas e relatos não fazem chamadas externas e explicam que não foram enviados.
- O protótipo apresenta estados de validação, vazio e dados indisponíveis.
- A jornada é utilizável em telas pequenas e não depende exclusivamente de cor ou hover.
- A marca aparece como wordmark tipográfico “ConfyCity”, com ciano-aqua e tons pastéis, sem símbolo inventado.
- A barra inferior dá acesso claro a Planejar, Alertas, Salvas e Mais; os cartões de rota são o foco dos resultados e o mapa é apenas complementar.
- O alternador de tema claro/escuro funciona e mantém legibilidade, contraste e estados identificáveis em ambos os temas.

IMPLEMENTAÇÃO E LIMITES
- Construa a interface e navegação com dados locais/mock, sem backend.
- Não adicione login, pagamento, recarga, geolocalização, integração externa, notificações push ou envio real de relatos.
- Não mostre informações fictícias como previsões reais; mantenha rótulos de demonstração visíveis e próximos aos dados.
- Mantenha o fluxo principal de busca e comparação como foco; os demais recursos devem estar acessíveis sem interromper a tarefa central.
```
