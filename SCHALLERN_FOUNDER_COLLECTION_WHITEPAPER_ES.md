# Schallern — Whitepaper de la Founder Collection

**Versión 0.1 · Borrador de trabajo · 16 de octubre de 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Un tiro. Una pared. Deciden los milímetros.

## 1. Resumen

Schallern es un juego de lanzar monedas con física real que se juega en el navegador: lanza una moneda contra una pared y gana la moneda cuyo canto queda en reposo más cerca de la pared. El juego es una versión moderna de un juego de patio de colegio que se jugaba con el dinero de la leche en la Alemania de los años 80. Una demo gratuita y jugable con tres arenas y tres personajes está disponible en https://schallern.io/play/.

La **Founder Collection** es una serie prevista de **10.000 coleccionables digitales en Solana** (monedas y personajes). Los Founder Collectibles son cosméticos: cambian el aspecto de la moneda y del avatar de un jugador, nunca cambian la física, la geometría ni las probabilidades. El mint financia la siguiente etapa de desarrollo del juego. Este whitepaper describe el juego, la colección, la mecánica del mint, el uso de los fondos, la hoja de ruta y el equipo, y separa lo que está activo hoy de lo que está previsto.

## 2. El juego

**Regla.** Una pared, una moneda por tiro, tres rondas por partida. Tras tres rondas gana la menor suma de distancias. Un tiro que nunca toca la pared, sale del carril, vuela por encima de la pared o rebota más de 150 cm es falta y cuenta con la distancia máxima publicada.

**Medición.** La distancia se mide desde el canto más cercano de la moneda hasta la pared una vez que la moneda se ha detenido, cuantizada a una cuadrícula milimétrica publicada. La cámara, las sombras y los efectos visuales nunca deciden un ganador; lo decide el resultado de la física.

**Física.** La moneda es un disco delgado rígido simulado a un paso fijo de 240 Hz con restitución dependiente de la velocidad, fricción de rodadura por superficie (asfalto, arena, mármol) y materiales de pared (hormigón, arenisca, laca). Todos los jugadores de una ronda lanzan con la misma distancia, superficie y pared. Los tiros son deterministas para la misma entrada.

**Controles.** Arrastra hacia abajo para la fuerza, hacia los lados para la dirección, un control deslizante para el arco; ratón y táctil comparten los mismos límites de entrada normalizados. El lanzamiento se muestra a cámara lenta con una mano de cinco dedos y un golpe de pulgar.

**Equidad.** Nada que un jugador pueda comprar cambia la masa, el diámetro, la fricción, el rebote ni la precisión. La rareza es visual. Esta es la regla fundacional del proyecto y se aplica a cada coleccionable descrito aquí.

## 3. Estado actual (qué está activo y qué no)

| Activo hoy | Todavía no |
|---|---|
| Demo gratuita en el navegador en schallern.io/play/, escritorio y móvil, sin wallet | Mesas con dinero real (solo tras licencia, auditoría y aprobación, y solo en países permitidos) |
| Tres arenas (asfalto de Berlin, arena de Giza, mármol de Vegas), tres personajes (NEO, MAYA, BO), rivales de IA locales | Multijugador online, torneos, crews de ciudad |
| Chat de feedback con recompensas, programa de creadores con enlaces de seguimiento, newsletter | Founder Mint en mainnet (el flujo completo se ha ensayado en la devnet de Solana, ver sección 6) |
| Servidor de Discord con el bot Schallern Rewards | Vinculación de wallet en el juego |

Los puntos de la demo no tienen valor en efectivo. Jugar la demo no crea ningún NFT, token ni pago.

## 4. La Founder Collection

- **Suministro:** 10.000 coleccionables, numerados.
- **Motivos:** monedas Schallern (materiales, acabados, cantos, grabados, pátina) y personajes al estilo de las propias figuras del juego; temas de arena opcionales de un catálogo de 48 paredes famosas.
- **Estándar:** Metaplex Core en Solana; cada coleccionable es un activo on-chain dentro de una colección verificada con información de regalías on-chain.
- **Rareza:** un sistema de rasgos (unas 8 a 12 categorías de rasgos, 200 a 300 variantes) da a cada pieza su propio rango de rareza del 1 al 10.000, además de cinco niveles de marketing y un pequeño número de piezas únicas 1/1. La rareza es solo prestigio.
- **Reveal:** si los compradores eligen su nivel sin reveal aleatorio o si el artwork se revela en un día de reveal es una decisión de producto abierta; se publica antes de que abra el mint.
- **Derechos sobre el artwork:** los holders reciben una licencia personal y no exclusiva sobre su artwork; la marca denominativa SCHALLERN sigue siendo de la operadora. El texto final de la licencia se publica con las condiciones del mint.

## 5. Qué recibe un Founder y qué no recibe

**Recibe:** el coleccionable como skin de lanzamiento en el juego en cuanto la vinculación de wallet esté activa; una insignia Founder con el número del coleccionable en el perfil de jugador; el rol Founder y canales para holders en Discord; un voto sobre qué arenas y diseños de moneda llegan después; acceso anticipado a nuevas arenas en modo de dinero ficticio.

**No recibe:** una participación en la empresa, un derecho a beneficios, repartos, recompras o revalorización, ni ninguna ventaja en el juego. La Founder Collection es un coleccionable, no un producto de inversión. Cualquier financiación de la empresa es una oferta aparte, estructurada por separado (ver sección 10).

## 6. Mecánica del mint

| Elemento | Plan |
|---|---|
| Cadena y estándar | Solana, Metaplex Core, Core Candy Machine con Candy Guard |
| Niveles y precios | #1–4.000 a 0,5 SOL · #4.001–7.000 a 1 SOL · #7.001–9.000 a 1,5 SOL · #9.001–10.000 a 2 SOL (modelo previsto; las condiciones definitivas se publican antes del inicio) |
| Fases | equipo y OG → Allowlist (garantizada, limitada por wallet) → sorteo de la lista de espera → público; las fechas se anuncian solo en schallern.io y en el canal de anuncios de Discord |
| Límites | límites de mint por wallet y por fase; impuesto antibots; cada transacción de mint la construye y cofirma el backend de Schallern tras comprobaciones de captcha y de frecuencia |
| Dónde | solo en schallern.io; el equipo nunca escribe primero y nunca pide frases semilla |
| Tesorería | los ingresos del mint van directamente a una tesorería multifirma (2 de 3) |
| Regalías | 5 % de regalías en el mercado secundario, inscritas en la colección |
| Almacenamiento | artwork y metadatos en Arweave (permanente) |
| Ensayo | el flujo completo (colección, cuatro máquinas por nivel con grupos de fase, pruebas de Allowlist, firmante de backend, pruebas de bots y de carga, subida a Arweave, actualización del reveal) se ha ejecutado y verificado en la devnet de Solana en octubre de 2026 |

Los costes del mint para los compradores son el precio del nivel más las comisiones de red de Solana (unos 0,003 SOL por mint).

## 7. Uso de los fondos

Los fondos financian la siguiente etapa de desarrollo de Schallern. La asignación prevista cubre: desarrollo del juego (multijugador, torneos, cuentas), arte y animación (producción de la colección, nuevas arenas), infraestructura y seguridad (servidores, RPC, auditorías), comunidad y marketing (programa de creadores, eventos) y una reserva operativa. El reparto porcentual y los escenarios de financiación mínima, objetivo y ampliada se publican antes de que abra el mint. Las regalías del mercado secundario no forman parte del presupuesto base.

## 8. Hoja de ruta

1. **Jugable ya:** demo 3D, tres arenas, ajuste fino con el feedback de los jugadores, programa de creadores, recompensas de la demo.
2. **Siguiente:** la Founder Collection, crecimiento de la comunidad, el concepto final del mint y el mint.
3. **Previsto:** partidas online, crews de ciudad, torneos, cuentas de jugador con recompensas y paneles de afiliados.
4. **Visión:** figuras físicas personales, paredes reales, eventos en vivo.

No se prometen fechas. Cada paso se anuncia cuando está listo.

## 9. La economía del juego (modo de dinero real previsto)

El juego con dinero real es una etapa posterior, con licencia aparte. El modelo previsto: una mesa fija la apuesta (por ejemplo, seis jugadores, tres rondas, 1 USDC cada uno); el ganador se lleva el bote menos una **comisión de la casa del 10 % sobre la ganancia positiva**; las apuestas y las comisiones de la casa se mantienen estrictamente separadas. Los creadores que traen jugadores reciben el **10 % de las comisiones de la casa ajustadas** de sus jugadores durante 36 meses (ver schallern.io/partners.html). Los Founder Collectibles no desempeñan ningún papel en esta economía más allá de ser la skin con la que lanza un jugador.

## 10. Financiación de la empresa (separada de la colección)

Schallern también habla con inversores privados sobre la financiación de la empresa (mínimo previsto de 20.000 EUR). Es una oferta privada aparte, con sus propias condiciones y documentos, disponible solo tras solicitud y revisión. Nunca se combina con la Founder Collection, y nada de este whitepaper forma parte de ella.

## 11. Equipo y operadora

Operadora hasta que se funde la sociedad del juego: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Director: Kai Zimmer (fundador). Equipo: Kai (fundador), Pallavi (finanzas), Riya (operaciones), Arsh (desarrollo), Raj (desarrollo). Contacto: mint@schallern.io.

## 12. Tecnología

- **Juego:** 3D en tiempo real con Three.js, física de moneda determinista propia, personajes con rigging y animación facial, telemetría para el balanceo. Los resultados en modos competitivos se calcularán en el servidor.
- **Stack del mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave vía Irys, RPC de Helius, un firmante de backend en Node, multifirma Squads.
- **Sitio web:** schallern.io (primero en inglés, alemán), páginas legales en schallern.io/legal.html.

## 13. Comunidad y recompensas

Discord: https://discord.gg/FpZ5zDjV4. Los testers de la demo ganan vales de crédito de juego por feedback cualificado, por unirse a Discord y por niveles de comunidad (con tope por persona; canjeables solo en el lanzamiento con dinero real; no convertibles en efectivo). Los creadores ganan a través del programa de creadores. Reglas: schallern.io/legal.html#rewards y #partners.

## 14. Riesgos

Schallern está en desarrollo. La demo puede cambiar, la colección puede retrasarse, las redes blockchain y las wallets pueden fallar, los coleccionables digitales pueden perder valor y el juego con dinero real depende de licencias que todavía no existen. Compra solo lo que puedas permitirte conservar por sí mismo.

## 15. Aviso legal y versiones

El marco legal, las condiciones, la privacidad y los disclaimers los mantiene Culturetek Pte. Ltd. y se publican en https://schallern.io/legal.html. Este documento es informativo, no es una oferta de venta de valores ni asesoramiento de inversión. Las versiones de este whitepaper se publican con su fecha en schallern.io/whitepaper/ y en el repositorio público enlazado allí.

- v0.1 · 16 de octubre de 2026 · primer borrador de trabajo
