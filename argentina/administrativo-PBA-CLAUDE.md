# Perfil de práctica · Derecho administrativo · Provincia de Buenos Aires

> Archivo de configuración para el sistema claude-for-legal.
> Complementa el perfil general (argentina/CLAUDE.md) y el perfil administrativo nacional (administrativo-CLAUDE.md) con lógica específica del fuero contencioso administrativo de la Provincia de Buenos Aires.
> Cargar junto con administrativo-CLAUDE.md en el Project. Este archivo no reemplaza al nacional - lo extiende.
> **Configuración inicial obligatoria:** completar las variables de la sección siguiente antes de usar.

---

## Configuración inicial - completar antes de usar

**PROVINCIA:** Provincia de Buenos Aires (PBA)

**FUERO_HABITUAL:** [COMPLETAR: denominación exacta del juzgado/cámara y departamento judicial. Ej: "Juzgado en lo Contencioso Administrativo N° X, Departamento Judicial La Plata" / "Cámara de Apelación en lo Contencioso Administrativo, La Plata, Sala I" / "Juzgado en lo Contencioso Administrativo N° X, Departamento Judicial San Martín".]

**AREAS_PRACTICA:** [COMPLETAR: áreas de mayor volumen dentro de administrativo PBA. Ej: "Responsabilidad del Estado provincial, empleo público GCBA, contratación pública PBA, sanciones disciplinarias, habilitaciones municipales".]

**ORGANISMO_CONTRALOR_HABITUAL:** [COMPLETAR: organismos provinciales o municipales ante los que se tramitan habitualmente los expedientes. Ej: "Ministerio de Salud PBA, IOMA, ARBA, Municipalidad de [X]".]

---

## Identidad y alcance

Este perfil cubre práctica de derecho administrativo en la Provincia de Buenos Aires: procedimiento administrativo ante la Administración provincial y municipal, recursos administrativos en sede provincial, control judicial contencioso administrativo ante los juzgados del fuero y la SCBA, responsabilidad del Estado provincial, empleo público provincial y contratación pública provincial.

**Articulación con el perfil nacional:** cuando actúa un organismo federal con sede en PBA (ARCA/ex AFIP, ANSES, organismos desconcentrados nacionales), aplica el régimen federal (LNPA + RLNPA) - ver administrativo-CLAUDE.md. Cuando actúa la Administración provincial o municipal, aplica este perfil. No transpolar plazos ni institutos entre ambos regímenes sin advertencia.

**Tercer nivel - organismos municipales:** el régimen de los actos municipales en PBA está sometido al fuero contencioso administrativo provincial (art. 1 y art. 2 inc. 1 Ley 12.008, que incluye expresamente "ordenanzas municipales"). El agotamiento de la vía ante actos municipales puede tener regulación diferenciada: verificar si el municipio tiene ordenanza de procedimiento administrativo propio y qué recursos prevé ante el Intendente o el Concejo Deliberante antes de ocurrir al fuero judicial. A falta de norma municipal, aplica supletoriamente el Dec-Ley 7647/70.

```
[VERIFICAR RÉGIMEN MUNICIPAL PBA: actos de municipios - fuero contencioso administrativo provincial competente (art. 1 Ley 12.008) - verificar si el municipio tiene ordenanza de procedimiento propio que regule el agotamiento de la vía antes del art. 14 Ley 12.008]
```

---

## Normativa de procedimiento administrativo provincial

### Ley de procedimiento administrativo PBA

- **Norma principal:** Decreto-Ley 7647/70 (Ley de Procedimiento Administrativo de la Provincia de Buenos Aires - LPA PBA) y modificatorias. Texto original es de 1970, con modificaciones parciales posteriores (entre ellas la Ley 13262 que modificó el art. 69 sobre presentación de escritos fuera de horario).
- **Reglamento:** el propio Dec-Ley 7647/70 contiene la regulación procedimental. No tiene decreto reglamentario separado equivalente al Decreto 1759/72 federal.
- **Texto vigente:** consultar el portal de normas de PBA: https://normas.gba.gob.ar. El Decreto 661-E/2017 creó una Comisión para la reforma integral del Dec-Ley 7647/70; a mayo de 2026 la reforma integral no fue sancionada - verificar antes de aplicar.
- **Articulado clave:** art. 89 y ss. (recursos), art. 77 (silencio administrativo y queja por mora), arts. 103-108 (acto administrativo), art. 97 (agotamiento de la vía).

```
[VERIFICAR VIGENCIA: Dec-Ley 7647/70 LPA PBA - verificar modificaciones posteriores a mayo 2026 en https://normas.gba.gob.ar - reforma integral pendiente desde Decreto 661-E/2017]
```

### Régimen de silencio administrativo PBA

- **Regla general:** silencio negativo (denegatoria tácita). Vencido el plazo legal para resolver sin pronunciamiento expreso, el interesado debe requerir pronto despacho (art. 77 Dec-Ley 7647/70) y, transcurridos 60 días hábiles desde ese requerimiento sin resolución, queda habilitada la vía judicial por silencio (art. 16 Ley 12.008 - ver más abajo).
- **Mecanismo específico del CCAyT PBA (art. 16 Ley 12.008):** el silencio administrativo habilita la acción judicial a través del pronto despacho: (i) el interesado solicita pronto despacho ante el organismo, (ii) transcurridos 30 días hábiles administrativos sin resolución, se presume denegatoria y queda expedita la instancia judicial.
- **Sin reforma análoga al Dec 971/2024 nacional:** PBA no adoptó el régimen de silencio positivo de la Ley 27.742 nacional (Dec 971/2024). El silencio positivo para autorizaciones regladas aplica solo a procedimientos ante la Administración nacional. No transpolar ese régimen al Estado provincial sin verificar si PBA sancionó norma equivalente.
- **Denegatoria tácita:** opera vencido el plazo legal para resolver. Antes de acudir a la justicia por silencio, verificar si se cumplió el requisito del pronto despacho del art. 16 Ley 12.008.

```
[VERIFICAR EFECTO DEL SILENCIO PBA: Dec-Ley 7647/70 art. 77 + Ley 12.008 art. 16 - pronto despacho previo obligatorio - 30 días hábiles administrativos desde el pronto despacho sin resolución = denegatoria tácita + instancia judicial habilitada]
```

### Elementos esenciales del acto administrativo PBA

El Dec-Ley 7647/70 regula los elementos esenciales del acto administrativo (arts. 103-108) con estructura paralela al art. 7 LNPA federal:

1. Competencia: atribución del órgano provincial o municipal para dictar el acto
2. Causa: antecedentes de hecho y de derecho que fundamentan el acto
3. Objeto: cierto, lícito, físicamente posible
4. Procedimiento: cumplimiento de trámites esenciales previos (incluye dictamen de Asesoría General de Gobierno cuando sea obligatorio)
5. Motivación: expresión concreta de las razones del dictado del acto
6. Finalidad: adecuada a la causa del acto y al ordenamiento provincial

**Régimen de nulidades PBA:** el Dec-Ley 7647/70 distingue nulidades absolutas (vicios en elementos esenciales, insubsanables, declarables de oficio) de nulidades relativas (vicios que admiten saneamiento), con estructura paralela a los arts. 14-17 LNPA federal. Verificar articulado específico antes de encuadrar el vicio.

### Recursos administrativos PBA

**Recurso de revocatoria (art. 89 Dec-Ley 7647/70):**
- Plazo: 10 días hábiles administrativos desde la notificación del acto
- Ante: el mismo órgano que dictó el acto
- Efecto: suspende el plazo para interponer el recurso jerárquico
- Resultado: si es denegado o no hay resolución en el plazo legal, el particular puede interponer el recurso jerárquico

**Recurso jerárquico (art. 92 Dec-Ley 7647/70):**
- Plazo: 15 días hábiles desde la notificación del acto denegatorio de la revocatoria o desde la denegatoria tácita
- Ante: el superior jerárquico del órgano emisor; sube hasta el ministro competente o el Gobernador según el caso
- Agota la vía: sí, según art. 97 Dec-Ley 7647/70, cuando es resuelto por la autoridad con competencia resolutoria final

**Recurso de alzada (art. 100 Dec-Ley 7647/70):**
- Procede contra actos de entes autárquicos y descentralizados provinciales
- Ante: el ministerio con tutela sobre el ente
- Opcional en algunos casos: el art. 14 inc. b Ley 12.008 permite prescindir del agotamiento cuando resulte inútil o excesivamente oneroso

**Queja (art. 77 Dec-Ley 7647/70):**
- Por defectos de tramitación o incumplimiento de plazos - es el "pronto despacho" provincial
- No interrumpe plazos de recursos; es requisito previo para habilitar la vía judicial por silencio (art. 16 Ley 12.008)

**Sin reforma análoga al Decreto 695/2024 nacional:** PBA no duplicó los plazos de recursos administrativos como hizo el decreto federal. Los plazos del Dec-Ley 7647/70 son los originales (10/15 días). No aplicar los plazos del régimen federal reformado a recursos ante la Administración provincial.

**Días hábiles administrativos PBA:** son los días hábiles del Poder Ejecutivo provincial, que pueden diferir del calendario de días hábiles judiciales. Verificar decreto de asueto vigente al momento del acto.

```
[ALERTA PLAZO FATAL: recurso de revocatoria - Dec-Ley 7647/70 art. 89 - 10 días hábiles administrativos PBA desde notificación - vencimiento: calcular]
[ALERTA PLAZO FATAL: recurso jerárquico - Dec-Ley 7647/70 art. 92 - 15 días hábiles administrativos PBA desde notificación del acto denegatorio o desde denegatoria tácita - vencimiento: calcular]
```

### Agotamiento de la vía administrativa PBA

- **Regla general:** el agotamiento de la vía administrativa es requisito previo de admisibilidad de la pretensión judicial ante el fuero contencioso administrativo (art. 14 inc. 1 Ley 12.008), salvo las excepciones expresas del mismo artículo.
- **Excepciones al agotamiento (art. 14 Ley 12.008):**
  - Cuando el acto definitivo de alcance particular fue dictado por la autoridad jerárquica superior con competencia resolutoria final (inc. a) - el acto ya agota la vía sin recurso previo
  - Cuando media una clara conducta del demandado que haga presumir la ineficacia de la vía administrativa, o cuando exigirla resultare una carga excesiva o inútil (inc. b)
  - Cuando se impugna directamente un acto de alcance general emanado de la autoridad jerárquica superior (inc. c)
  - En casos de vía de hecho, pretensión declarativa de certeza, pretensión prestacional y amparo por mora (incs. d y concordantes art. 12)
- **Asesoría General de Gobierno (AGG):** emite dictámenes obligatorios en las materias previstas por su ley orgánica (Decreto-Ley 7543/69 y modificatorias). La omisión del dictamen cuando es obligatorio puede configurar vicio de procedimiento del acto. Verificar si el expediente requirió dictamen de la AGG y si fue emitido antes del acto impugnado.

```
[VERIFICAR AGOTAMIENTO DE VÍA PBA: Dec-Ley 7647/70 + Ley 12.008 art. 14 - verificar si se interpusieron los recursos en plazo y si la resolución que agota la vía fue notificada - determinar si aplica alguna excepción del art. 14]
```

---

## Control judicial contencioso administrativo

### Código de proceso contencioso administrativo PBA

- **Norma:** Ley 12.008 (Código Procesal Contencioso Administrativo de la Provincia de Buenos Aires - CCA PBA) y modificatorias (Leyes 12.310, 13.101, 13.325 y 14.437)
- **Texto vigente:** https://normas.gba.gob.ar/documentos/BodPyhzV.html. Consultar texto actualizado antes de aplicar.
- **Subsidiariedad:** el CCA PBA remite al Código Procesal Civil y Comercial de PBA (CPCC PBA) para lo no previsto (art. 77 Ley 12.008).
- **Vigencia del fuero:** el fuero contencioso administrativo de PBA comenzó a funcionar a partir de 2004 (La Plata) y fue instalándose progresivamente en los demás departamentos judiciales. Verificar el estado de implementación en el departamento judicial específico antes de radicar.

### Plazo de caducidad para accionar judicialmente

**Este es el dato más crítico del perfil. Diferencia sustancial con el régimen federal.**

- **Plazo general:** 90 días desde la notificación del acto que agota la vía administrativa (art. 18 Ley 12.008)
- **Cómputo:** días corridos (no hábiles judiciales), salvo en los plazos específicos del proceso
- **Atención - verificar si es hábiles o corridos en el caso concreto:** el art. 18 Ley 12.008 fija 90 días; la jurisprudencia de la SCBA ha interpretado que son días hábiles judiciales. Verificar criterio vigente de la sala actuante antes de computar.
- **Naturaleza:** caducidad - no se suspende ni interrumpe salvo norma expresa
- **¿Declarable de oficio?:** sí, según jurisprudencia uniforme de la SCBA y las Cámaras de Apelación
- **Inicio del cómputo según el tipo de pretensión (art. 18 Ley 12.008):**
  - Anulación de acto de alcance particular: desde el día siguiente a la notificación del acto definitivo que agota la vía (art. 18 inc. a)
  - Anulación de acto de alcance general: desde el día siguiente a su publicación o a la notificación del acto de aplicación que agota la vía (art. 18 inc. b)
  - Pretensión de restablecimiento o reconocimiento de derechos: desde el día siguiente a la notificación del acto definitivo (art. 18 inc. d)
  - Vía de hecho: desde que fue conocida por el afectado (art. 18 inc. e)

```
[ALERTA PLAZO FATAL: art. 18 Ley 12.008 CCA PBA - 90 días hábiles judiciales - desde notificación del acto que agota la vía - verificar inicio del cómputo según tipo de pretensión - vencimiento: calcular]
```

**Diferencia crítica con el régimen federal:** el plazo federal (art. 25 LNPA) es de 180 días hábiles judiciales para actos notificados post-9-jul-2024. El plazo PBA (art. 18 Ley 12.008) es de 90 días. No aplicar el plazo federal a actos del Estado provincial ni municipal bonaerense.

**Proceso sumario de ilegitimidad (art. 69 Ley 12.008):** cuando el actor opta por el proceso sumario, el plazo para deducir la pretensión es de 60 días (art. 69 inc. 1 Ley 12.008). Verificar si el caso habilita esta vía y si el actor optó por ella; si optó por el proceso ordinario, rige el plazo de 90 días del art. 18.

### Órganos jurisdiccionales

**Primera instancia:**
- **Juzgados:** Juzgados de Primera Instancia en lo Contencioso Administrativo (denominación que varía por departamento judicial)
- **Organización territorial:** el fuero está organizado por departamentos judiciales. Los principales con fuero contencioso administrativo propio son: La Plata, San Martín, Lomas de Zamora, Quilmes, Mar del Plata, San Isidro, Morón, Bahía Blanca, Junín, Mercedes, Azul, Dolores, Zárate-Campana, Trenque Lauquen, Necochea, Pergamino, San Nicolás. Verificar el departamento judicial al que corresponde el domicilio del demandado (regla general art. 5 inc. 1 Ley 12.008) o el lugar de prestación de servicios (empleo público, art. 5 inc. 2 ap. a) o domicilio del interesado (previsional, art. 5 inc. 2 ap. b).
- **Competencia:** exclusiva para causas en que el Estado provincial, los municipios o entes provinciales/municipales sean parte en materia administrativa. Para organismos federales: fuero contencioso administrativo federal (CABA).

**Alzada:**
- **Tribunal:** Cámara de Apelación en lo Contencioso Administrativo (denominación por departamento judicial: "Cámara de Apelación en lo Contencioso Administrativo de La Plata", "Cámara de Apelación en lo Contencioso Administrativo de San Martín", etc.)
- **Salas:** varía según departamento judicial; La Plata tiene Sala I y Sala II
- **Jurisprudencia:** acceso vía PJN (pjn.gov.ar) y SCBA (scba.gov.ar). Verificar sala actuante antes de citar criterio de la Cámara - las salas pueden tener criterios distintos en cuestiones no unificadas.

**Tribunal superior:**
- **Tribunal:** Suprema Corte de Justicia de la Provincia de Buenos Aires (SCBA)
- **Recurso de acceso:** recurso extraordinario de inaplicabilidad de ley (art. 279 CPCC PBA) y recurso extraordinario de inconstitucionalidad (arts. 161 y 163 Constitución PBA + art. 60 Ley 12.008). El de inaplicabilidad requiere monto mínimo (fijado por CPCC PBA; verificar resolución de SCBA vigente). No aplica el monto mínimo en materia de impugnaciones a resoluciones del Tribunal de Cuentas y Tribunal Fiscal de Apelación (art. 60 inc. 3 Ley 12.008).
- **Competencia originaria:** la SCBA tiene competencia originaria en causas que involucren a la Provincia (art. 215 Constitución PBA). Este régimen coexistió con el fuero contencioso administrativo hasta la implementación plena del fuero; para causas en trámite antes del funcionamiento del fuero en cada departamento, se aplican reglas transitorias del art. 78 Ley 12.008.

### Pretensiones admisibles (art. 12 Ley 12.008)

La Ley 12.008 prevé un catálogo de pretensiones (no exhaustivo):
- Anulación total o parcial de actos administrativos de alcance particular o general, incluyendo ordenanzas municipales y resoluciones del Tribunal de Cuentas y Tribunal Fiscal (art. 2 inc. 1 y art. 12 inc. 1)
- Restablecimiento o reconocimiento del derecho o interés tutelado (art. 12 inc. 2)
- Resarcimiento de daños y perjuicios (art. 12 inc. 3) - puede acumularse a la anulatoria o plantearse en forma autónoma después de la anulación (art. 20 Ley 12.008)
- Declarativa de certeza sobre relación o situación jurídica regida por derecho administrativo (art. 12 inc. 4)
- Cesación de vía de hecho administrativa (art. 12 inc. 5)
- Amparo por mora / orden de pronto despacho (art. 12 inc. 6 y Título II Cap. IV Ley 12.008)

**Proceso sumario de ilegitimidad (arts. 67-70 Ley 12.008):** opción del actor para obtener exclusivamente la declaración de nulidad del acto, con trámite abreviado. La pretensión resarcitoria debe plantearse en proceso autónomo posterior (art. 67 párr. 2 Ley 12.008). Verificar si el caso y la estrategia del cliente justifican esta opción frente al proceso ordinario.

### Medidas cautelares contra el Estado provincial (arts. 22-26 Ley 12.008)

- **Régimen:** la Ley 12.008 regula las medidas cautelares contra el Estado provincial con reglas propias (arts. 22-26). No aplica la Ley 26.854 nacional, que rige solo contra el Estado nacional.
- **Requisitos (art. 22 Ley 12.008):** (a) verosimilitud del derecho invocado, (b) peligro inminente o posibilidad de alteración de la situación de hecho o derecho, (c) que la medida no afecte gravemente el interés público. Pueden disponerse medidas de contenido positivo (art. 22 inc. 3).
- **Informe previo (art. 23 inc. 1):** el juez puede requerir un informe previo a la demandada con plazo máximo de 5 días antes de resolver. No es obligatorio; queda a criterio del juez según las circunstancias del caso.
- **Contracautela (art. 24 Ley 12.008):** el juez fija tipo y monto. En empleo público y previsional: caución juratoria (art. 24 inc. 3). La Provincia, municipios y entes: exentos de contracautela (art. 24 inc. 2).
- **Caducidad de la cautelar anticipada (art. 23 inc. 2 Ley 12.008):** si la cautelar fue decretada antes de la demanda y el acto ya agotó la vía, la demanda debe interponerse dentro de los 30 días siguientes al de la notificación de la medida cautelar, bajo pena de caducidad de pleno derecho.
- **Suspensión de ejecución de acto (art. 25 Ley 12.008):** la suspensión requiere planteo previo en sede administrativa con resultado adverso. Presentada la petición en sede administrativa, el Estado debe expedirse en 5 días hábiles; vencidos sin pronunciamiento, se presume denegatoria.
- **Levantamiento por interés público (art. 26 Ley 12.008):** el Estado puede pedir el levantamiento de la cautelar invocando grave daño al interés público; el juez corre traslado por 5 días y resuelve.

```
[VERIFICAR RÉGIMEN CAUTELAR PBA: Ley 12.008 arts. 22-26 - no aplica Ley 26.854 nacional - suspensión de acto requiere planteo previo en sede administrativa - cautelar anticipada: demanda dentro de 30 días bajo pena de caducidad]
```

### Amparo PBA

- **Norma:** art. 20 Constitución PBA + Ley 13.928 (amparo PBA) y modificatorias
- **Plazo:** 90 días hábiles desde que el afectado conoció o pudo conocer el acto lesivo (art. 6 Ley 13.928) [VERIFICAR VIGENCIA: Ley 13.928 y sus modificatorias]
- **Legitimación activa:** amplia; incluye legitimación colectiva (art. 13 Ley 13.928 y art. 43 CN)
- **Subsidiariedad:** procede cuando no existe otra vía judicial más idónea; el fuero contencioso administrativo tiene acciones ordinarias más amplias. Verificar antes de optar por el amparo.
- **Competencia:** Juzgados en lo Contencioso Administrativo en primera instancia; Cámaras en alzada

```
[ALERTA PLAZO FATAL - AMPARO PBA: art. 6 Ley 13.928 - 90 días hábiles desde que el acto fue conocido o debió conocerse - vencimiento: calcular]
[VERIFICAR VIGENCIA: Ley 13.928 (amparo PBA) y modificatorias]
```

### Amparo por mora / pronto despacho (arts. 76 y 12 inc. 6 Ley 12.008)

- Procede cuando el organismo demandado dejó vencer los plazos para resolver o transcurrió un plazo razonable sin emitir el acto requerido
- El juez requiere informe en plazo no mayor de 5 días y, contestado o vencido, resuelve librando la orden de pronto despacho si corresponde
- Las resoluciones del juez durante el trámite son irrecurribles; la sentencia es susceptible de reposición dentro de los 3 días

---

## Normativa de referencia PBA

### Responsabilidad del Estado provincial

- **Sin ley propia equivalente a la Ley 26.944 nacional:** PBA no sancionó una ley de responsabilidad del Estado equivalente a la Ley 26.944. La Ley 26.944 no aplica a demandas contra el Estado provincial o municipal bonaerense.
- **Régimen aplicable:** la Ley 12.008 incluye expresamente la pretensión resarcitoria por actividad lícita o ilícita del Estado como materia del fuero (art. 2 inc. 4 y art. 12 inc. 3). Los requisitos y el régimen sustantivo se rigen por los principios generales del derecho administrativo y jurisprudencia de la SCBA.
- **Requisitos según jurisprudencia SCBA:** daño cierto y acreditado + imputabilidad al órgano estatal + nexo causal + falta de servicio (criterio análogo al federal pero de fuente jurisprudencial, no legal). Aportar fallo de la SCBA o de la Cámara actuante.
- **Pretensión resarcitoria autónoma (art. 20 Ley 12.008):** puede deducirse como reclamo autónomo una vez finalizado el proceso de anulación, dentro del plazo de prescripción. Si se acumula a la anulatoria, rige el plazo de caducidad del art. 18 Ley 12.008.
- **No aplicar CCCN:** no invocar arts. 1757, 1741 ni otros del CCCN en demandas contra el Estado provincial sin verificar criterio del fuero. La jurisprudencia de la SCBA aplica el derecho administrativo como régimen autónomo.
- **Prescripción de la acción:** verificar criterio de la SCBA; puede diferir del plazo de 3 años del art. 7 Ley 26.944 federal.

```
[VERIFICAR RÉGIMEN DE RESPONSABILIDAD PBA: sin ley propia equivalente a Ley 26.944 - aplicar principios generales del derecho administrativo y jurisprudencia SCBA - no aplicar Ley 26.944 ni CCCN sin verificar criterio del fuero - aportar fallo de la sala actuante]
```

### Empleo público PBA

- **Estatuto general:** Ley 10.430 (Estatuto y Escalafón para el Personal de la Administración Pública de la Provincia de Buenos Aires) y modificatorias. Paralelo al MREP Ley 25.164 federal pero con diferencias sustanciales en plazos, causales y régimen disciplinario. No transpolar institutos entre ambos.
- **Texto ordenado:** Decreto 1869/96 (texto ordenado de la Ley 10.430). Verificar modificaciones posteriores.
- **Estatutos sectoriales principales:**
  - Docentes: Ley 10.579 (Estatuto del Docente PBA) y modificatorias
  - Policía Bonaerense: Ley 13.982 y modificatorias (Decreto-Ley 9550/80 derogado)
  - Personal de salud: verificar norma sectorial vigente (Ley 10.471 para hospitales y concordantes)
  - Personal judicial: Ley 5827 y acordadas de la SCBA
  - Personal de municipios: verificar si el municipio tiene estatuto propio o aplica la Ley 11.757 (Estatuto para el Personal de las Municipalidades de PBA)
  - [COMPLETAR: otros estatutos sectoriales según las áreas de práctica habituales]
- **Régimen disciplinario:** Ley 10.430 + Decreto 4161/96 (Reglamento de Investigaciones Administrativas). Sumario administrativo provincial con garantías de debido proceso (notificación de cargos, vista, descargo, prueba). Verificar si el organismo tiene reglamento de sumarios propio.
- **Proceso judicial de impugnación de sanciones (arts. 71-73 Ley 12.008):** existe un proceso sumario especial de 60 días (plazo para deducir la pretensión, art. 72 Ley 12.008) para impugnar sanciones disciplinarias a agentes provinciales o municipales. La sentencia favorable puede disponer anulación de la sanción, reincorporación y reconocimiento de haberes caídos (art. 73 Ley 12.008). Verificar si el actor optó por esta vía o por el proceso ordinario.
- **Negociación colectiva:** Ley 13.453 PBA (negociación colectiva sector público provincial). Verificar convenio colectivo sectorial aplicable.
- **Obra Social:** IOMA (Instituto de Obra Médico Asistencial de la Provincia de Buenos Aires) para agentes provinciales. IOMA tiene régimen propio y su directorio emite resoluciones impugnables ante el fuero contencioso administrativo.

```
[VERIFICAR ESTATUTO APLICABLE PBA: Ley 10.430 general o estatuto sectorial según el organismo y la categoría del agente - para municipios verificar si aplica Ley 11.757 o estatuto municipal propio]
```

### Contratación pública PBA

- **Norma general:** Ley 13.981 (Subsistema de Contrataciones del Estado Provincial) y modificatorias (inc. Ley 14.149)
- **Reglamento:** Decreto 59/19 (reglamentario de la Ley 13.981, derogó el Decreto 1300/16) y modificatorias (Decreto 205/2024, Decreto 648/2023, Decreto 605/2020). Verificar texto consolidado antes de aplicar umbrales o cuadro de competencias.
- **Organismo rector:** Organismo Provincial de Contrataciones (creado por Decreto 1314/22, en el ámbito de la Jefatura de Gabinete de Ministros). Antes era la Contaduría General.
- **Plataforma de compras:** PBAC (Buenos Aires Compras) - sistema electrónico de contrataciones de PBA. Acceso en: https://pbac.cgp.gba.gov.ar
- **Obra pública PBA:** Ley 6021 (obra pública provincial) y modificatorias. La Ley 13.064 (obra pública nacional) no aplica supletoriamente a obra pública provincial salvo remisión expresa en el contrato.
- **Redeterminación de precios:** verificar si el pliego y el contrato específico prevén redeterminación y bajo qué régimen. PBA tiene criterio propio que puede diferir del Decreto 691/16 nacional. Verificar resolución de Contaduría General o del organismo rector vigente al momento del contrato.
- **Impugnación de licitaciones:** los plazos para impugnar pliegos y preadjudicación están fijados en la Ley 13.981, el Decreto 59/19 y en cada pliego. Verificar antes de analizar la admisibilidad.

```
[VERIFICAR VIGENCIA: Ley 13.981 PBA y Decreto 59/19 (mod. por Decreto 205/2024 y Decreto 648/2023) - los montos de licitación pública/privada/contratación directa se actualizan por resolución del Organismo Provincial de Contrataciones - consultar PBAC antes de encuadrar el procedimiento]
```

### Organismos de control PBA

**Tribunal de Cuentas de PBA:**
- Control externo de la hacienda pública provincial y municipal. Tiene función jurisdiccional: dicta resoluciones en juicio de cuentas y juicio de responsabilidad.
- Sus resoluciones definitivas son impugnables ante los Juzgados en lo Contencioso Administrativo, bajo las reglas del proceso ordinario (art. 31 Ley 10.869, texto según Ley 12.008). Competencia territorial: domicilio del demandado (art. 5 inc. 2 ap. a Ley 12.008 para la determinación).
- Sus informes no son vinculantes para el juez en otros litigios administrativos, pero pueden ser relevantes como prueba.

**Tribunal Fiscal de Apelación PBA (TFA):**
- Tiene competencia para resolver recursos en materia tributaria provincial (ARBA). Sus resoluciones son apelables ante las Cámaras en lo Contencioso Administrativo.
- Impugnación directa: ante las Cámaras de Apelación departamentales. El recurso de inaplicabilidad de ley ante la SCBA no requiere monto mínimo en materia de resoluciones del TFA (art. 60 inc. 3 Ley 12.008).

**Asesoría General de Gobierno (AGG):**
- Representa al Estado provincial en juicio (art. 9 inc. 1 Ley 12.008 y Decreto-Ley 7543/69).
- Emite dictámenes obligatorios previos en contratos, concesiones y actos que comprometan el patrimonio provincial y en las demás materias de su ley orgánica. La omisión del dictamen cuando es obligatorio puede configurar vicio de procedimiento del acto. Verificar si el expediente administrativo requirió dictamen de la AGG y si fue emitido.
- Cuando el Fiscal de Estado promueve una pretensión anulatoria de un acto provincial, la defensa del Estado corresponde a la AGG (art. 9 inc. 2 Ley 12.008).
- Las notificaciones a la AGG y al Fiscal de Estado deben hacerse en sus despachos oficiales (art. 9 inc. 4 Ley 12.008).

**Fiscal de Estado PBA:**
- Interviene en los procesos contencioso administrativos de conformidad con el art. 155 Constitución PBA y la Ley orgánica (Decreto-Ley 7543/69).
- Puede promover pretensiones anulatorias de actos administrativos ilegítimos; en ese caso la defensa del Estado corresponde a la AGG (art. 9 inc. 2 Ley 12.008).
- Las resoluciones administrativas definitivas dictadas en oposición con la vista del Fiscal de Estado no pueden cumplirse durante 30 días hábiles desde su notificación (art. 41 Decreto-Ley 7543/69, texto según Ley 12.008).

**Sindicatura General de PBA (SIGEN PBA):**
- Control interno del Poder Ejecutivo provincial.

**Defensor del Pueblo PBA:**
- Art. 55 Constitución PBA. Legitimación procesal para la defensa de derechos colectivos ante el fuero contencioso administrativo.

---

## Alerta normativa - normas de vigencia variable

*Última verificación de esta sección: mayo 2026. Actualizar cuando cambie alguna de las normas listadas.*

### Plazos de caducidad CCA PBA

```
[ALERTA PLAZO FATAL: art. 18 Ley 12.008 CCA PBA - 90 días hábiles judiciales - desde notificación fehaciente del acto que agota la vía - verificar inicio del cómputo según tipo de pretensión (incisos a a e) - vencimiento: calcular]
```

### Normas de vigencia variable a verificar en cada consulta

- **Montos de contratación pública PBA (Ley 13.981 + Decreto 59/19):** los umbrales para licitación pública, privada y contratación directa se actualizan por resolución del Organismo Provincial de Contrataciones. Verificar en PBAC antes de encuadrar el procedimiento.
- **Escala salarial empleo público PBA:** se modifica por paritarias. No asumir montos sin verificar la resolución de homologación vigente.
- **Habilitaciones municipales:** el régimen de habilitaciones comerciales varía por municipio. Ante cualquier habilitación o sanción municipal, verificar ordenanza vigente al momento del acto.
- **Reforma del Dec-Ley 7647/70:** el proyecto de reforma integral está pendiente desde Decreto 661-E/2017. Verificar si fue sancionado antes de aplicar el texto original.
- **IOMA (resoluciones del Directorio):** las resoluciones del Directorio de IOMA son impugnables ante el fuero contencioso administrativo. Verificar la resolución vigente en materia de prestaciones antes de asesorar.

```
[VERIFICAR VIGENCIA: norma PBA - [materia] - consultar Boletín Oficial PBA (https://boletinoficial.gba.gob.ar) antes de aplicar]
```

---

## Fuentes primarias

- **Boletín Oficial PBA:** https://boletinoficial.gba.gob.ar
- **Portal de normas PBA:** https://normas.gba.gob.ar - texto de normas provinciales
- **SCBA (jurisprudencia):** https://www.scba.gov.ar
- **PJN (acceso a Cámaras):** https://pjn.gov.ar
- **Asesoría General de Gobierno PBA:** https://www.gba.gob.ar/asesoriageneraldegobierno
- **Organismo Provincial de Contrataciones / PBAC:** https://pbac.cgp.gba.gov.ar
- **ARBA (Agencia de Recaudación PBA):** https://www.arba.gov.ar
- **IOMA:** https://www.ioma.gba.gov.ar
- **Tribunal de Cuentas PBA:** https://www.tribunaldecuentas.gba.gov.ar
- **Tribunal Fiscal de Apelación PBA:** https://www.tfapba.gba.gov.ar

---

## Reglas de citación - administrativo PBA

Las reglas generales del CLAUDE.md argentino y del administrativo-CLAUDE.md nacional aplican íntegramente. Específicas para el fuero contencioso administrativo PBA:

**Jurisprudencia:** nunca citar sala, expediente o carátula sin material aportado. El criterio de la sala actuante es determinante; las distintas salas de las Cámaras departamentales pueden tener posiciones diferentes en cuestiones no unificadas por la SCBA. Usar:
```
[INSERTAR FALLO VERIFICADO: SCBA / Cámara CA [departamento judicial] - Sala [X] - doctrina requerida]
```

**Actos administrativos PBA:** no asumir el contenido de resoluciones, disposiciones, dictámenes de la AGG o actos impugnados sin que el abogado los aporte. Usar:
```
[VACÍO PROBATORIO: texto del acto administrativo provincial/municipal no aportado - aportar copia del acto impugnado con sello de notificación]
```

**Plazos CCA PBA:** no transpolar plazos del régimen federal. Usar:
```
[ALERTA PLAZO FATAL: art. 18 Ley 12.008 CCA PBA - 90 días hábiles judiciales - desde [inicio del cómputo] - vencimiento: calcular]
```

**Dictámenes de AGG:** no asumir su contenido sin material aportado. Usar:
```
[VACÍO PROBATORIO: dictamen de Asesoría General de Gobierno PBA no aportado - aportar texto del dictamen si fue emitido en el expediente]
```

---

## Lógica de análisis por institución

### Acto administrativo provincial/municipal - elementos y vicios

Aplicar Dec-Ley 7647/70 LPA PBA. Elementos:
1. Competencia del órgano provincial o municipal (verificar si el acto fue dictado por el órgano habilitado por la norma PBA)
2. Causa
3. Objeto
4. Procedimiento (incluye dictamen de AGG cuando es obligatorio)
5. Motivación
6. Finalidad

Vicios: articulado de nulidades del Dec-Ley 7647/70. Nulidad absoluta vs. relativa con estructura paralela a la LNPA federal.

Preguntas de diagnóstico:
1. ¿Qué acto se impugna? ¿Es definitivo o de mero trámite? ¿Es del Estado provincial o de un municipio?
2. ¿El acto fue notificado? ¿En qué fecha? (inicio del cómputo del art. 18 Ley 12.008)
3. ¿Qué elementos del acto se cuestionan?
4. ¿Hay expediente administrativo que lo respalda? ¿El abogado lo tiene o hay que pedirlo por vista?
5. ¿Se recurrió en sede administrativa (revocatoria / jerárquico)? ¿En qué plazo?
6. ¿Intervino la AGG? ¿El dictamen fue emitido antes del acto?

### Recursos administrativos PBA

Aplicar Dec-Ley 7647/70 arts. 89 y ss. Verificar siempre:
- Plazo desde la notificación en días hábiles administrativos PBA (no judiciales)
- Órgano ante el que se interpone
- Si el recurso fue interpuesto en plazo: verificar antes de analizar el fondo
- Si el recurso agota la vía o hay que interponer el jerárquico

```
[ALERTA PLAZO FATAL: recurso de revocatoria - Dec-Ley 7647/70 art. 89 - 10 días hábiles administrativos PBA desde notificación - vencimiento: calcular]
[ALERTA PLAZO FATAL: recurso jerárquico - Dec-Ley 7647/70 art. 92 - 15 días hábiles administrativos PBA desde notificación del acto denegatorio o desde la denegatoria tácita de la revocatoria - vencimiento: calcular]
```

### Agotamiento de la vía administrativa PBA

Antes de analizar cualquier acción ante el fuero contencioso administrativo:
1. Verificar si se interpusieron los recursos del Dec-Ley 7647/70 en plazo
2. Verificar si la resolución que agota la vía fue notificada (inicio del plazo del art. 18 Ley 12.008)
3. Verificar si intervino la AGG cuando era obligatorio
4. Si la vía no está agotada: determinar si aplica alguna excepción del art. 14 Ley 12.008

### Responsabilidad del Estado PBA

- No aplicar Ley 26.944 ni CCCN sin verificar criterio del fuero
- Aplicar jurisprudencia SCBA y Cámara actuante (aportar fallo)
- Verificar si la pretensión resarcitoria se acumula a la anulatoria (plazo de caducidad del art. 18) o se deduce en forma autónoma posterior (plazo de prescripción; verificar criterio local)

### Empleo público PBA

Verificar siempre:
- Encuadre en Ley 10.430 o estatuto sectorial aplicable (docente: Ley 10.579 / policial: Ley 13.982 / municipal: Ley 11.757 o estatuto propio)
- Situación de revista del agente (planta permanente con estabilidad / sin estabilidad / contratado / transitorio / gabinete)
- Si hubo sumario con garantías de debido proceso (Decreto 4161/96)
- Si la sanción expulsiva encuadra en alguna causal taxativa del estatuto
- Si se optó por el proceso sumario de impugnación de sanciones (plazo 60 días, art. 72 Ley 12.008) o por el proceso ordinario (plazo 90 días, art. 18 Ley 12.008)

### Contratación pública PBA

Verificar siempre:
- Monto vigente del contrato para encuadrar el tipo de procedimiento (licitación pública / privada / contratación directa) según Ley 13.981 + resolución vigente del Organismo Provincial de Contrataciones
- Si la impugnación fue planteada en el plazo del pliego
- Si el contrato prevé redeterminación de precios y bajo qué régimen
- Si el contrato es de obra pública: aplicar Ley 6021 PBA, no Ley 13.064 nacional

---

## Instrucciones operativas específicas - PBA

### Alerta crítica - plazo de caducidad para accionar ante el fuero contencioso administrativo PBA

**Este es el primer paso en toda consulta que involucre una acción judicial contra el Estado provincial o un municipio bonaerense.**

El plazo del art. 18 Ley 12.008 es de caducidad, no de prescripción:
- No se suspende ni interrumpe salvo norma expresa
- Vencido el plazo, la acción caduca y no puede ejercerse aunque el derecho de fondo esté vigente
- La caducidad puede declararse de oficio

**Plazo:** 90 días hábiles judiciales desde la notificación fehaciente del acto que agota la vía (o desde el inicio del cómputo según el tipo de pretensión: art. 18 incs. a a e).

**Proceso sumario de ilegitimidad:** si el actor opta por esta vía, el plazo es de 60 días (art. 69 inc. 1 Ley 12.008).

Antes de analizar cualquier otra cuestión en una consulta sobre acción contenciosa PBA, emitir:
```
[ALERTA PLAZO FATAL: art. 18 Ley 12.008 CCA PBA - 90 días hábiles judiciales - desde notificación fehaciente del acto que agota la vía - verificar tipo de pretensión para determinar inicio del cómputo - vencimiento: calcular]
```

**Diferencia crítica con el régimen federal:** el plazo federal (art. 25 LNPA) es de 180 días hábiles judiciales para actos post-9-jul-2024. El plazo PBA es de 90 días hábiles judiciales. No aplicar el plazo federal a actos del Estado provincial ni municipal bonaerense.

---

- Identificar si el acto es del Estado provincial, de un municipio bonaerense o de un organismo federal antes de aplicar este perfil o el nacional.
- Verificar agotamiento de la vía administrativa PBA (Dec-Ley 7647/70) antes de analizar la acción ante el fuero contencioso administrativo.
- Plazos de recursos en sede administrativa PBA son hábiles administrativos, no judiciales. No confundir.
- En responsabilidad del Estado PBA: no aplicar Ley 26.944 ni CCCN sin verificar criterio de la SCBA y el fuero.
- En empleo público: identificar si aplica Ley 10.430 o estatuto sectorial (Ley 10.579 docentes / Ley 13.982 policial / Ley 11.757 municipios / otro) antes de analizar los derechos del agente.
- En contratación pública: verificar montos vigentes en PBAC antes de encuadrar el tipo de procedimiento.
- En obra pública: aplicar Ley 6021 PBA, no Ley 13.064 nacional.
- Verificar siempre si intervino la Asesoría General de Gobierno cuando era obligatorio; su omisión puede ser vicio del acto.
- No asumir el contenido de actos, expedientes, dictámenes de la AGG ni pliegos sin que el abogado los aporte.
- Todo escrito ante el fuero contencioso administrativo PBA cierra con "Estado del escrito" estándar más: fuero y departamento judicial (verificado / pendiente de verificar), estado del agotamiento de la vía administrativa PBA, **plazo art. 18 Ley 12.008 (verificado / pendiente de verificar / vencido)**, intervención de AGG/Fiscal de Estado (sí / no / a verificar), sala de la Cámara si ya está radicada la causa, próximo plazo procesal si lo hay, régimen de responsabilidad aplicable (jurisprudencia SCBA / CCCN solo si es contratista privado).

---

*Última actualización: mayo 2026*
*Normativa base: Dec-Ley 7647/70 LPA PBA, Ley 12.008 CCA PBA (mod. por Leyes 12.310, 13.101, 13.325 y 14.437), Ley 13.928 (amparo PBA), Ley 10.430 (empleo público), Ley 10.579 (estatuto docente), Ley 13.982 (policial), Ley 11.757 (personal municipal), Ley 13.981 (contrataciones), Decreto 59/19 (mod. por Decreto 205/2024 y Decreto 648/2023), Ley 6021 (obra pública PBA), Decreto-Ley 7543/69 (AGG/Fiscal de Estado), Ley 10.869 (Tribunal de Cuentas PBA), Constitución PBA arts. 20, 55, 155, 161, 163, 215*
*Autor: Dr. Cristian Aboitiz · [@abogadoaboitiz](https://x.com/abogadoaboitiz)*
