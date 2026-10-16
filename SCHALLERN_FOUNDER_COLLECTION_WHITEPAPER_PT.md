# Schallern — Whitepaper da Founder Collection

**Versão 0.1 · Rascunho de trabalho · 16 de outubro de 2026 · Culturetek Pte. Ltd., Singapura**

> Flip the World. Um arremesso. Uma parede. Milímetros decidem.

## 1. Resumo

Schallern é um jogo de arremesso de moedas com física real jogado no navegador: arremesse uma moeda contra uma parede; a moeda cuja borda parar mais perto da parede vence. O jogo é uma versão moderna de um jogo de pátio de escola jogado com o dinheiro do leite na Alemanha dos anos 1980. Uma demo gratuita e jogável, com três arenas e três personagens, está no ar em https://schallern.io/play/.

A **Founder Collection** é uma série planejada de **10.000 colecionáveis digitais na Solana** (moedas e personagens). Os Founder Collectibles são cosméticos: eles mudam a aparência da moeda e do avatar de um jogador, nunca mudam a física, a geometria ou as chances. O mint financia a próxima etapa de desenvolvimento do jogo. Este whitepaper descreve o jogo, a coleção, a mecânica do mint, o uso dos recursos, o roadmap e a equipe, e separa o que está no ar hoje do que está planejado.

## 2. O jogo

**Regra.** Uma parede, uma moeda por arremesso, três rodadas por partida. Após três rodadas, vence a menor soma das distâncias. Um arremesso que nunca toca a parede, sai da pista, voa por cima da parede ou rebate mais de 150 cm é falta e conta a distância máxima publicada.

**Medição.** A distância é medida da borda mais próxima da moeda até a parede depois que a moeda para, quantizada em uma grade milimétrica publicada. A câmera, as sombras e os visuais nunca decidem um vencedor; o resultado da física decide.

**Física.** A moeda é um disco fino e rígido, simulado em um passo fixo de 240 Hz com restituição dependente da velocidade, atrito de rolamento por superfície (asfalto, areia, mármore) e materiais de parede (concreto, arenito, laca). Todos os jogadores de uma rodada arremessam sob a mesma distância, superfície e parede. Os arremessos são determinísticos para a mesma entrada.

**Controles.** Arraste para baixo para dar força, arraste para os lados para a direção, um controle deslizante para o arco; mouse e toque compartilham os mesmos limites de entrada normalizados. A soltura é mostrada em câmera lenta com uma mão de cinco dedos e o flip do polegar.

**Justiça.** Nada que um jogador possa comprar muda massa, diâmetro, atrito, quique ou precisão. A raridade é visual. Esta é a regra fundadora do projeto e se aplica a todos os colecionáveis descritos aqui.

## 3. Situação hoje (o que está no ar, o que não está)

| No ar hoje | Ainda não |
|---|---|
| Demo gratuita no navegador em schallern.io/play/, desktop e celular, sem carteira | Mesas com dinheiro real (somente após licenciamento, auditoria e aprovação, e somente em países permitidos) |
| Três arenas (asfalto de Berlin, areia de Giza, mármore de Vegas), três personagens (NEO, MAYA, BO), oponentes de IA locais | Multiplayer online, torneios, turmas de cidade |
| Chat de feedback com recompensas, Programa de criadores com links de rastreamento, newsletter | Founder Mint na mainnet (o fluxo completo foi ensaiado na devnet da Solana, veja a seção 6) |
| Servidor no Discord com o bot Schallern Rewards | Vinculação de carteira no jogo |

Os pontos da demo não têm valor em dinheiro. Nenhum NFT, token ou pagamento é criado ao jogar a demo.

## 4. A Founder Collection

- **Oferta:** 10.000 colecionáveis, numerados.
- **Temas:** moedas Schallern (materiais, acabamentos, bordas, gravuras, pátina) e personagens no estilo das próprias figuras do jogo; temas de arena opcionais a partir de um catálogo de 48 paredes famosas.
- **Padrão:** Metaplex Core na Solana; cada colecionável é um ativo on-chain em uma coleção verificada com informação de royalties on-chain.
- **Raridade:** um sistema de atributos (cerca de 8 a 12 categorias de atributos, 200 a 300 variantes) dá a cada peça seu próprio ranking de raridade de 1 a 10.000, além de cinco níveis de marketing e um pequeno número de especiais 1/1. A raridade é apenas prestígio.
- **Revelação:** se os compradores escolhem seu nível sem revelação aleatória ou se a arte é revelada em um dia de revelação é uma decisão de produto em aberto; ela será publicada antes da abertura do mint.
- **Direitos sobre a arte:** os holders recebem uma licença pessoal e não exclusiva sobre sua arte; a marca nominativa SCHALLERN permanece com a operadora. O texto final da licença será publicado com os termos do mint.

## 5. O que um Founder recebe, e o que um Founder não recebe

**Recebe:** o colecionável como skin de arremesso no jogo assim que a vinculação de carteira estiver ativa; um selo de Founder com o número do colecionável no perfil de jogador; o cargo de Founder e os canais de holders no Discord; um voto sobre quais arenas e designs de moeda vêm a seguir; acesso antecipado a novas arenas no modo de dinheiro fictício.

**Não recebe:** uma participação na empresa, direito a lucros, distribuições, recompras ou valorização, nem qualquer vantagem de jogo. A Founder Collection é um colecionável, não um produto de investimento. Qualquer financiamento da empresa é uma oferta separada e estruturada à parte (veja a seção 10).

## 6. Mecânica do mint

| Item | Plano |
|---|---|
| Rede e padrão | Solana, Metaplex Core, Core Candy Machine com Candy Guard |
| Níveis e preços | #1–4.000 a 0,5 SOL · #4.001–7.000 a 1 SOL · #7.001–9.000 a 1,5 SOL · #9.001–10.000 a 2 SOL (modelo planejado; as condições finais serão publicadas antes do início) |
| Fases | equipe e OG → Allowlist (garantida, limitada por carteira) → sorteio da lista de espera → público; as datas são anunciadas somente em schallern.io e no canal de anúncios do Discord |
| Limites | limites de mint por carteira por fase; taxa anti-bot; cada transação de mint é construída e coassinada pelo backend da Schallern após verificações de captcha e de frequência |
| Onde | somente em schallern.io; a equipe nunca envia a primeira mensagem e nunca pede frases-semente |
| Tesouraria | os recursos do mint vão diretamente para uma tesouraria multiassinatura (2 de 3) |
| Royalties | 5% de royalties no mercado secundário, gravados na coleção |
| Armazenamento | arte e metadados na Arweave (permanente) |
| Ensaio | o fluxo completo (coleção, quatro máquinas de nível com grupos de fase, provas de Allowlist, assinador no backend, testes de bot e de carga, upload na Arweave, atualização da revelação) foi executado e verificado na devnet da Solana em outubro de 2026 |

Os custos de mint para os compradores são o preço do nível mais as taxas de rede da Solana (cerca de 0,003 SOL por mint).

## 7. Uso dos recursos

Os recursos financiam a próxima etapa de desenvolvimento da Schallern. A alocação planejada cobre: desenvolvimento do jogo (multiplayer, torneios, contas), arte e animação (produção da coleção, novas arenas), infraestrutura e segurança (servidores, RPC, auditorias), comunidade e marketing (Programa de criadores, eventos) e uma reserva operacional. A divisão percentual e os cenários de financiamento mínimo, alvo e ampliado serão publicados antes da abertura do mint. Os royalties do mercado secundário não fazem parte do orçamento base.

## 8. Roadmap

1. **Jogável agora:** demo 3D, três arenas, ajuste fino com o feedback dos jogadores, Programa de criadores, recompensas da demo.
2. **A seguir:** a Founder Collection, crescimento da comunidade, o conceito final do mint e o mint.
3. **Planejado:** partidas online, turmas de cidade, torneios, contas de jogador com painéis de recompensas e afiliados.
4. **Visão:** figuras físicas pessoais, paredes reais, eventos ao vivo.

Datas não são prometidas. Cada etapa é anunciada quando está pronta.

## 9. A economia do jogo (modo com dinheiro real planejado)

O jogo com dinheiro real é uma etapa posterior, licenciada separadamente. O modelo planejado: uma mesa define a aposta (por exemplo, seis jogadores, três rodadas, 1 USDC cada); o vencedor leva o pote menos uma **taxa da casa de 10% sobre o ganho positivo**; apostas e taxas da casa são mantidas estritamente separadas. Criadores que trazem jogadores recebem **10% das taxas da casa ajustadas** dos seus jogadores por 36 meses (veja schallern.io/partners.html). Os Founder Collectibles não têm nenhum papel nessa economia além de serem a skin com a qual um jogador arremessa.

## 10. Financiamento da empresa (separado da coleção)

A Schallern também conversa com investidores privados sobre o financiamento da empresa (mínimo planejado de EUR 20.000). Trata-se de uma oferta separada e privada, com seus próprios termos e documentos, disponível somente após candidatura e análise. Ela nunca é combinada com a Founder Collection, e nada neste whitepaper faz parte dela.

## 11. Equipe e operadora

Operadora até a fundação da empresa do jogo: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Diretor: Kai Zimmer (fundador). Equipe: Kai (fundador), Pallavi (finanças), Riya (operações), Arsh (desenvolvimento), Raj (desenvolvimento). Contato: mint@schallern.io.

## 12. Tecnologia

- **Jogo:** 3D em tempo real com Three.js, física de moeda determinística própria, personagens com rig e animação facial, telemetria para balanceamento. Os resultados nos modos competitivos serão calculados no servidor.
- **Stack do mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave via Irys, Helius RPC, um assinador de backend em Node, multisig Squads.
- **Site:** schallern.io (inglês primeiro, alemão), páginas legais em schallern.io/legal.html.

## 13. Comunidade e recompensas

Discord: https://discord.gg/FpZ5zDjV4. Testadores da demo ganham vouchers de crédito de jogo por feedback qualificado, por entrar no Discord e por níveis na comunidade (com limite por pessoa; resgatáveis somente no lançamento com dinheiro real; não conversíveis em dinheiro). Criadores ganham por meio do Programa de criadores. Regras: schallern.io/legal.html#rewards e #partners.

## 14. Riscos

A Schallern está em desenvolvimento. A demo pode mudar, a coleção pode atrasar, redes blockchain e carteiras podem falhar, colecionáveis digitais podem perder valor, e o jogo com dinheiro real depende de licenças que ainda não existem. Compre somente o que você pode se permitir manter por si só.

## 15. Aviso legal e versões

O arcabouço legal, os termos, a privacidade e os avisos são mantidos pela Culturetek Pte. Ltd. e publicados em https://schallern.io/legal.html. Este documento é informativo, não é uma oferta de venda de valores mobiliários nem aconselhamento de investimento. As versões deste whitepaper são publicadas com a sua data em schallern.io/whitepaper/ e no repositório público vinculado lá.

- v0.1 · 16 de outubro de 2026 · primeiro rascunho de trabalho
