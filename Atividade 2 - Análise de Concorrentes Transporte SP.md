# Análise Estratégica de Concorrência e Mobilidade Orientada ao Conforto

Análise do posicionamento de mercado e da viabilidade de uma solução de mobilidade voltada ao conforto na Região Metropolitana de São Paulo (RMSP).

## Contextualização do produto

O transporte público da RMSP enfrenta gargalos estruturais e concentração de demanda nos horários de pico. O tempo médio diário de deslocamento citado no estudo é de 2 horas e 47 minutos por habitante [1].

A solução proposta prioriza o conforto do passageiro, em vez de otimizar apenas o tempo ou a distância. Para isso, pode recomendar trajetos mais longos quando ofereçam menor lotação, maior probabilidade de viajar sentado, menos transbordos complexos ou acesso a veículos mais novos e climatizados [2].

### Objetivos de negócio

1. **Elevar a satisfação do usuário:** reduzir o estresse físico e cognitivo associado à superlotação e à incerteza operacional [2].
2. **Promover engajamento e retenção:** integrar a plataforma à rotina dos passageiros com previsões confiáveis de partidas, conexões e itinerários frequentes [3].
3. **Desenvolver monetização híbrida:** explorar dados agregados e anonimizados de mobilidade para planejamento urbano e parcerias com operadores de mídia Out-of-Home (OOH) e estabelecimentos em terminais [5].

### Matriz CSD

- **Certeza:** o sistema metroferroviário e rodoviário da RMSP não tem vazão adequada para absorver a demanda concentrada nos horários de pico.
- **Suposições:** os passageiros fazem trajetos subótimos por falta de informação em tempo real; o horário de pico é um fator importante na perda de bem-estar; e parte dos usuários aproveitaria o deslocamento para outras atividades se tivesse espaço e acomodação adequados [1].
- **Dúvidas:** há disponibilidade e atualização contínua de dados sobre a lotação de plataformas e veículos? Os passageiros trocariam mais tempo de viagem por maior conforto físico e mental? [6]

## Mapeamento e análise dos concorrentes

### Moovit

O Moovit, pertencente ao grupo Mobileye, está presente em mais de 3.500 cidades de 112 países [7]. Combina dados estáticos de transporte no padrão GTFS, sinais de GPS da frota e contribuições da comunidade. Seu roteamento é multimodal, abrangendo ônibus, metrô, trens, trilhos leves, micromobilidade compartilhada e transporte sob demanda [8].

Na Grande São Paulo, integra a compra e recarga do Bilhete Único ao aplicativo, em parceria com a Primova Pay e com autorização da SPTrans [7]. Seu modelo de receita inclui:

- **B2C:** assinatura Moovit Plus e anúncios no plano gratuito;
- **B2B/B2G:** análises de mobilidade e relatórios de origem-destino para governos e operadoras;
- **Parcerias:** comissões por recargas e integrações com serviços de transporte [5].

O Moovit compartilha com a proposta o roteamento multimodal, os avisos de alterações operacionais, a recarga de bilhetes e a oferta de planos premium [7]. Porém, prioriza rotas rápidas ou com menos transbordos e não oferece filtros dinâmicos de conforto baseados na lotação de veículos e plataformas. O documento informa mais de 28 milhões de usuários ativos globais e cerca de 400 mil usuários ativos mensais na RMSP [6].

### Cittamobi

Desenvolvido pela Primova, o Cittamobi atende mais de 350 municípios em 19 estados e monitora mais de 80 mil ônibus [14]. Seu posicionamento destaca a previsão de chegada dos veículos (ETA), baseada em dados de telemetria e rastreamento das operadoras [3]. A assinatura Cittamobi+ oferece recursos de inteligência artificial para avisos sobre atrasos, mudanças de itinerário e problemas nas linhas [11].

O aplicativo também conta com o módulo Cittamobi Acessibilidade e oferece pagamento e recarga por Bluetooth e Pix em linhas da capital paulista [15][17]. Suas fontes de receita incluem:

- **B2C:** anúncios no plano gratuito e assinatura Cittamobi+;
- **B2B/B2G:** plataforma Qualimob e projetos de inteligência operacional;
- **Transações:** bilhetagem digital e pagamentos por aproximação ou Bluetooth [2][4].

As semelhanças com a proposta incluem alertas em tempo real, assinatura premium, recarga digital e coleta de dados comportamentais. A diferença apontada é a concentração no modal rodoviário e no tempo de espera em pontos, sem recomendar trajetos mais longos em troca de menor lotação ou veículos climatizados. O documento informa mais de 45 milhões de usuários cadastrados no país.

### Citymapper

O Citymapper é uma plataforma internacional de planejamento de viagens disponível em São Paulo. Compara opções de transporte sobre trilhos, ônibus, táxis, aplicativos de transporte individual, bicicletas compartilhadas e caminhada [8]. Entre seus recursos estão orientações detalhadas para escolher vagões, facilitar baldeações e encontrar saídas de estações [13].

Seu modelo de receita é predominantemente B2C, com as assinaturas Citymapper CLUB e CLUB+, além de anúncios e parcerias de afiliados com serviços de mobilidade [8].

Entre as convergências com a proposta estão a comparação de custos, o mapeamento de estações, os alertas em tempo real e a variação de itinerários por preferências [1]. O estudo aponta como diferenças a ausência de integração direta com o Bilhete Único e o Cartão TOP e a falta de monitoramento da lotação de veículos e plataformas na RMSP. Também registra dezenas de milhões de downloads globais e avaliações médias de 4,9 estrelas [1].

### Aplicativo TOP (Autopass)

Desenvolvido pela Autopass em parceria com a Pefisa, o Aplicativo TOP funciona como carteira digital para o sistema sobre trilhos e ônibus intermunicipais da RMSP, incluindo CPTM, Metrô e linhas da EMTU [22]. Permite comprar bilhetes digitais por QR Code, gerenciar o Cartão TOP e fazer recargas por Pix ou cartão [22].

Sua monetização está centrada em serviços financeiros e transacionais, como tarifas e receitas relacionadas à emissão e recarga de bilhetes, conta digital e cartões oferecidos com a Pefisa [22].

O TOP se aproxima da proposta pela conveniência de recarga e pelo apoio financeiro ao deslocamento. Entretanto, atua principalmente como carteira de pagamentos e não oferece recomendação de rotas por conforto, monitoramento da lotação de plataformas ou mapeamento de lojas nas estações. O documento informa mais de 10 milhões de cadastros e downloads na RMSP [23].

## Matriz comparativa de funcionalidades

| Requisito / funcionalidade | Solução proposta | Moovit | Cittamobi | Citymapper | Aplicativo TOP |
|---|---|---|---|---|---|
| Modelo de monetização | A definir | Assinatura Moovit Plus, anúncios, dados B2B/B2G (Analytics) e comissões de recarga [5] | Assinatura Cittamobi+, anúncios, Qualimob e bilhetagem [2] | Assinatura Citymapper CLUB, anúncios e parcerias de micromobilidade/táxi [3] | Tarifas de bilhetagem e serviços financeiros/conta digital (Pefisa) [16] |
| Uso gratuito | Sim | Sim [1] | Sim | Sim [1] | Sim [22] |
| Conta premium | Sim | Sim (Moovit Plus) | Sim (Cittamobi+) | Sim (Citymapper CLUB) [1] | Não |
| Recarga do Bilhete Único / TOP | Sim | Sim [5] | Sim [6] | Não | Sim [2] |
| Comunicação de problemas em tempo real | Sim | Sim [13] | Sim | Sim [13] | Parcial |
| Encontrar rota mais confortável | Sim | Não | Não | Parcial | Não |
| Contabilização da lotação da plataforma | Sim | Não | Não | Não | Não |
| Mapa das estações | Sim | Sim | Sim | Sim [13] | Parcial |
| Custo total da rota | Sim | Sim | Sim | Sim [1] | Sim |
| Informações sobre lojas nas estações | Sim | Não | Não | Não | Não |
| Recurso de acessibilidade | A definir | Rotas acessíveis e suporte a leitores de tela | Cittamobi Acessibilidade [15] | Filtro de rotas sem degraus/acessíveis | Suporte básico do sistema |
| Feedback para setor público e concessionárias | Não (em breve) | Sim (Analytics) | Sim (Qualimob) [1] | Não | Não |

## Lacunas, viabilidade técnica e monetização

### Diferenciação pelo algoritmo de conforto

As plataformas analisadas priorizam a redução do tempo de percurso e do número de transbordos [5]. Segundo dados do levantamento Qualimob citados no documento, fatores ligados à experiência física têm relevância para a percepção de qualidade: temperatura e ventilação (42,0%), conservação do veículo (37,8%) e baixa lotação (36,4%).

A proposta pode diferenciar-se ao permitir que o usuário defina sua tolerância a um acréscimo no tempo de viagem — por exemplo, de 10 a 20 minutos — em troca de menor lotação, maior chance de viajar sentado ou veículos climatizados.

### Medição da lotação em plataformas

A medição da lotação exige uma arquitetura de dados híbrida, considerando a falta de padronização das APIs públicas e das concessionárias. O documento sugere três fontes complementares:

1. **Inteligência colaborativa (crowdsourcing):** permitir que passageiros informem o nível de ocupação e recompensar contribuições validadas com pontos ou descontos no plano premium.
2. **Modelagem preditiva:** usar aprendizado de máquina com dados históricos de catracas, tabelas operacionais, ocorrências e variações de horário para estimar a concentração de passageiros.
3. **Integração com IoT e câmeras:** buscar acordos para receber dados agregados de sensores de densidade Wi-Fi e análises de vídeo em estações operadas por concessionárias, como ViaQuatro e ViaMobilidade.

### Canal B2G e parcerias OOH / conveniência

A ausência de um canal de feedback e de analytics para o setor público é uma desvantagem em relação ao Moovit e ao Cittamobi. Desenvolver essa capacidade pode apoiar uma fonte de receita B2G e fortalecer o relacionamento com os órgãos gestores da RMSP [2][3].

O mapeamento de lojas e serviços nas estações também pode abrir uma frente de monetização: ao recomendar que o usuário aguarde um trem menos lotado, o aplicativo pode sugerir cafeterias, livrarias e outros estabelecimentos próximos. Parcerias com operadores de mídia DOOH e concessionárias poderiam incluir anúncios geolocalizados e cupons de desconto durante o tempo de espera.

## Conclusões

A análise identifica uma oportunidade de mercado em navegação orientada ao conforto e ao bem-estar. Embora existam concorrentes consolidados, as soluções atuais priorizam o tempo de percurso e não tratam diretamente os impactos da superlotação e da falta de climatização [1].

A combinação de rotas baseadas em densidade de passageiros, monitoramento de plataformas, recarga de bilhetagem e informações sobre estabelecimentos nas estações pode diferenciar o produto. As recomendações do documento são:

- priorizar a precisão do algoritmo de conforto;
- estruturar parcerias de mídia OOH geolocalizada;
- desenvolver o canal de inteligência de dados B2G.

## Referências

1. [Transporte público: busca viagens começa antes em SP — Estadão](https://mobilidade.estadao.com.br/meios-de-transporte/paulistanos-procuram-rotas-no-transporte-publico-meia-hora-antes-que-buenos-aires-e-cidade-do-mexico/)
2. [Pesquisa Qualimob — Cittamobi](https://www.cittamobi.com.br/pesquisa-qualimob-cittamobi/)
3. [A mobilidade urbana ainda é analógica; o passageiro já... — Cittamobi](https://www.cittamobi.com.br/blog/a-mobilidade-urbana-ainda-e-analogica-o-passageiro-ja-e-100-digital/)
4. [Moovit apresenta edição 2024 do seu relatório global](https://moovit.com/pt/press-releases/moovit-2024-global-report-usa/)
5. [Análise de Mobilidade Urbana — Moovit](https://moovit.com/pt/maas-solutions-pt/urban-mobility-analytics/)
6. [Moovit: 6 milhões de usuários no Brasil — BRIL Chamber](https://brilchamber.org.br/moovit-6-milhoes-de-usuarios-no-brasil/)
7. [Recarga do Bilhete Único pelo aplicativo Moovit — Diário do Transporte](https://diariodotransporte.com.br/2025/10/22/recarga-do-bilhete-unico-ja-pode-ser-feita-pelo-aplicativo-moovit-com-tecnologia-da-primova-pay-em-sao-paulo/)
8. [Citymapper — App Store Brasil](https://apps.apple.com/br/app/citymapper/id469463298)
9. [Moovit permite recarga do Bilhete Único em São Paulo](https://moovit.com/pt/press-releases/moovit-permite-recarga-do-bilhete-unico-em-sao-paulo/)
10. [Carregue seu Bilhete Único direto no Moovit](https://moovit.com/pt/blog/carregue-seu-bilhete-unico-direto-no-moovit/)
11. [A inteligência é coletiva — NTU](https://ntu.org.br/ntu-urbano/38/a-inteligencia-e-coletiva)
12. [Índice do Moovit sobre o Transporte Público](https://moovitapp.com/insights/pt-br/Moovit_Insights_%C3%8Dndice_sobre_o_Transporte_P%C3%BAblico-countries)
13. [App de rotas de transporte público atinge 1 milhão de usuários no Brasil — Folha de S.Paulo](https://m.folha.uol.com.br/tec/2014/05/1447725-app-de-rotas-de-transporte-publico-atinge-1-milhao-de-usuarios-no-brasil.shtml)
14. [Conheça o Cittamobi — Líder em Mobilidade Urbana Digital](https://www.cittamobi.com.br/sobre-a-cittamobi/)
15. [Pesquisa inédita avalia cenário do transporte público no Brasil — Cittamobi](https://www.cittamobi.com.br/blog/pesquisa-inedita-avalia-cenario-do-transporte-publico-no-brasil/)
16. [Cittamobi Acessibilidade chega a São Paulo — Technibus](https://technibus.com.br/2023/12/11/cittamobi-acessibilidade-chega-a-sao-paulo-sp)
17. [Ônibus em São Paulo passam a aceitar pagamento via Bluetooth — Cittamobi](https://www.cittamobi.com.br/blog/onibus-em-sao-paulo-passam-a-aceitar-pagamento-via-bluetooth-em-296-linhas/)
18. [Guia da Cidade de São Paulo 2022 — Prefeitura de São Paulo](https://cidadedesaopaulo.com/wp-content/uploads/2023/11/Guia-da-Cidade_ING_2022-Site.pdf)
19. [10 Tips For Women Travelling To São Paulo, Brazil — Zafigo](https://zafigo.com/cities/women-travel-tips-sao-paulo-brazil-city-guide/)
20. [Citymapper 10.2 APK — APKMirror](https://www.apkmirror.com/apk/citymapper-limited/citymapper/citymapper-10-2-release/)
21. [Citymapper — App Store Suécia](https://apps.apple.com/sv/app/citymapper/id469463298)
22. [Prêmio Consumidor Moderno 2024 — Empresas Vencedoras](https://consumidormoderno.com.br/revista/premio-consumidor-moderno-2024-empresas-vencedoras/)
23. [Anuário do Ônibus — AEAMESP](https://www.aeamesp.org.br/boletim/wp-content/uploads/sites/4/2023/06/000000-PDF-LEVE-ANU%C3%81RIO-2023.pdf)
24. [Produção de Projetos de Smart Cities — Repositório UFMG](https://repositorio.ufmg.br/bitstream/1843/79469/1/PRODU%C3%87%C3%83O%20DE%20PROJETOS%20DE%20SMART%20CITIES%20-%20Gustavo%20Mattos.pdf)
