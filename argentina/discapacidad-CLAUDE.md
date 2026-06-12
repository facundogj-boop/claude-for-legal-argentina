# Perfil de práctica · Derecho de la discapacidad argentino

> Archivo de configuración para el sistema claude-for-legal.
> Complementa el perfil general (argentina/CLAUDE.md) con lógica específica de práctica en discapacidad.
> **Configuración inicial obligatoria:** completar las variables de la sección siguiente antes de usar.

---

## Configuración inicial - completar antes de usar

**FUERO_HABITUAL:**
Indicar el fuero donde tramitan habitualmente tus causas. Opciones: "fuero civil y comercial federal (CABA)", "fuero contencioso administrativo federal", "fuero contencioso administrativo CABA", "fuero civil y comercial PBA - [departamento judicial]", "fuero federal de seguridad social", o combinación.

Ejemplo: `FUERO_HABITUAL: Fuero civil y comercial federal (CABA)`

**AREAS_PRACTICA:**
Indicar las áreas de mayor volumen (prestaciones médicas / obra social y prepaga, CUD, pensiones no contributivas, cupo laboral, accesibilidad, salud mental, amparo por cobertura, etc.).

Ejemplo: `AREAS_PRACTICA: Amparo por cobertura de prestaciones, obra social y prepaga, CUD`

---

## Identidad y alcance

Este perfil cubre la práctica en derecho de la discapacidad argentino: cobertura de prestaciones por obras sociales y empresas de medicina prepaga, obtención y alcances del Certificado Único de Discapacidad (CUD), pensiones no contributivas, cupo laboral, accesibilidad física y comunicacional, salud mental, y tutela judicial efectiva a través del amparo de salud.

El marco normativo es supranacional (Convención sobre los Derechos de las Personas con Discapacidad con jerarquía constitucional desde la Ley 27.044), nacional (Leyes 22.431, 24.901, 27.793 y concordantes) y provincial / local (Ley PBA 10.592 - texto actualizado Ley 14.968, Ley CABA 962 y CCAyT).

No aplica el régimen general de daños del CCCN como fuente principal salvo que haya responsabilidad civil concurrente. Las obras sociales se rigen por la Ley 23.660/23.661 con las obligaciones ampliadas por la Ley 24.901; las empresas de medicina prepaga, por la Ley 26.682. El sistema opera en la intersección de derecho administrativo, derecho a la salud y derechos humanos. En CABA, los amparos contra obras sociales nacionales y prepagas tramitan ante el fuero Civil y Comercial Federal; los reclamos contra el Estado nacional o ANDIS, ante el fuero Contencioso Administrativo Federal.

**FUERO_HABITUAL:** ver sección de configuración inicial
**AREAS_PRACTICA:** ver sección de configuración inicial

---

## Códigos y normativa por fuero

La competencia en discapacidad se determina por el demandado, no por la materia en abstracto.

Fuero | Demandado típico | Código procesal | Alzada
--- | --- | --- | ---
Civil y Comercial Federal (CABA) | Obras sociales nacionales (Ley 23.660), PAMI, empresas de medicina prepaga (Ley 26.682) | CPCCN (Ley 17.454) | Cámara Nacional de Apelaciones en lo Civil y Comercial Federal
Federal Seguridad Social (CABA) | ANSES (prestaciones previsionales, jubilaciones, pensiones, asignaciones familiares) | CPCCN (Ley 17.454) | Cámara Federal de la Seguridad Social (CFSS)
Contencioso Administrativo Federal (CABA) | ANDIS, Ministerio de Salud, organismos públicos nacionales | CPCCN + Ley 26.854 | CNACAF
CCAyT CABA | Gobierno de la Ciudad (transporte, accesibilidad urbana, Ley 962, educación especial CABA) | CCAyT (Ley 189 CABA) | Cámara de Apelaciones CCAyT
Civil y Comercial PBA | Provincia de Buenos Aires, municipios, obras sociales provinciales, empresas privadas | CPCCBA (Ley 7425) | Cámara de Apelación Civil y Comercial por departamento judicial

### Regla especial - demandado mixto (obra social + Estado)

Cuando se demanda conjuntamente a una obra social o prepaga y al Estado nacional (por ejemplo, por el subsidio bajo Ley 24.901 o por incumplimiento sistémico), la jurisprudencia de la CSJN atribuye competencia al fuero Civil y Comercial Federal por especialidad en materia médica. El fuero Contencioso Administrativo Federal queda reservado para cuando el único o principal demandado es el Estado nacional o ANDIS.

### Regla general

El sistema identifica el fuero al inicio de cada consulta. No transpola instituciones procesales entre fueros sin advertencia. Si la consulta no especifica fuero, pregunta antes de analizar. En materia de discapacidad el fuero competente depende de quién es el demandado (obra social nacional, prepaga, ANDIS, GCBA, Estado provincial) y del tipo de prestación; verificar siempre antes de plantear la demanda.

---

## Alerta normativa - normas de vigencia variable

*Última verificación de esta sección: junio 2026. Actualizar cuando cambie alguna de las normas listadas.*

### Emergencia Nacional en Discapacidad - Ley 27.793

La Ley 27.793 (promulgada el 21/09/2025) declaró la emergencia en discapacidad hasta el 31/12/2026 (prorrogable un año). Importante: la ley no creó la Pensión No Contributiva (PNC) por discapacidad; la PNC por invalidez fue instituida por el art. 9 de la Ley 13.478 y el Decreto 432/97. Lo que hace la Ley 27.793 es elevar el piso normativo, blindar presupuestariamente el 70% del haber mínimo frente a decretos de desregulación y reestructurar las auditorías de ANDIS. Ordenó además actualización de aranceles y fortalecimiento del organismo. El Decreto Reglamentario 84/2026 aprueba el reglamento con su anexo integrado. La ejecución de algunos efectos fue objeto de cuestionamiento presupuestario; verificar estado de implementación al momento de cada consulta.

Regla operativa: ante cualquier reclamo de PNC o de aranceles actualizados bajo esta ley, verificar si la emergencia fue prorrogada o vencida:
```
[VERIFICAR VIGENCIA: Ley 27.793 - emergencia en discapacidad - estado al momento de la consulta]
```

### Nomenclador de prestaciones bajo Ley 24.901

Los aranceles del nomenclador se actualizan periódicamente por resolución de la autoridad de aplicación (Ministerio de Salud / ANDIS), no por ley. La última resolución verificada a la fecha de este perfil es RESOL-2026-13-APN-SND#MS (29/03/2026). No citar monto de prestación sin verificar el nomenclador vigente al momento de la consulta.

Regla operativa:
```
[VERIFICAR ARANCEL VIGENTE: prestación - resolución ANDIS en vigor]
```

### Denominación del organismo de aplicación

El organismo nacional de aplicación en materia de discapacidad tuvo varias denominaciones: Subsecretaría de Discapacidad, Secretaría Nacional de Discapacidad, y finalmente ANDIS (Agencia Nacional de Discapacidad), creada por Decreto 698/2017 (BO 06/09/2017) como organismo descentralizado. Los decretos posteriores, incluyendo los de 2024, modificaron su dependencia jerárquica (órbita de Vicepresidencia, luego Jefatura de Gabinete de Ministros) y estructura interna, pero no su creación. En escritos, identificar siempre como ANDIS y verificar la dependencia jerárquica actual:
```
[VERIFICAR VIGENCIA: denominación y estructura del organismo de aplicación - ANDIS]
```

### Ley 26.682 - Medicina prepaga y desregulación económica

Los decretos de desregulación económica dictados entre 2024 y 2026 impactaron sobre la Ley 26.682 y las facultades de la Superintendencia de Servicios de Salud (SSS) en materia de cuotas y cobertura. No invocar topes tarifarios, autorizaciones o regulaciones de la SSS sin verificar que no hayan sido derogadas o liberadas por decreto posterior.
```
[VERIFICAR VIGENCIA: impacto de decretos de desregulación económica sobre Ley 26.682 y facultades de la SSS respecto a cuotas y cobertura]
```

La Ley 26.657 (Derecho a la Protección de la Salud Mental) está en proceso de implementación progresiva y su reglamentación fue objeto de modificaciones. Antes de invocar plazos de internación o criterios de capacidad jurídica, verificar el estado de las normas reglamentarias:
```
[VERIFICAR VIGENCIA: reglamentación Ley 26.657 - plazos e internación involuntaria]
```

### Ley 10.592 PBA - texto actualizado

La Ley 10.592 de la Provincia de Buenos Aires fue actualizada por la Ley 14.968. En escritos referidos a PBA, citar el texto actualizado y verificar si hubo nuevas modificaciones:
```
[VERIFICAR VIGENCIA: Ley PBA 10.592 texto actualizado - Ley 14.968 y modificatorias]
```

---

## Normativa de referencia

### Fundamento supranacional y constitucional

- **Convención sobre los Derechos de las Personas con Discapacidad (CDPCD):**
  - Ley 26.378: aprobación y ratificación de la Convención.
  - Ley 27.044 (promulgada 18/11/2014): otorga jerarquía constitucional conforme art. 75 inc. 22 CN. Fuente interpretativa obligatoria para toda la normativa interna.
  - Arts. clave: 9 (accesibilidad), 12 (capacidad jurídica), 24 (educación inclusiva), 25 (salud sin discriminación), 27 (trabajo y empleo).
- **Convención Interamericana para la Eliminación de Todas las Formas de Discriminación contra las Personas con Discapacidad (CIADDIS):** Ley 25.280 [VERIFICAR VIGENCIA: jerarquía constitucional actual]

### Leyes nacionales fundamentales

- **Ley 22.431 (Sistema de Protección Integral):** base del sistema. Modificada por Ley 25.689 (cupo laboral). Reglamentada por Decreto 312/10. [VERIFICAR VIGENCIA]
- **Ley 24.901 (Prestaciones básicas):** cobertura de obras sociales y prepagas. Prestaciones médico-asistenciales, terapéuticas, educativas y sociales. Obligación de la obra social de cubrir el 100% sin límite de monto.
  - Art. 17: maestra / acompañante terapéutico
  - Art. 22: prestaciones de rehabilitación
  - Art. 24: centros de día
  - Art. 33: sistema de prestaciones básicas para personas sin obra social (ANDIS / Estado)
- **Ley 27.793 (Emergencia Nacional en Discapacidad):** vigente hasta 31/12/2026 (prorrogable). PNC por discapacidad (70% haber mínimo). Actualización de aranceles. [VERIFICAR VIGENCIA]
- **Ley 27.711 (CUD sin vencimiento):** el Certificado Único de Discapacidad no tiene fecha de vencimiento. Gratuito. Válido en todo el territorio nacional.
- **Ley 22.431 + Ley 25.504:** régimen original del CUD (reemplazado en lo pertinente por Ley 27.711 respecto del vencimiento). [VERIFICAR VIGENCIA de interacción]
- **Ley 25.635 (Transporte gratuito):** libre tránsito en transporte colectivo terrestre con CUD. Eximición de peajes. [VERIFICAR VIGENCIA]
- **Ley 24.314 (Accesibilidad y transporte):** accesibilidad para personas con movilidad reducida. [VERIFICAR VIGENCIA]
- **Ley 26.522 (art. 66):** accesibilidad en servicios de comunicación audiovisual. Subtitulado, lengua de señas, audiodescripción.
- **Ley 26.653:** accesibilidad de información en páginas web del Estado, empresas estatales y concesionarias de servicios públicos.
- **Ley 26.858 (Perro guía o de asistencia):** derecho de acceso a espacios públicos y privados.
- **Ley 26.657 (Salud mental):** protección del derecho a la salud mental. Internación involuntaria como último recurso. Interacción con CDPCD art. 12 (capacidad jurídica). [VERIFICAR VIGENCIA reglamentación]
- **Ley 23.660 / 23.661 (Obras sociales y ANSSAL):** marco del sistema de obras sociales nacionales. Base para la obligación de cobertura bajo Ley 24.901.
- **Ley 26.682 (Medicina prepaga):** obligación de las empresas de medicina prepaga de cubrir las prestaciones de la Ley 24.901 y el PMO.

### Decretos reglamentarios clave

- **Decreto 84/2026:** reglamentación de la Ley 27.793 (Emergencia Nacional en Discapacidad). [VERIFICAR VIGENCIA]
- **Decreto 312/10:** reglamentario de la Ley 22.431. Certificación de discapacidad por el Ministerio de Salud / ANDIS.
- **Decreto 1421/02:** reglamentación de la Ley Marco de Empleo Público Nacional (Ley 25.164). Cupo laboral en el sector público. [VERIFICAR VIGENCIA]
- **Decreto 214/06:** homologa el Convenio Colectivo para la Administración Pública Nacional. [VERIFICAR VIGENCIA]

### Normativa provincial y local

- **Ley PBA 10.592 (texto actualizado Ley 14.968):** régimen jurídico básico e integral para personas con discapacidad en la Provincia de Buenos Aires. [VERIFICAR VIGENCIA]
- **Ley CABA 962:** accesibilidad física para todos. Modifica el Código de Edificación de CABA (rampas, aceras, pendientes). [VERIFICAR VIGENCIA]

### Cupo laboral

- **4% mínimo** de personal con discapacidad en: Poder Ejecutivo, Legislativo, Judicial (nacional y provincial), empresas del Estado y servicios públicos.
- Base normativa: Ley 25.689 (modifica Ley 22.431).
- En PBA: verificar régimen específico provincial.

### Fuentes primarias de consulta

- **ANDIS (andis.gob.ar):** organismo de aplicación. Nomenclador, CUD, PNC, normativa actualizada.
- **Infoleg (infoleg.gob.ar):** texto oficial de leyes y decretos nacionales.
- **BOPBA (gob.gba.gov.ar):** normativa provincial PBA.
- **BOCBA (boletinoficial.buenosaires.gob.ar):** normativa CABA.
- **CSJN (csjn.gov.ar):** jurisprudencia federal en materia de discapacidad y amparo de salud.
- **CFSS (cij.gov.ar):** jurisprudencia de la Cámara Federal de la Seguridad Social.
- **SCBA (scba.gov.ar):** jurisprudencia PBA.

---

## Institutos frecuentes y lógica de diagnóstico

### Amparo por cobertura de prestaciones

El amparo de salud es la vía ordinaria para exigir cobertura inmediata de prestaciones. Verificar antes de plantear:

1. ¿El beneficiario tiene CUD vigente o está en trámite?
2. ¿La obra social o prepaga fue intimada fehacientemente y rechazó o guardó silencio?
3. ¿La prestación reclamada está en el nomenclador bajo Ley 24.901 o fue prescripta por profesional habilitado? Si no está en el nomenclador, la obligación de cobertura puede igualmente fundarse en los arts. 25 y 26 CDPCD con jerarquía constitucional (Ley 27.044), siempre que se acredite la inexistencia de alternativa eficaz dentro del nomenclador.
4. ¿La prescripción médica está debidamente fundada? Para prestaciones de tracto sucesivo como acompañante terapéutico (art. 17 Ley 24.901) o maestra de apoyo, acompañar resumen de historia clínica que justifique la especificidad, frecuencia e intensidad de la prestación. La orden médica escueta sin respaldo clínico debilita la verosimilitud.
5. ¿Está configurada la negativa o el silencio? Parametrizar: 48 a 72 horas hábiles sin respuesta en prestaciones urgentes; 10 días corridos en prestaciones de tracto sucesivo. Pasado ese plazo sin respuesta, el silencio es omisión idónea para el amparo.
6. ¿Hay urgencia que justifique medida cautelar autónoma o dentro del amparo?
7. ¿Es obra social nacional o prepaga (fuero Civil y Comercial Federal), obra social provincial (fuero provincial) o demandado estatal único como ANDIS (fuero Contencioso Administrativo Federal)?

Alertas específicas:
- La cobertura del 100% bajo Ley 24.901 no admite copagos ni topes de monto. Si la obra social impone coseguro, es resistible.
- La demora de la obra social en responder la prescripción médica puede configurar conducta omisiva suficiente para el amparo sin necesidad de rechazo expreso.
- Verificar siempre si hay prestador de la red; si no lo hay, la obra social debe autorizar el prestador elegido por el beneficiario.
- Acompañante Terapéutico vs. Cuidador Domiciliario: las obras sociales suelen rechazar la cobertura de AT argumentando que la figura corresponde a un cuidador domiciliario (prestación con menor amplitud o no contemplada del mismo modo en el PMO). La distinción es clínica: el AT cumple un rol terapéutico de rehabilitación con objetivos específicos de salud mental o desarrollo, establecidos en un plan de tratamiento; el cuidador es asistencial. Para resistir el rechazo, el dictamen médico debe explicitar el rol terapéutico y los objetivos rehabilitatorios del AT. Sin ese respaldo, la obra social puede sostener la sustitución.

### Medida cautelar de urgencia

En amparos de salud / discapacidad la medida cautelar es casi siempre autónoma respecto del fondo. Fundamentos habituales:

- Verosimilitud: dictamen médico + Ley 24.901 + CUD (o constancia de trámite)
- Peligro en la demora: irreversibilidad del daño a la salud o al desarrollo del paciente
- Contracautela: en caso de persona en situación de vulnerabilidad, pedir eximición o juratoria

Regla operativa: en amparos de salud en fuero Civil y Comercial Federal, verificar si aplica la Ley 26.854 cuando hay codemandado estatal:
```
[VERIFICAR VIGENCIA: aplicación Ley 26.854 a medidas cautelares en amparo de salud - fuero Civil y Comercial Federal con codemandado estatal]
```

### Certificado Único de Discapacidad (CUD)

- Emitido por ANDIS. Gratuito. Sin fecha de vencimiento (Ley 27.711). Aclaración operativa: "sin vencimiento" no implica que no pueda requerirse actualización de la situación médica o del perfil del beneficiario; la implementación es progresiva según las resoluciones operativas de ANDIS. Verificar si el CUD del beneficiario requiere actualización de datos antes de invocarlo en juicio.
- Habilita: transporte gratuito, cobertura bajo Ley 24.901, pensión no contributiva, cupo laboral, franquicias fiscales.
- La ausencia de CUD no es obstáculo insuperable para el amparo si hay diagnóstico médico acreditado y el trámite está en curso; la jurisprudencia admite la cobertura provisional.

### Pensión No Contributiva (PNC) por discapacidad

- Origen: art. 9 Ley 13.478 y Decreto 432/97. La Ley 27.793 elevó y blindó el piso del 70% del haber mínimo jubilatorio frente a decretos de desregulación.
- Organismo otorgante: ANDIS.
- Monto vigente: 70% del haber mínimo jubilatorio. [VERIFICAR VIGENCIA y monto actualizado al momento de la consulta]
- Requisitos de incompatibilidad: verificar si el beneficiario tiene otro ingreso, jubilación o asignación que genere incompatibilidad.
- Vía de impugnación ante denegatoria: recurso administrativo ante ANDIS; agotada la vía, acción contencioso administrativa federal.

### Cupo laboral

- Obligación del 4% en el sector público y servicios públicos (Ley 25.689 / Ley 22.431).
- Para acreditar el incumplimiento: solicitar informe de planta de personal y porcentaje cubierto.
- Alerta de diagnóstico prudente: las acciones judiciales individuales para exigir el nombramiento de una persona concreta tienen progreso acotado. El amparo colectivo o la acción de cumplimiento presentan mejores perspectivas que el reclamo individual, salvo que el beneficiario se encuentre en los primeros lugares de un orden de mérito de concurso ya aprobado y firme. Evaluar la estrategia antes de litigar.
- En PBA: verificar régimen provincial específico. [VERIFICAR VIGENCIA: cupo laboral PBA]

### Salud mental - internación involuntaria

- La internación involuntaria es de último recurso (Ley 26.657, art. 20). Requiere dictamen del equipo interdisciplinario y control judicial inmediato.
- Plazo máximo de internación involuntaria sin revisión judicial: verificar en la reglamentación vigente.
- Interacción con CDPCD art. 12: la capacidad jurídica de la persona con discapacidad psicosocial o intelectual se presume; las restricciones son de interpretación estricta (CCCN arts. 31-50 post reforma Ley 26.657).

### Prescripción y caducidad

No existe un plazo único para acciones en materia de discapacidad. La regla varía según el tipo de reclamo:

Tipo de reclamo | Plazo | Observación
--- | --- | ---
Prestaciones médicas bajo Ley 24.901 (cobertura futura o en curso) | No prescriptible (derecho continuo) | La obligación de cobertura subsiste mientras subsiste la discapacidad
Reintegros dinerarios por prestaciones ya pagadas | 5 años (art. 2560 CCCN) | La imprescriptibilidad alcanza al derecho a la cobertura, no a la acción de repetición de gastos pasados; no reclamar reintegros sin verificar el cómputo desde cada pago
Pensión No Contributiva (Ley 13.478 / Decreto 432/97) | No prescriptible | Derecho de carácter alimentario
Transporte gratuito con CUD | No prescriptible | Derecho continuo vinculado al CUD
Cupo laboral (reclamo laboral) | 2 años | Aplicar régimen según fuero laboral competente; ver alerta cupo laboral
Accesibilidad - daños y perjuicios (Ley 962 / Ley 22.431) | 3 años | Art. 2561 CCCN (responsabilidad civil concurrente)
Amparo federal (Ley 16.986) | 15 días hábiles (art. 2 inc. e Ley 16.986), pero inaplicable cuando el daño es de tracto sucesivo | La CSJN tiene dicho reiteradamente que en materia de salud el plazo de caducidad no rige mientras la lesión sea continua u omisiva; la falta de cobertura renueva el daño a diario
Amparo local CABA (Ley 2145) | 45 días hábiles desde el acto lesivo | Misma excepción por omisión continua según TSJ CABA; de todas formas alertar siempre y no confiar en la excepción sin verificar jurisprudencia actualizada
Reclamo administrativo (PNC, CUD denegado) | Verificar plazos de silencio y recurso según LPA aplicable | LPA nacional o provincial según el caso

Regla operativa: alertar siempre sobre el plazo aplicable y la fecha de inicio del cómputo antes de analizar el fondo. En amparos locales CABA, el plazo de caducidad es una de las primeras verificaciones a realizar.

---

## Procesos especiales

### Amparo de salud - fuero Civil y Comercial Federal (CABA)

- Vía principal para exigir cobertura inmediata contra obras sociales nacionales y empresas de medicina prepaga.
- El escrito debe: acreditar la condición del beneficiario (CUD o constancia de trámite), la prescripción médica, la intimación a la obra social o prepaga y su silencio o rechazo, y la urgencia.
- Petitorio: medida cautelar de cobertura inmediata + sentencia definitiva de condena a cubrir la prestación + imposición de costas a la demandada.
- Regla operativa: incluir siempre en el petitorio la imposición de costas a la obra social, prepaga o Estado demandado, fundada en la naturaleza alimentaria del reclamo y en la tutela del derecho a la salud como derecho humano. La persona con discapacidad no debe ver mermado su patrimonio para defender su salud.
- Regla operativa procesal: incluir siempre la prueba documental completa como anexo; el fuero resuelve con celeridad cuando la urgencia está acreditada. Verificar aplicación de Ley 26.854 en materia cautelar si hay demandado estatal codemandado.

### Amparo - fuero contencioso administrativo (CABA o federal)

- Para actos u omisiones del GCBA o del Estado nacional (ANDIS, otros organismos).
- En CABA: Ley 2145 (amparo local). Verificar si la materia es de competencia del CCAyT o del fuero civil.
- Plazo de caducidad en CABA: 45 días hábiles desde el acto lesivo (Ley 2145). Alertar siempre.

```
[VERIFICAR VIGENCIA: Ley CABA 2145 - plazo de caducidad del amparo local - estado actual]
```

### Proceso ordinario - obra social o prepaga

- Cuando la prestación no es urgente o el reclamo es dinerario (reintegros, daños).
- Verificar fuero competente: Civil y Comercial Federal para obras sociales nacionales y prepagas; federal de seguridad social para reclamos previsionales ante ANSES; contencioso administrativo federal si el único demandado es el Estado nacional o ANDIS.

### Proceso ordinario o contencioso contra el Estado nacional / ANDIS - vía administrativa previa

- Antes de iniciar un proceso ordinario contra el Estado nacional o ANDIS, verificar el agotamiento de la vía administrativa (Ley 19.549 [VERIFICAR VIGENCIA]): recurso de reconsideración ante el mismo órgano y, si correspondiere, recurso jerárquico ante la autoridad superior. La omisión de este requisito puede derivar en excepción de falta de agotamiento de la vía.
- Excepción para el amparo: la jurisprudencia exime del agotamiento previo cuando el tránsito por la vía administrativa tornaría ilusorio el derecho a la salud o generaría un daño irreversible. En esos casos, la urgencia y el peligro en la demora justifican acudir directamente al amparo sin agotar sede administrativa.
- Regla operativa: ante cualquier reclamo contra el Estado o ANDIS, definir primero si la vía es el amparo (urgencia + omisión continua) o el proceso ordinario (reclamo patrimonial sin urgencia). La elección determina si el agotamiento previo es exigible.

---

## Instrucciones operativas específicas - discapacidad

- Identificar siempre: (a) si el beneficiario tiene CUD vigente o en trámite; (b) quién es el obligado a cubrir (obra social nacional, provincial, prepaga, Estado); (c) si la prestación está en el nomenclador o fue prescripta.
- No asumir cobertura sin verificar que la prestación está contemplada bajo Ley 24.901 o en el PMO. Si hay duda, marcar con [REVISIÓN NORMATIVA REQUERIDA].
- Verificar fuero antes de cualquier análisis procesal: la competencia varía según el tipo de demandado.
- En amparos de salud: plantear siempre la medida cautelar. La demora en la cobertura de prestaciones para personas con discapacidad configura peligro en la demora in re ipsa en la mayoría de los fueros.
- No cuantificar aranceles sin verificar el nomenclador vigente. Si el abogado pide una estimación orientativa, brindarla con marcador [AVANCE BAJO RESERVA] y señalar qué resolución ANDIS corresponde verificar.
- Prescripción: no asumir plazo único; identificar el tipo de reclamo y aplicar la tabla de prescripción y caducidad de este perfil. En amparos locales CABA, verificar el plazo de caducidad de 45 días hábiles como primera verificación.
- Tasa de justicia y BLSG: en amparos de salud / discapacidad, verificar si el fuero aplica exención de tasa de justicia para personas con discapacidad o en situación de vulnerabilidad antes de presentar el escrito inicial. Si el proceso no es un amparo sino un ordinario (ej. daños y perjuicios por falta de accesibilidad), la exención de tasa no cubre automáticamente los gastos de peritos ni las costas en caso de resultado adverso; evaluar y proponer la promoción del Beneficio de Litigar sin Gastos (BLSG) en paralelo con la demanda principal.
```
[VERIFICAR JURISPRUDENCIA: exención de tasa de justicia en amparos de salud/discapacidad - fuero Civil y Comercial Federal y fuero actuante]
```
- Costas: en todo amparo de salud o medida cautelar que resulte en la concesión de la prestación, incluir siempre en el petitorio la imposición de costas a la demandada (obra social, prepaga o Estado). Ver también regla de costas en sección "Amparo de salud - fuero Civil y Comercial Federal".
- Todo escrito en discapacidad cierra con "Estado del escrito" estándar más: fuero y competencia, si el beneficiario tiene CUD vigente (sí / en trámite / ausente), obligado identificado (obra social / prepaga / Estado), prestación en nomenclador (sí / a verificar / fuera de nomenclador con fundamento CDPCD), medida cautelar planteada (sí / no / a evaluar), próximo plazo procesal si lo hay.

---

*Última actualización: junio 2026*
*Normativa base: CDPCD (Ley 26.378 / Ley 27.044), Ley 22.431, Ley 24.901, Ley 27.793, Ley 27.711, Ley 26.657, Ley 26.682*
*Nota: verificar aranceles ANDIS y estado de la emergencia (Ley 27.793) al momento de cada consulta*
*Autor: Dr. Cristian Aboitiz · [@abogadoaboitiz](https://x.com/abogadoaboitiz)*
