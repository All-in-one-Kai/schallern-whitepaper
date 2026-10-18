# Schallern — Whitepaper da Founder Collection

**Versão 0.2 · Rascunho de trabalho · 18 de outubro de 2026 · Culturetek Pte. Ltd., Singapura**

> Flip the World. Um arremesso. Uma parede. Milímetros decidem.

## 1. Resumo

Schallern é um jogo de arremesso de moedas calibrado fisicamente, jogado no navegador: arremesse uma moeda em direção a uma parede; a moeda cuja borda mais próxima parar mais perto da parede vence. O jogo é uma versão moderna de um jogo de pátio de escola jogado com o dinheiro do leite na Alemanha dos anos 1980. Uma demo gratuita e jogável, com três arenas e três personagens, está no ar em https://schallern.io/play/.

A **Founder Collection** é uma série planejada de **10.000 colecionáveis digitais na Solana** (moedas e personagens). Os Founder Collectibles são cosméticos: eles mudam a aparência da moeda e do avatar de um jogador, nunca mudam a física, a geometria ou as chances. O mint financia a próxima etapa de desenvolvimento do jogo. Este whitepaper descreve o jogo, a coleção, a mecânica do mint, o uso dos recursos, o roadmap e a equipe, e separa o que está no ar hoje do que está planejado.

## 2. O jogo

**Regra.** Uma parede, uma moeda por arremesso, três rodadas por partida; vence o menor total. Cada arremesso vale a distância, em milímetros, da borda mais próxima da moeda até a parede, depois que a moeda para. A moeda **não** precisa tocar a parede. Uma moeda que fica encostada na parede (leaner) vale 0 mm. A câmera, as sombras e os visuais nunca decidem um vencedor; o resultado da física decide.

**Falta e arremessos inválidos.** A única falta é uma moeda que voa por cima da parede. Um arremesso é inválido se o primeiro contato da moeda com o chão ficar a menos de 2 m depois da linha de arremesso (cair exatamente na linha de 2 m é válido). Uma falta ou um arremesso inválido conta a distância da rodada; nenhum arremesso válido pode pontuar pior do que isso.

**Carta da rodada.** Antes de cada rodada, uma carta mostra as condições, iguais para todos os jogadores: a distância de arremesso entre 6 e 10 m, em valores quebrados (por exemplo, 7,43 m), a moeda da rodada, tirada de um catálogo de moedas reais em seus tamanhos reais, e as áreas visíveis do chão e da parede (por exemplo, rachaduras, cascalho, pontos lisos ou chapas de metal), além da inclinação.

**Física.** A moeda é um disco fino com dados de moedas reais, simulado com atrito, resistência ao rolamento e quique por superfície (asfalto, areia, mármore) e por material de parede. O modelo é calibrado fisicamente com base em medições publicadas; a calibração com arremessos reais filmados ainda está pendente, por isso ainda não falamos em física real. A simulação é determinística: a mesma entrada gera o mesmo resultado em qualquer dispositivo.

**Controles.** Quatro estilos de arremesso: Deslizante (baixo e rasante), Meio arco, Balão alto e Tapa na parede, cada um com sua própria faixa de velocidade e de arco. Pressione e puxe para trás para definir força e direção, curve o gesto para dar efeito lateral e solte enquanto o anel de soltura se fecha; o timing e a mão firme decidem a qualidade da soltura. Mouse e toque usam a mesma entrada normalizada.

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
- **Temas:** moedas Schallern em oito categorias de atributos visíveis: nível, material, acabamento, borda, motivo (incluindo os personagens do jogo), inscrição, fundo (incluindo 48 paredes famosas) e efeito.
- **Padrão:** Metaplex Core na Solana; cada colecionável é um ativo on-chain em uma coleção verificada com informação de royalties on-chain.
- **Raridade:** 8 categorias de atributos com 129 valores; cada peça tem todas as categorias e seu próprio ranking de raridade. Níveis: 11 peças únicas (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon e 5.000 Common. A raridade é apenas prestígio visual.
- **Atribuição aleatória e revelação:** os compradores não escolhem a arte, a raridade nem o nível. Até a coleção esgotar, todos os colecionáveis mostram a mesma imagem provisória. Antes da abertura do mint, um hash de proveniência da coleção completa e ordenada é publicado e gravado on-chain. Depois que a coleção esgota, o deslocamento inicial é tirado de um slot futuro da Solana anunciado com antecedência, de modo que ninguém, nem mesmo a equipe, consegue direcionar quem recebe qual peça. Qualquer pessoa pode conferir o resultado com o hash publicado.
- **Direitos sobre a arte:** os holders podem usar comercialmente a arte do seu colecionável. A marca SCHALLERN (nome e logotipo) fica excluída e permanece com a operadora. O texto final da licença será publicado com os termos do mint.

## 5. O que um Founder recebe, e o que um Founder não recebe

**Recebe:** o colecionável como skin de arremesso no jogo assim que a vinculação de carteira estiver ativa; um selo de Founder com o número do colecionável no perfil de jogador; o cargo de Founder e os canais de holders no Discord; um voto sobre quais arenas e designs de moeda vêm a seguir; acesso antecipado a novas arenas no modo de dinheiro fictício; o direito de usar a arte comercialmente (exceto a marca SCHALLERN).

**Não recebe:** uma participação na empresa, direito a lucros, distribuições, recompras ou valorização, nem qualquer vantagem de jogo. A Founder Collection é um colecionável, não um produto de investimento. Qualquer financiamento da empresa é uma oferta separada e estruturada à parte (veja a seção 10).

## 6. Mecânica do mint

| Item | Plano |
|---|---|
| Rede e padrão | Solana, Metaplex Core, uma única Core Candy Machine com Candy Guard |
| Faixas de preço | definidas pela quantidade vendida, não escolhidas pelo comprador: #1–4.000 a 0,5 SOL · #4.001–7.000 a 1 SOL · #7.001–9.000 a 1,5 SOL · #9.001–10.000 a 2 SOL. Quem compra antes paga menos; uma compra que atravessa uma faixa é cobrada por peça (modelo planejado; as condições finais serão publicadas antes do início) |
| Atribuição | arte e raridade aleatórias para todos os 10.000 a partir de uma única Candy Machine, reveladas depois que a coleção esgotar (veja a seção 4) |
| Fases | início em **11 de novembro de 2026, 11:11 SGT (03:11 UTC)**; OG → Allowlist → público; a Allowlist dá acesso antecipado. As datas e eventuais mudanças são anunciadas somente em schallern.io e nos canais oficiais do Discord e do Telegram |
| Limites | sem limites por carteira em nenhuma fase; proteção anti-bot com captcha, verificações de frequência e taxa anti-bot; cada transação de mint é construída e coassinada pelo backend da Schallern |
| Onde | somente em schallern.io; a equipe nunca envia a primeira mensagem e nunca pede frases-semente |
| Disponibilidade | o mint só tem restrição geográfica onde os termos dos nossos prestadores de serviço exigem |
| Tesouraria | os recursos do mint são pagos on-chain em um cofre multisig 2 de 3 (Squads v4) da operadora; nenhuma chave sozinha consegue movimentar os fundos |
| Royalties | 5% de royalties no mercado secundário, gravados na coleção |
| Armazenamento | arte e metadados na Arweave (permanente); a arte final é enviada na revelação |
| Ensaio | o fluxo completo (coleção, uma única Candy Machine com imagem provisória e hash de proveniência on-chain, grupos de fase e de faixa de preço, assinador no backend, verificações geográficas e de sanções, testes de bot e de carga, revelação a partir de um slot da Solana, verificação pública) foi executado e verificado na devnet da Solana em outubro de 2026 |

Os custos de mint para os compradores são o preço da faixa vigente mais as taxas de rede da Solana (cerca de 0,003 SOL por mint).

## 7. Uso dos recursos

Os recursos financiam a próxima etapa de desenvolvimento da Schallern. A alocação planejada cobre: desenvolvimento do jogo (multiplayer, torneios, contas), arte e animação (produção da coleção, novas arenas), infraestrutura e segurança (servidores, RPC, auditorias), comunidade e marketing (Programa de criadores, eventos) e uma reserva operacional. A divisão percentual e os cenários de financiamento mínimo, alvo e ampliado serão publicados antes da abertura do mint. Os royalties do mercado secundário não fazem parte do orçamento base.

## 8. Roadmap

1. **Jogável agora:** demo 3D, três arenas, ajuste fino com o feedback dos jogadores, Programa de criadores, recompensas da demo.
2. **A seguir:** a Founder Collection, crescimento da comunidade, o conceito final do mint e o mint.
3. **Planejado:** partidas online, turmas de cidade, torneios, contas de jogador com painéis de recompensas e afiliados.
4. **Visão:** figuras físicas pessoais, paredes reais, eventos ao vivo.

Exceto o início do Founder Mint (11 de novembro de 2026, 11:11 SGT), datas não são prometidas. Cada etapa é anunciada quando está pronta.

## 9. A economia do jogo (modo com dinheiro real planejado)

O jogo com dinheiro real é uma etapa posterior, licenciada separadamente. O modelo planejado: uma mesa define a aposta (por exemplo, seis jogadores, três rodadas, 1 USDC cada); o vencedor leva o pote menos uma **taxa da casa de 10% sobre o ganho positivo**; apostas e taxas da casa são mantidas estritamente separadas. Criadores que trazem jogadores recebem **10% das taxas da casa ajustadas** dos seus jogadores por 36 meses (veja schallern.io/partners.html). Os Founder Collectibles não têm nenhum papel nessa economia além de serem a skin com a qual um jogador arremessa.

## 10. Financiamento da empresa (separado da coleção)

A Schallern também conversa com investidores privados sobre o financiamento da empresa (mínimo planejado de EUR 20.000). Trata-se de uma oferta separada e privada, com seus próprios termos e documentos, disponível somente após candidatura e análise. Ela nunca é combinada com a Founder Collection, e nada neste whitepaper faz parte dela.

## 11. Equipe e operadora

Operadora até a fundação da empresa do jogo: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Diretor: Kai Zimmer (fundador). Equipe: Kai (fundador), Pallavi (finanças), Riya (operações), Arsh (desenvolvimento), Raj (desenvolvimento). Contato: mint@schallern.io.

## 12. Tecnologia

- **Jogo:** 3D em tempo real com Three.js, física de moeda própria, determinística e calibrada fisicamente, personagens com rig e animação facial, telemetria para balanceamento. Os resultados nos modos competitivos serão calculados no servidor.
- **Stack do mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, um assinador de backend em Node, um cofre multisig Squads v4 para os recursos.
- **Site:** schallern.io (inglês primeiro, alemão), páginas legais em schallern.io/legal.html.

## 13. Comunidade e recompensas

Discord: https://discord.gg/FpZ5zDjV4. Testadores da demo ganham vouchers de crédito de jogo por feedback qualificado, por entrar no Discord e por níveis na comunidade (com limite por pessoa; resgatáveis somente no lançamento com dinheiro real; não conversíveis em dinheiro). Criadores ganham por meio do Programa de criadores. Regras: schallern.io/legal.html#rewards e #partners.

## 14. Riscos

A Schallern está em desenvolvimento. A demo pode mudar, a coleção pode atrasar, redes blockchain e carteiras podem falhar, colecionáveis digitais podem perder valor, e o jogo com dinheiro real depende de licenças que ainda não existem. Compre somente o que você pode se permitir manter por si só.

## 15. Aviso legal e versões

O arcabouço legal, os termos, a privacidade e os avisos são mantidos pela Culturetek Pte. Ltd. e publicados em https://schallern.io/legal.html. Este documento é informativo, não é uma oferta de venda de valores mobiliários nem aconselhamento de investimento. As versões deste whitepaper são publicadas com a sua data em schallern.io/whitepaper/ e no repositório público vinculado lá.

- v0.1 · 16 de outubro de 2026 · primeiro rascunho de trabalho
- v0.2 · 18 de outubro de 2026 · regras de jogo da demo V04 (não é preciso tocar a parede, única falta = por cima da parede, linha de contato de 2 m, carta da rodada, quatro estilos de arremesso), expressão "calibrado fisicamente", atribuição aleatória com raridades e revelação após a coleção esgotar, uma única Candy Machine, faixas de preço pela quantidade vendida, sem limites por carteira, sistema de atributos e quantidade por nível, uso comercial da arte, restrição geográfica
