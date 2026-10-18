# Schallern — Whitepaper de la Founder Collection

**Versión 0.2 · Borrador de trabajo · 18 de octubre de 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Un tiro. Una pared. Deciden los milímetros.

## 1. Resumen

Schallern es un juego de lanzar monedas, calibrado físicamente, que se juega en el navegador: lanza una moneda hacia una pared; gana la moneda cuyo canto más cercano queda en reposo más cerca de la pared. El juego es una versión moderna de un juego de patio de colegio que se jugaba con el dinero de la leche en la Alemania de los años 80. Una demo gratuita y jugable con tres arenas y tres personajes está disponible en https://schallern.io/play/.

La **Founder Collection** es una serie prevista de **10.000 coleccionables digitales en Solana** (monedas y personajes). Los Founder Collectibles son cosméticos: cambian el aspecto de la moneda y del avatar de un jugador, nunca cambian la física, la geometría ni las probabilidades. El mint financia la siguiente etapa de desarrollo del juego. Este whitepaper describe el juego, la colección, la mecánica del mint, el uso de los fondos, la hoja de ruta y el equipo, y separa lo que está activo hoy de lo que está previsto.

## 2. El juego

**Regla.** Una pared, una moneda por tiro, tres rondas por partida; gana la menor suma. Cada tiro puntúa la distancia en milímetros desde el canto más cercano de la moneda hasta la pared, una vez que la moneda se ha detenido. La moneda **no** tiene que tocar la pared. Una moneda que queda apoyada contra la pared (leaner) puntúa 0 mm. La cámara, las sombras y los efectos visuales nunca deciden un ganador; lo decide el resultado de la física.

**Falta y tiros no válidos.** La única falta es una moneda que vuela por encima de la pared. Un tiro no es válido si el primer contacto de la moneda con el suelo queda a menos de 2 m de la línea de tiro (caer justo sobre la línea de 2 m es válido). Una falta o un tiro no válido cuenta con la distancia de la ronda; ningún tiro válido puede puntuar peor.

**Tarjeta de ronda.** Antes de cada ronda, una tarjeta muestra las condiciones, iguales para todos los jugadores: la distancia de tiro entre 6 y 10 m en valores no redondos (por ejemplo, 7,43 m), la moneda de la ronda, tomada de un catálogo de monedas reales en su tamaño real, y las zonas visibles del suelo y de la pared (por ejemplo, grietas, grava, zonas lisas o placas metálicas), así como la pendiente.

**Física.** La moneda es un disco delgado con datos de monedas reales, simulado con fricción, resistencia a la rodadura y rebote por superficie (asfalto, arena, mármol) y por material de pared. El modelo está calibrado físicamente a partir de mediciones publicadas; la calibración con tiros reales filmados sigue pendiente, por eso todavía no lo llamamos física real. La simulación es determinista: la misma entrada da el mismo resultado en cualquier dispositivo.

**Controles.** Cuatro estilos de tiro: Deslizador (bajo y plano), Medio arco, Globo alto y Golpe a la pared, cada uno con su propio rango de velocidad y de arco. Mantén pulsado y tira hacia atrás para la fuerza y la dirección, curva el gesto para dar efecto lateral y suelta mientras el anillo de lanzamiento se encoge y se cierra; el timing y el pulso firme deciden la calidad del lanzamiento. Ratón y táctil usan la misma entrada normalizada.

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
- **Motivos:** monedas Schallern en ocho categorías de rasgos visibles: nivel, material, acabado, canto, motivo (incluidos los personajes del juego), inscripción, fondo (incluidas 48 paredes famosas) y efecto.
- **Estándar:** Metaplex Core en Solana; cada coleccionable es un activo on-chain dentro de una colección verificada con información de regalías on-chain.
- **Rareza:** 8 categorías de rasgos con 129 valores; cada pieza tiene todas las categorías y su propio rango de rareza. Niveles: 11 piezas únicas (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon y 5.000 Common. La rareza es solo prestigio visual.
- **Asignación aleatoria y reveal:** los compradores no eligen el artwork, la rareza ni el nivel. Hasta que se agote la colección, todos los coleccionables muestran el mismo placeholder. Antes de que abra el mint se publica un hash de procedencia de la colección completa y ordenada, que queda guardado on-chain. Una vez agotada, el desplazamiento inicial se toma de un slot futuro de Solana anunciado de antemano, de modo que nadie, ni siquiera el equipo, puede decidir quién recibe qué pieza. Cualquiera puede comprobar el resultado con el hash publicado.
- **Derechos sobre el artwork:** los holders pueden usar comercialmente el artwork de su coleccionable. La marca SCHALLERN (nombre y logotipo) queda excluida y sigue siendo de la operadora. El texto final de la licencia se publica con las condiciones del mint.

## 5. Qué recibe un Founder y qué no recibe

**Recibe:** el coleccionable como skin de lanzamiento en el juego en cuanto la vinculación de wallet esté activa; una insignia Founder con el número del coleccionable en el perfil de jugador; el rol Founder y canales para holders en Discord; un voto sobre qué arenas y diseños de moneda llegan después; acceso anticipado a nuevas arenas en modo de dinero ficticio; el derecho a usar comercialmente el artwork (excepto la marca SCHALLERN).

**No recibe:** una participación en la empresa, un derecho a beneficios, repartos, recompras o revalorización, ni ninguna ventaja en el juego. La Founder Collection es un coleccionable, no un producto de inversión. Cualquier financiación de la empresa es una oferta aparte, estructurada por separado (ver sección 10).

## 6. Mecánica del mint

| Elemento | Plan |
|---|---|
| Cadena y estándar | Solana, Metaplex Core, una sola Core Candy Machine con Candy Guard |
| Escalones de precio | los fija el número de piezas vendidas, no los elige el comprador: #1–4.000 a 0,5 SOL · #4.001–7.000 a 1 SOL · #7.001–9.000 a 1,5 SOL · #9.001–10.000 a 2 SOL. Quien compra antes paga menos; una compra que cruza un escalón se cobra pieza por pieza (modelo previsto; las condiciones definitivas se publican antes del inicio) |
| Asignación | artwork y rareza aleatorios para las 10.000 piezas desde una sola Candy Machine, revelados cuando se agota la colección (ver sección 4) |
| Fases | inicio el **11 de noviembre de 2026, 11:11 SGT (03:11 UTC)**; OG → Allowlist → público; la Allowlist da acceso antes. Las fechas y cualquier cambio se anuncian solo en schallern.io y en los canales oficiales de Discord y Telegram |
| Límites | sin límites por wallet en ninguna fase; protección antibots mediante captcha, comprobaciones de frecuencia e impuesto antibots; cada transacción de mint la construye y cofirma el backend de Schallern |
| Dónde | solo en schallern.io; el equipo nunca escribe primero y nunca pide frases semilla |
| Disponibilidad | el mint solo tiene restricciones geográficas donde lo exigen las condiciones de nuestros proveedores de servicios |
| Tesorería | los ingresos del mint se pagan on-chain a una bóveda multisig 2 de 3 (Squads v4) de la operadora; ninguna clave por sí sola puede mover los fondos |
| Regalías | 5 % de regalías en el mercado secundario, inscritas en la colección |
| Almacenamiento | artwork y metadatos en Arweave (permanente); el artwork final se sube en el reveal |
| Ensayo | el flujo completo (colección, una sola Candy Machine con placeholder y hash de procedencia on-chain, grupos de fase y de escalón de precio, firmante de backend, comprobaciones geográficas y de sanciones, pruebas de bots y de carga, reveal a partir de un slot de Solana, verificación pública) se ha ejecutado y verificado en la devnet de Solana en octubre de 2026 |

Los costes del mint para los compradores son el precio del escalón vigente más las comisiones de red de Solana (unos 0,003 SOL por mint).

## 7. Uso de los fondos

Los fondos financian la siguiente etapa de desarrollo de Schallern. La asignación prevista cubre: desarrollo del juego (multijugador, torneos, cuentas), arte y animación (producción de la colección, nuevas arenas), infraestructura y seguridad (servidores, RPC, auditorías), comunidad y marketing (programa de creadores, eventos) y una reserva operativa. El reparto porcentual y los escenarios de financiación mínima, objetivo y ampliada se publican antes de que abra el mint. Las regalías del mercado secundario no forman parte del presupuesto base.

## 8. Hoja de ruta

1. **Jugable ya:** demo 3D, tres arenas, ajuste fino con el feedback de los jugadores, programa de creadores, recompensas de la demo.
2. **Siguiente:** la Founder Collection, crecimiento de la comunidad, el concepto final del mint y el mint.
3. **Previsto:** partidas online, crews de ciudad, torneos, cuentas de jugador con recompensas y paneles de afiliados.
4. **Visión:** figuras físicas personales, paredes reales, eventos en vivo.

Salvo el inicio del Founder Mint (11 de noviembre de 2026, 11:11 SGT), no se prometen fechas. Cada paso se anuncia cuando está listo.

## 9. La economía del juego (modo de dinero real previsto)

El juego con dinero real es una etapa posterior, con licencia aparte. El modelo previsto: una mesa fija la apuesta (por ejemplo, seis jugadores, tres rondas, 1 USDC cada uno); el ganador se lleva el bote menos una **comisión de la casa del 10 % sobre la ganancia positiva**; las apuestas y las comisiones de la casa se mantienen estrictamente separadas. Los creadores que traen jugadores reciben el **10 % de las comisiones de la casa ajustadas** de sus jugadores durante 36 meses (ver schallern.io/partners.html). Los Founder Collectibles no desempeñan ningún papel en esta economía más allá de ser la skin con la que lanza un jugador.

## 10. Financiación de la empresa (separada de la colección)

Schallern también habla con inversores privados sobre la financiación de la empresa (mínimo previsto de 20.000 EUR). Es una oferta privada aparte, con sus propias condiciones y documentos, disponible solo tras solicitud y revisión. Nunca se combina con la Founder Collection, y nada de este whitepaper forma parte de ella.

## 11. Equipo y operadora

Operadora hasta que se funde la sociedad del juego: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Director: Kai Zimmer (fundador). Equipo: Kai (fundador), Pallavi (finanzas), Riya (operaciones), Arsh (desarrollo), Raj (desarrollo). Contacto: mint@schallern.io.

## 12. Tecnología

- **Juego:** 3D en tiempo real con Three.js, física de moneda propia, determinista y calibrada físicamente, personajes con rigging y animación facial, telemetría para el balanceo. Los resultados en modos competitivos se calcularán en el servidor.
- **Stack del mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, RPC de Helius, un firmante de backend en Node, una bóveda multisig Squads v4 para los ingresos.
- **Sitio web:** schallern.io (primero en inglés, alemán), páginas legales en schallern.io/legal.html.

## 13. Comunidad y recompensas

Discord: https://discord.gg/FpZ5zDjV4. Los testers de la demo ganan vales de crédito de juego por feedback cualificado, por unirse a Discord y por niveles de comunidad (con tope por persona; canjeables solo en el lanzamiento con dinero real; no convertibles en efectivo). Los creadores ganan a través del programa de creadores. Reglas: schallern.io/legal.html#rewards y #partners.

## 14. Riesgos

Schallern está en desarrollo. La demo puede cambiar, la colección puede retrasarse, las redes blockchain y las wallets pueden fallar, los coleccionables digitales pueden perder valor y el juego con dinero real depende de licencias que todavía no existen. Compra solo lo que puedas permitirte conservar por sí mismo.

## 15. Aviso legal y versiones

El marco legal, las condiciones, la privacidad y los disclaimers los mantiene Culturetek Pte. Ltd. y se publican en https://schallern.io/legal.html. Este documento es informativo, no es una oferta de venta de valores ni asesoramiento de inversión. Las versiones de este whitepaper se publican con su fecha en schallern.io/whitepaper/ y en el repositorio público enlazado allí.

- v0.1 · 16 de octubre de 2026 · primer borrador de trabajo
- v0.2 · 18 de octubre de 2026 · reglas de juego de la demo V04 (no hace falta tocar la pared, única falta = por encima de la pared, línea de contacto de 2 m, tarjeta de ronda, cuatro estilos de tiro), formulación "calibrado físicamente", asignación aleatoria con rarezas y reveal tras agotarse la colección, una sola Candy Machine, escalones de precio según el número vendido, sin límites por wallet, sistema de rasgos y número de piezas por nivel, uso comercial del artwork, restricción geográfica
