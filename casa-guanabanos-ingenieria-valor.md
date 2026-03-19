# Casa Guanábanos — Ingeniería de Valor y Recomendaciones de Especificación

> **Objetivo**: Maximizar la calidad percibida y el valor de reventa de una residencia de alta gama en Cuajimalpa, eliminando gastos innecesarios y haciendo sustituciones inteligentes donde el costo no equivale a calidad.
>
> **Marco de evaluación**: Cada recomendación se clasifica:
> - **Mantener** = La especificación actual es correcta. No cambiar.
> - **Mejorar** = Sub-especificado para el mercado. Invertir aquí o arrepentirse después.
> - **Reducir** = Sobre-especificado. Ahorrar dinero sin perder calidad.
> - **Agregar** = No existe en los planos. Falta crítica para alta gama.

---

## Resumen Ejecutivo

El juego de planos MEP es ingeniería sólida — bien organizado, completo, y ya incluye varias decisiones inteligentes de diseño (cable neutro en cada apagador, captación pluvial, solar, contactos regulados). Pero está diseñado como un paquete de instalación MEP, no como una experiencia de vida de alta gama. Hay brechas significativas en sistemas de confort, infraestructura de domótica, y varias áreas donde el dinero puede reasignarse de subsistemas sobre-ingenierizados a características que realmente impactan la calidad de vida y el valor de reventa.

**Impacto neto estimado de todas las recomendaciones:**

| Categoría | Ahorro | Gasto Adicional | Neto |
|-----------|--------|-----------------|------|
| Optimización eléctrica | ~$3,000–5,000 USD | — | Ahorro |
| Plataforma domótica (dimensionamiento correcto) | ~$40,000–80,000 USD | — | Ahorro |
| Sistemas de agua (mejora + recirculación) | — | ~$5,500–11,000 USD | Gasto |
| Seguridad (mejora) | — | ~$5,000–10,000 USD | Gasto |
| Carga de vehículo eléctrico (agregar) | — | ~$1,500–3,000 USD | Gasto |
| Red / AV (dimensionamiento correcto) | ~$15,000–25,000 USD | — | Ahorro |

**Conclusión**: Los ahorros en domótica y AV por sí solos pueden financiar cada mejora listada abajo y aún sobrar dinero.

---

## 1. Eléctrica — Mayormente Mantener, Dos Correcciones

### 1a. Alimentadores Principales: **Mantener**

La mezcla de cobre THHW-LS para circuitos derivados y aluminio MC4 para alimentadores principales (CED-02, 10, 11, 12, 19) es la decisión correcta. Los alimentadores de aluminio en estos calibres (1/0 a 350 KCM) cumplen norma, son confiables, y ahorran ~40% vs. cobre en esos tamaños. Si alguien sugiere usar todo cobre "por calidad," recházalo — la calidad está en las conexiones, no en el metal del conductor para alimentadores.

**Costo protegido: ~$3,000–5,000 USD ahorrados vs. alimentadores todo cobre.**

### 1b. CED-17 y CED-18: **Mejorar**

Estos dos circuitos están sub-especificados:
- CED-17: #12 AWG, 27m, 8.12A → **2.08% caída de tensión**
- CED-18: #12 AWG, 27m, 10.59A → **2.72% caída de tensión**

La NOM-001-SEDE permite 3% para circuitos derivados, pero la mejor práctica para residencial de alta gama es <2%. Al 2.72%, CED-18 causará atenuación notable en circuitos de iluminación y rendimiento reducido en equipos sensibles.

**Recomendación**: Subir ambos a #10 AWG. Misma tubería (21mm es suficiente), diferencia mínima de costo (~$200–400 USD en cable), y la caída de tensión baja a ~1.3% y ~1.7% respectivamente.

### 1c. Contactos Regulados (CR): **Mejorar**

Actualmente solo en PB y S1. Para una casa de alta gama, extender CR a la PA (planta alta) — ahí estará la suite principal, y ahí vive el equipo AV, mesas de noche con carga, camas motorizadas y electrónicos sensibles.

**Costo: ~$500–1,000 USD por el circuito y contactos adicionales. Alto valor percibido.**

### 1d. Sistema de Energía de Emergencia: **Mejorar (ver Sección 7)**

Los planos actuales tienen contactos de emergencia (CE) e iluminación de emergencia (IE) con respaldo de batería, pero no hay estrategia de respaldo de energía para toda la casa. Ver Sección 7 para el enfoque recomendado.

### 1e. Tubería Conduit PVC: **Mantener**

PVC es el estándar para construcción residencial mexicana y cumple con la norma para esta aplicación. No es necesario subir a EMT o IMC — PVC con soportes adecuados funciona perfectamente y es mucho más barato de instalar. Las abrazaderas omega y anclas para concreto especificadas son apropiadas.

### 1f. Solar (SOL): **Mantener + Optimizar**

Los paneles solares ya están en los planos — bien. Para Cuajimalpa (alta elevación, fuerte insolación), el solar es una de las mejores inversiones por retorno. La decisión clave es si combinarlo con almacenamiento de batería (ver Sección 7).

---

## 2. Iluminación — Mantener la Base, Elegir Plataforma con Inteligencia

### 2a. Pre-cableado para Apagadores Inteligentes: **Mantener — Esto es Oro**

La nota explícita en los planos de IL — "En cada apagador se considera neutro para el uso de apagadores inteligentes" — significa que tu electricista ya sabe llevar neutro a cada caja de apagador. Esto es lo más caro de hacer en retrofit y ya está hecho. Protege esta especificación.

### 2b. Plataforma de Control de Iluminación: **Reducir de Crestron/Savant → Lutron RadioRA3**

Para una casa de este tamaño, la tentación será ir con Control4, Crestron, o Savant para iluminación. No lo hagas.

| Plataforma | Costo Típico (casa de este tamaño) | Confiabilidad | Expansibilidad | Costos Continuos |
|------------|-------------------------------------|---------------|----------------|-----------------|
| Crestron | $80,000–150,000 USD | Excelente | Requiere distribuidor | Dependiente del distribuidor |
| Savant | $60,000–120,000 USD | Muy buena | Requiere distribuidor | Dependiente del distribuidor |
| Control4 | $40,000–80,000 USD | Buena | Requiere distribuidor | Licencia anual |
| **Lutron RadioRA3** | **$15,000–35,000 USD** | **La mejor del mercado** | **Auto-expandible** | **Ninguno** |

Lutron RadioRA3 es:
- La misma empresa que fabrica los sistemas comerciales de cada hotel de lujo que has visitado
- El único control de iluminación con historial de confiabilidad de 99.99%+
- Compatible con HomeKit, Alexa, Google y sistemas de terceros
- Sin cuotas anuales, sin dependencia del distribuidor después de la instalación
- Soporta controles Pico (apagadores inalámbricos sin batería que puedes colocar en cualquier lugar)

**Tus cables neutros ya están ahí. Los apagadores RadioRA3 se instalan directamente.**

**Ahorro: $40,000–80,000 USD vs. Crestron/Savant por funcionalidad equivalente o superior.**

### 2c. Zonas de Iluminación: **Mantener**

26+ zonas solo en S1 indica control granular habitación por habitación. Esto es apropiado para alta gama. Cada zona se mapea a un apagador o dimmer RadioRA3.

### 2d. Selección de Luminarias (No en Planos MEP): **Agregar Guía**

Los planos MEP especifican circuitos y apagadores, no luminarias. Para lujo costo-eficiente:
- **Empotrados (downlights)**: Usar Lucifer Lighting o WAC Lighting (grado arquitectónico, mitad del precio de Flos/iGuzzini, misma calidad de luz)
- **Luminarias decorativas**: Aquí es donde gastar — piezas de declaración en vestíbulo, comedor, sala
- **LED en todo**: Especificar mínimo CRI 90+ para todas las luminarias. Esto es lo que hace que una casa se sienta lujosa — el índice de rendimiento de color, no la marca.
- **Warm dim**: Para recámaras y salas, especificar luminarias con capacidad warm-dim (atenúan a ~2200K como incandescente). Lutron lo soporta nativamente.

---

## 3. Plomería y Agua — Base Sólida, Tres Mejoras Clave

### 3a. Cinco Sistemas de Agua: **Mantener**

Cuajimalpa tiene suministro municipal de agua notoriamente poco confiable. Tener cinco sistemas separados (suministro, sanitaria, pluvial, aguas sucias, alternativo) no es sobre-ingeniería — es inteligente. La captación pluvial y el sistema alternativo se pagarán solos.

### 3b. Presión de Agua: **Mejorar — Agregar Sistema Hidroneumático**

Los planos muestran un sistema tradicional de tinaco (tanque por gravedad). Para una casa de 6 niveles, esto significa:
- Presión inconsistente entre pisos
- Presión débil de regadera en pisos superiores
- No se pueden usar múltiples muebles de alto flujo simultáneamente

**Recomendación**: Agregar un sistema hidroneumático en el cuarto de máquinas (MQ en S1/S2). Usa la cisterna como reservorio y una bomba de velocidad variable para mantener presión constante en toda la casa.

- Equipo: Bomba de presión de velocidad variable (Grundfos SCALA2 o similar)
- **Costo: ~$3,000–5,000 USD instalado**
- **Impacto: Transforma la experiencia diaria de regadera/baño. Esta es la queja #1 en casas de lujo mexicanas que lo omiten.**

Conservar los tinacos como respaldo de emergencia / suministro de riego — no eliminarlos.

### 3c. Recirculación de Agua Caliente: **Agregar — Especificación Detallada**

No incluido actualmente en los planos. Esta es la mejora de confort de mayor impacto para la experiencia de vida diaria.

**El problema**: El calentador de agua está en el cuarto de máquinas (MQ) en nivel S1/S2. El mueble más lejano (probablemente un baño principal en PA o una llave en AZ) está a 20–30+ metros de tubería. Sin recirculación, dejas correr el agua 45–90 segundos antes de que llegue caliente — desperdiciando 5–15 litros cada vez. En un hogar completo, eso es 15,000–30,000 litros de agua desperdiciados por año, más la frustración diaria de esperar.

#### Sistema Recomendado: Línea de Retorno Dedicada con Control por Demanda

**Cómo funciona**: Una tubería de retorno de pequeño diámetro conecta el final de cada ramal de agua caliente de vuelta al calentador. Una bomba circuladora mantiene el agua caliente moviéndose lentamente por el circuito para que cuando abras cualquier llave caliente, el agua ya esté caliente en la tubería.

#### Especificación de Equipo

| Componente | Producto Recomendado | Propósito | Costo Est. (USD) |
|------------|---------------------|-----------|-----------------|
| Bomba circuladora | **Grundfos COMFORT 15-14 BA PM** | Velocidad variable, auto-adaptación, ultra silenciosa (5 dB). Timer integrado + sensor de temperatura. | $400–600 |
| Tubería de retorno | CPVC 1/2" o cobre tipo L | Línea de retorno dedicada desde el mueble más lejano hasta el calentador. Aislar todos los tramos con espuma de 3/4". | $800–1,500 (material + mano de obra) |
| Válvula check | Resorte, 1/2" latón | Previene flujo inverso por termosifón cuando la bomba está apagada | $30–50 |
| Válvulas de balanceo | Serie Caleffi 116 o equivalente | Una por ramal para balancear flujo entre pisos | $50–80 cada una (×3–4) |
| Sensor de temperatura | Incluido con modelo Grundfos PM | Auto-aprende patrones de uso, opera la bomba solo cuando es necesario | Incluido |
| Aislamiento de tubería | Espuma de celda cerrada 3/4" (Armaflex o equivalente) | Previene pérdida de calor en línea de retorno, reduce desperdicio de energía | $200–400 |
| **Total** | | | **$1,700–3,200** |

#### Distribución de Tubería para Casa Guanábanos

Basado en la estructura del edificio (calentador en S1/S2, muebles de S1 a AZ):

```
AZ (Azotea) ────── ramal agua caliente ──┐
                                          │ (retorno)
PA (Planta Alta) ── ramal agua caliente ──┤
                                          │ (retorno)
PB (Planta Baja) ── ramal agua caliente ──┤
                                          │ (retorno)
S1 (Sótano 1) ──── ramal agua caliente ──┤
                                          │
                    ┌─────────────────────┘
                    ▼
            Bomba circuladora → Calentador (MQ en S1/S2)
```

**Notas clave de ruteo para el ingeniero MEP:**
1. Pasar la línea de retorno paralela a las columnas de suministro de agua caliente existentes (planos IH) — misma columna, mismos soportes
2. Cada nivel recibe una tee de la línea de retorno con válvula de balanceo
3. El retorno se conecta al lado de entrada de agua fría del calentador (a través de la bomba circuladora y la válvula check)
4. Aislar AMBAS líneas (suministro Y retorno) en la columna vertical — tubería sin aislar en una columna actúa como radiador y desperdicia energía

#### Modos de Control (Grundfos COMFORT PM)

| Modo | Cómo Funciona | Uso de Energía | Mejor Para |
|------|--------------|----------------|------------|
| **AutoAdapt (recomendado)** | Aprende tus patrones diarios en 7 días. Opera la bomba solo durante ventanas de uso predichas. | Mínimo — 5–15 watts promedio | Uso diario, consciente de energía |
| Timer | Tú configuras horario on/off (ej. 6–9am, 5–10pm) | Bajo | Horarios predecibles |
| Continuo | Bomba opera 24/7 a baja velocidad | Moderado (~25W constante) | Máxima conveniencia, mayor energía |
| Controlado por temperatura | Opera cuando la temperatura de retorno baja del punto de ajuste | Bajo-moderado | Enfoque balanceado |

**Recomendación: Usar modo AutoAdapt.** La bomba aprende cuándo tu hogar típicamente usa agua caliente y pre-circula solo durante esas ventanas. El costo anual de electricidad es aproximadamente $15–25 USD.

#### Por Qué Retorno Dedicado (No una Válvula de Cruce/Bypass)

Existe una alternativa más barata — una válvula de cruce (como Watts 500800) instalada bajo el mueble más lejano que usa la línea de agua fría como ruta de retorno. Cuesta $100–200 y no necesita tubería de retorno.

**No la uses.** La válvula de cruce empuja agua tibia a tus líneas de agua fría, lo que significa:
- Tu agua fría sale tibia los primeros 10–20 segundos
- Los WC se llenan con agua tibia (desperdicia energía, promueve acumulación mineral)
- El agua fría potable del grifo no sale fría
- No es apropiado para una casa de alta gama

El retorno dedicado cuesta más pero entrega un resultado limpio: el agua caliente es caliente, el agua fría es fría, instantáneamente.

#### Momento de Instalación

**Esto DEBE hacerse durante obra negra (antes de cerrar muros).** La tubería de retorno corre junto a la tubería de suministro en las mismas columnas y ductos. Hacer retrofit significa:
- Abrir muros terminados en cada piso
- Resanar y repintar
- Costo típico de retrofit: $5,000–8,000+ vs. $1,700–3,200 durante construcción

#### Qué Decirle al Ingeniero MEP

> "Agregar una línea de retorno de agua caliente dedicada de 1/2" desde la derivación del mueble más alto/lejano de cada nivel de regreso al cuarto de máquinas. Especificar una bomba circuladora Grundfos COMFORT 15-14 BA PM con válvula check en la conexión de retorno al calentador. Incluir válvulas de balanceo en cada tee de nivel. Aislar TODA la tubería de suministro Y retorno de agua caliente con aislamiento mínimo de espuma de celda cerrada de 3/4"."

#### Ahorro Anual vs. Sin Recirculación

| Métrica | Sin Recirculación | Con Recirculación |
|---------|-------------------|-------------------|
| Tiempo de espera para agua caliente (pisos superiores) | 45–90 segundos | 3–5 segundos |
| Agua desperdiciada por año | ~20,000 litros | ~500 litros |
| Ahorro en costo de agua SACMEX | — | ~$800–1,200 MXN/año |
| Costo de energía de la bomba | $0 | ~$300–500 MXN/año |
| **Ahorro neto anual** | | **~$500–700 MXN/año + confort invaluable** |

### 3d. Filtración de Agua para Toda la Casa: **Agregar**

La calidad del agua municipal de CDMX no es potable. Incluso para uso no potable (regaderas, lavandería), el agua sin tratar causa acumulación mineral, daño a muebles e irritación de la piel.

**Recomendación**: Instalar un sistema de filtración para toda la casa en el punto de entrada del agua domiciliaria:
- Etapa 1: Filtro de sedimentos (50 micrones)
- Etapa 2: Carbón activado (cloro, sabor, olor)
- Etapa 3: Ósmosis inversa punto de uso solo en tarja de cocina (agua potable)

- **Costo: ~$2,000–4,000 USD para filtración general + OI en cocina**
- **Impacto: Protege cada mueble, extiende vida de electrodomésticos, provee agua potable. Estándar en casas de alta gama en CDMX.**

### 3e. Gas LP: **Mantener**

El gas LP es probablemente la única opción en esta parte de Cuajimalpa (la red de gas natural no llega a la mayoría de la zona). El sistema de manifold por nivel está correctamente especificado. Asegurar que la terraza tenga preparación de gas para cocina exterior.

---

## 4. HVAC — Calefacción + Ventilación

### 4a. Calefacción (CAL): **Mantener — Probablemente la Decisión Correcta**

Si esto es calefacción por piso radiante hidrónico (probable, basado en los planos de CAL y el cuarto de máquinas), es premium y eficiente en costo de operación:
- Operación silenciosa
- Distribución uniforme de calor
- Sin ductos
- Compatible con solar térmico para eficiencia

**Confirmar con ingeniero MEP: ¿Es hidrónico radiante, radiadores, o eléctrico?**

### 4b. Ventilación: **Agregar — Especialmente para Sótanos**

Dos niveles subterráneos (S1, S2) necesitan ventilación mecánica. Sin ella:
- La humedad se acumula → moho, olor a humedad
- La calidad del aire se degrada
- Cualquier equipo de gas (calentador, cuarto de máquinas) necesita aire de combustión

**Recomendación**:
- Niveles de sótano: Extractores + inyección de aire fresco con control de humedad
- **Costo: $3,000–5,000 para ventilación de sótanos**

---

## 5. Seguridad — Buen Inicio, Necesita Perímetro y Control de Acceso

### 5a. CCTV: **Mejorar Cobertura**

Actualmente solo S1 y PB tienen cobertura CCTV. Para Cuajimalpa (una zona deseable pero consciente de seguridad), se necesita:

| Zona | Actual | Recomendado |
|------|--------|-------------|
| S1 (Sótano) | Sí | Mantener — acceso a garage/estacionamiento |
| PB (Planta Baja) | Sí | Mantener — puntos principales de acceso |
| PA (Planta Alta) | No | Agregar — accesos de terraza/balcón |
| AZ (Azotea) | No | Agregar — vista perimetral |
| Perímetro exterior | No mostrado | **Agregar — capa principal de seguridad** |
| Acceso vehicular / portón | No mostrado | **Agregar — acceso vehicular** |

**Recomendación de cámaras para eficiencia de costo**: Cámaras Ubiquiti UniFi Protect:
- Grado comercial, resistentes a intemperie
- PoE (Power over Ethernet — un solo cable para energía + datos, usa tu cableado estructurado existente)
- Sin cuotas mensuales de nube (NVR local)
- 1/3 del costo de cámaras empresariales Axis o Hikvision
- **~$200–400 USD por cámara vs. $800–2,000 para Axis**
- Administradas desde la misma plataforma UniFi que tu red (ver Sección 6)

**Costo estimado para cobertura completa**: 8–12 cámaras adicionales × $300 promedio = $2,400–3,600 + NVR ($300–500)

### 5b. Control de Acceso: **Agregar**

No incluido en los planos actuales. Las casas de alta gama en Cuajimalpa necesitan:

| Componente | Recomendación | Costo |
|------------|--------------|-------|
| Videoportero en portón | DoorBird D2101V o 2N IP Verso | $1,500–3,000 |
| Cerradura electrónica puerta principal | Yale Assure Lock 2 o similar | $300–500 |
| Portón vehicular motorizado | Confirmar con arquitecto (probablemente ya planeado) | Variable |
| Botones de pánico | En recámara principal + cocina | $200–400 |

**Total control de acceso: ~$3,000–5,000 USD**

### 5c. Alarma / Intrusión: **Clarificar y Agregar si Falta**

El juego de planos es ambiguo sobre si existe un sistema de alarma dedicado. Como mínimo:
- Sensores de puerta/ventana en todos los accesos de planta baja y sótano
- Sensores de movimiento en áreas comunes
- Sensores de rotura de cristal en ventanales grandes
- Sirena (interior + exterior)
- Conexión de monitoreo (GSM + internet doble vía)

**Si se usa Ajax Systems (inalámbrico, excelente confiabilidad, popular en segmento de lujo CDMX): ~$2,000–4,000 para una casa de este tamaño.**

---

## 6. Red y AV — La Mayor Oportunidad de Ahorro

### 6a. Red Doméstica: **Reducir de Empresarial → Prosumer**

Los planos muestran un switch de datos de 24 puertos y cableado estructurado. Buena infraestructura. La pregunta es qué equipo va en el rack.

**Recomendación: Ubiquiti UniFi — la opción de valor clara**

| Componente | Especificación | Costo |
|------------|---------------|-------|
| UDM Pro SE (router + NVR) | 1× | $500 |
| USW-Pro-48-PoE (switch 48 puertos) | 1× (subir de 24 a 48 puertos) | $800 |
| Access points U6 Enterprise | 4–6× (uno por nivel + exterior) | $200–350 cada uno |
| **Total** | | **$2,500–4,000** |

Compara con Meraki ($15,000–25,000 + licencia anual) o Ruckus ($10,000–18,000) para la misma cobertura. UniFi se usa en hoteles de lujo, restaurantes y oficinas en todo el mundo. Para residencial, es exceso de calidad de la mejor manera.

**Ahorro: $10,000–20,000+ vs. alternativas empresariales.**

Nota: Subir de switch de 24 a 48 puertos durante construcción. La diferencia de costo es mínima ($300–500) y usarás cada puerto entre cámaras, APs, puntos de TV y dispositivos inteligentes.

### 6b. Audio Multizona: **Reducir de Integrado → Sonos**

Si un integrador AV propone Crestron, Savant, o Control4 para audio en toda la casa, el precio será $30,000–80,000 para una casa de este tamaño.

**Recomendación: Sonos**
- Sonos Architectural by Sonance (bocinas empotradas en plafón) para zonas permanentes
- Sonos Era 300 / Era 100 para habitaciones donde el empotrado no es necesario
- Sonos Amp para zonas exteriores y terraza
- AirPlay 2 + Spotify Connect + todo lo demás integrado
- Sin necesidad de distribuidor para uso continuo

| Zona | Solución | Costo por Zona |
|------|----------|---------------|
| Sala | Sonos Amp + par arquitectónico | $1,200–1,500 |
| Cocina | Sonos Amp + par arquitectónico | $1,200–1,500 |
| Recámara principal | Sonos Era 300 (par) | $900 |
| Terraza | Sonos Amp + par exterior | $1,500–2,000 |
| Baños | Sonos Era 100 | $250 cada uno |
| **Total (6–8 zonas)** | | **$6,000–10,000** |

**Ahorro: $25,000–70,000 vs. Crestron/Savant por calidad de audio igual o superior y 10× mejor usabilidad.**

### 6c. Canalizaciones de TV/AV (planos TV): **Mantener + Agregar Una Cosa**

Las canalizaciones vacías para TV/AV están correctamente especificadas. Agregar un requisito: **pasar una canalización HDMI de reserva (35mm o mayor) desde el gabinete principal de datos a cada ubicación principal de TV.** El streaming es el presente, pero la distribución HDMI aún se necesita para contenido 4K/8K de alta calidad y gaming.

---

## 7. Energía de Respaldo — Agregar una Estrategia

### Estado Actual
Los contactos de emergencia (CE) e iluminación de emergencia (IE) existen con respaldo de batería, pero no hay estrategia de respaldo para toda la casa.

### Recomendación: Solar + Batería (No Generador)

Ya tienes paneles solares en los planos. Agregar almacenamiento de batería en vez de generador diésel/gas:

| Opción | Costo | Costo Continuo | Ruido | Almacenamiento Combustible |
|--------|-------|----------------|-------|---------------------------|
| Generador diésel | $8,000–15,000 | Combustible + mantenimiento anual | Ruidoso | Riesgo de incendio |
| **Solar + Tesla Powerwall (×2)** | **$18,000–25,000** | **Casi cero** | **Silencioso** | **Ninguno** |
| Solar + Baterías Enphase IQ | $16,000–22,000 | Casi cero | Silencioso | Ninguno |

Para CDMX, donde los apagones típicamente duran 1–4 horas (no días), dos Powerwalls (27 kWh) cubren toda la casa. Se cargan con tus paneles solares durante el día y proporcionan transferencia automática durante apagones.

**Esto también permite optimización de tarifa** — cargar con solar durante tarifa punta de CFE, usar batería en la noche. Ahorro esperado de 30–50% en recibos de luz.

---

## 8. Carga de Vehículo Eléctrico — Preparar Ahora, Agradecerse Después

### No está en los planos actuales. Esto es $1,500 de preparación ahora vs. $8,000+ de retrofit después.

**Recomendación**: Durante construcción, tender:
- Circuito dedicado 40A/240V desde tablero principal al área de estacionamiento (S1 o S2)
- Tubería conduit 35mm (ya es un tamaño estándar en tus planos)
- Contacto NEMA 14-50 o preparación para cargador

El cargador real ($500–1,500 para una unidad Nivel 2) se puede instalar cuando sea. El circuito y la tubería son las partes caras de agregar después.

**Costo durante construcción: ~$1,500–3,000 USD (tubería + cable + interruptor)**

---

## 9. Persianas Motorizadas — Pre-cablear Ahora, Instalar Después

**No confirmado en los planos actuales.** Pedir al ingeniero MEP que agregue:
- Contacto 110V o alimentación de bajo voltaje en la parte superior de cada vano principal de ventana
- Idealmente dentro de un cajón oculto (fascia o nicho en plafón) para instalación limpia

Esto es ~$100–200 por ventana de preparación que ahorra $500–1,000 por ventana en costos de retrofit después. Las persianas reales (Lutron Palladiom, Hunter Douglas PowerView, o Coulisse — todas excelentes) pueden instalarse por fases.

Las persianas Lutron se integran perfectamente con RadioRA3 si eliges esa plataforma.

---

## 11. Resumen: Acciones Prioritarias

### Obligatorio (Antes de Cerrar Muros)

| # | Acción | Costo | Impacto |
|---|--------|-------|---------|
| 1 | Subir CED-17 y CED-18 a #10 AWG | ~$300 | Corrige caída de tensión marginal a norma |
| 2 | Agregar CR (contactos regulados) a nivel PA | ~$800 | Protección de equipo AV en recámara |
| 3 | Agregar sistema hidroneumático | ~$4,000 | Presión de agua consistente en todos los niveles |
| 4 | Agregar recirculación de agua caliente (retorno dedicado + bomba Grundfos COMFORT) | ~$2,500 | Agua caliente instantánea en cada mueble, ahorra ~20,000 litros/año |
| 5 | Agregar ventilación mecánica de sótanos | ~$4,000 | Previene moho, requerido para equipos de gas |
| 6 | Preparar circuito de carga EV en garage | ~$2,000 | Preparación para el futuro |
| 7 | Pre-cablear alimentación de persianas motorizadas en ventanas | ~$2,000 | Persianas futuras sin cableado visible |
| 8 | Subir a switch de 48 puertos (de 24) | ~$400 | Capacidad para cámaras + dispositivos inteligentes |

**Total preparación "Obligatorio": ~$16,000 USD**

### Compras Inteligentes (Post-Construcción, por Fases)

| # | Elemento | Costo | Cuándo Comprar |
|---|----------|-------|---------------|
| 1 | Sistema Lutron RadioRA3 | ~$20,000–30,000 | Durante acabados eléctricos |
| 2 | Stack de red Ubiquiti UniFi | ~$3,500 | Durante acabados de bajo voltaje |
| 3 | Cámaras Ubiquiti Protect (perímetro completo) | ~$4,000 | Durante acabados de bajo voltaje |
| 4 | Tesla Powerwall ×2 + integración solar | ~$20,000 | Después de instalación solar |
| 6 | Audio multizona Sonos | ~$8,000 | Cualquier momento — mayormente inalámbrico |
| 7 | Filtración de agua para toda la casa | ~$3,000 | Durante acabados de plomería |
| 8 | Control de acceso + alarma (Ajax) | ~$5,000 | Durante acabados de seguridad |
| 9 | Persianas motorizadas | ~$15,000–30,000 | Después de mudanza, habitación por habitación |

### En Qué NO Gastar

| Tentación | Por Qué Evitarlo | Ahorro |
|-----------|------------------|--------|
| Crestron o Savant para toda la casa | Dependiente de distribuidor, sin beneficio real sobre Lutron + Sonos | $50,000–100,000 |
| Networking Meraki o Ruckus | Licencias anuales, sin ventaja real para residencial | $10,000–20,000 |
| Alimentadores eléctricos todo cobre | MC4 aluminio es correcto para alimentadores, reservar cobre para derivados | $3,000–5,000 |
| Tubería conduit EMT/IMC (vs. PVC) | No requerido por NOM para residencial, PVC es suficiente | $5,000–10,000 |
| Distribución de audio cableada | Sonos iguala o supera la calidad a 1/5 del precio | $25,000–60,000 |
| Pantallas táctiles en cada habitación | Tu teléfono es la mejor pantalla táctil. Controles Pico de Lutron para apagadores. | $10,000–30,000 |

---

## 12. Preguntas para Tu Próxima Junta de Equipo

1. **Para el Ingeniero MEP**: ¿El sistema de CAL (calefacción) es hidrónico radiante o radiadores?
2. **Para el Ingeniero MEP**: CED-17 y CED-18 — ¿podemos subir a #10 AWG? ¿Y podemos agregar contactos CR al nivel PA?
3. **Para el Ingeniero MEP**: Agregar línea de retorno de agua caliente dedicada de 1/2" desde la derivación del mueble más alto/lejano de cada nivel de regreso al MQ. Especificar bomba circuladora Grundfos COMFORT 15-14 BA PM con válvula check en conexión de retorno al calentador. Incluir válvulas de balanceo en cada tee de nivel. Aislar TODA la tubería de suministro Y retorno de agua caliente con espuma de celda cerrada mínimo de 3/4".
4. **Para el Arquitecto**: ¿Están planeados cajones para persianas motorizadas en los cabezales de ventanas?
5. **Para el Ingeniero MEP**: ¿Cuál es la estrategia de ventilación para sótanos S1 y S2?
6. **Para Todos**: ¿Tenemos un espacio designado para el rack de red / gabinete de cableado estructurado? Los planos muestran un gabinete empotrado en muro — ¿es suficientemente grande para un stack completo de UniFi + NVR + paneles de parcheo?

---

*Última actualización: 19 de marzo de 2026*
