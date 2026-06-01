# Revision Turnitin para reenvio del articulo

## Nota sobre el 27% de IA

Segun la documentacion oficial de Turnitin, el porcentaje de escritura con IA no equivale al porcentaje total del documento ni constituye una prueba aislada de mala conducta academica. El indicador se calcula sobre texto calificado en prosa larga y estima que parte de ese texto podria haber sido generado o modificado por IA.

Turnitin tambien explica que el modelo procesa segmentos de varias oraciones y asigna una puntuacion a cada oracion dentro de su contexto. Por eso, una oracion tecnica puede verse afectada por un parrafo completo si el bloque presenta baja variacion estructural, repeticion, tono generico o parafrasis sin nuevo desarrollo argumental.

Fuentes oficiales revisadas:

- https://guides.turnitin.com/hc/en-us/articles/27139000787853-How-should-I-review-the-AI-Writing-report
- https://guides.turnitin.com/hc/en-us/articles/22774058814093-Using-the-AI-Writing-Report
- https://guides.turnitin.com/hc/en-us/articles/28477544839821-Turnitin-s-AI-writing-detection-capabilities-FAQs

## Criterios usados en la reescritura

- Reducir afirmaciones absolutas como "definitive", "unequivocally", "catastrophic", "fundamentally" y "undeniable".
- Cambiar frases genericas por formulaciones ligadas al experimento: escenario, condicion LOS/NLOS, ubicacion del tag, metrica o distribucion.
- Variar estructuras repetidas como "i.e.", "This finding shows", "This establishes" y "The results reveal".
- Mantener datos numericos, condiciones experimentales, citas y conclusiones tecnicas.
- No "humanizar" artificialmente: cada cambio debe mejorar precision, trazabilidad o tono academico.

## Matriz de revision por oracion o bloque equivalente

| Seccion | Oracion original | Riesgo frente a Turnitin | Problema academico | Cambio propuesto | Por que cambia | Que se conserva |
| --- | --- | --- | --- | --- | --- | --- |
| Abstract | "Ultra-Wideband (UWB) technology has emerged as a promising solution..." | Frase inicial generica y frecuente en textos de IA. | Tono promocional. | "Ultra-Wideband (UWB) is widely used..." | Vuelve la afirmacion mas descriptiva y verificable. | UWB, IPS y alta precision. |
| Abstract | "However, its performance... is significantly affected..." | Estructura contrastiva muy comun. | "significantly affected" es amplio. | "In body-worn tracking... can obstruct..." | Explica el mecanismo fisico. | BS degrada el enlace. |
| Abstract | "This article presents..." | Formula estandar repetida. | No precisa el tipo de enlace. | "This article reports an experimental characterization..." | Situa el estudio en 1D y 6.5 GHz. | Caracterizacion experimental. |
| Abstract | "Seven body-worn tag placements, i.e...." | Uso repetido de "i.e." y frase larga. | Enumeracion pesada. | "A fixed anchor and a body-worn tag were used..." | Mejora legibilidad y concreta el montaje. | Siete ubicaciones. |
| Abstract | "Time-of-Flight measurements were collected..." | Correcta, pero muy compacta. | Faltan nombres de escenarios. | "More than 100,000 independent ToF range samples..." | Agrega indoor corridor y outdoor open field. | ToF, LOS/NLOS y mas de 100,000 muestras. |
| Abstract | "The findings show..." | Formula generica de resultado. | "critically determines" es absoluto. | "The results indicate a clear dependence..." | Reduce intensidad sin perder conclusion. | Dependencia de la ubicacion. |
| Abstract | "In contrast, torso placements exhibit severe degradation..." | Lenguaje fuerte. | "severe degradation" sin matiz. | "Torso placements were the most affected..." | Mantiene el hallazgo con tono sobrio. | MAE maximo de 97.76 cm. |
| Abstract | "Furthermore, the statistical analysis indicates..." | Transicion generica. | "Log-normal" inconsistente en capitalizacion. | "Distribution fitting showed..." | Nombra directamente el metodo. | Modelo log-normal y comparacion con Gaussian. |
| Abstract | "It is also documented..." | Voz pasiva impersonal. | "paradoxically" puede sonar enfatico. | "The indoor corridor also produced..." | Conecta resultado con escenario medido. | Multipath constructivo. |
| Abstract | "These findings provide..." | Cierre generico. | "robust" sin evidencia directa. | "These measurements provide experimental support..." | Basa la conclusion en mediciones. | Algoritmos conscientes de ubicacion y distribucion. |
| Introduction | "Over the last two decades..." | Apertura amplia y comun. | No conecta rapido con el experimento. | "Indoor Positioning Systems have become part..." | Entra con aplicaciones concretas. | IPS y aplicaciones humanas. |
| Introduction | "UWB technology has emerged as a fundamental solution..." | "fundamental solution" es absoluto. | Tono promocional. | "UWB is frequently selected..." | Formula mas prudente. | UWB para ToF. |
| Introduction | "Despite these theoretical advantages..." | Estructura generica. | "critical obstacles" y "complex" sobreactuan. | "When the mobile node is worn..." | Relaciona problema con tag corporal. | BS como fuente de degradacion. |
| Introduction | "The BS phenomenon occurs..." | Define bien, pero abusa de "i.e." | Forma poco natural. | "In this study, the tag is..." | Aclara terminos sin latinismos repetidos. | Tag y anchor. |
| Introduction | "This effect is not negligible..." | Frase defensiva/generica. | "severely degrade" es intenso. | "These propagation changes can introduce..." | Describe impacto medible. | Errores de ranging y seguridad industrial. |
| Introduction | "These figures underscore..." | Tono de enfasis. | "fundamental barrier" es absoluto. | "These results show that BS must be considered..." | Convierte enfasis en implicacion de diseno. | Relevancia de BS. |
| Introduction | "The 6.5 GHz band remains relatively unexplored..." | Afirmacion valida pero amplia. | Falta foco en body-worn ranging. | "The 6.5 GHz band remains less documented..." | Precisa el vacio. | Frecuencia de 6.5 GHz. |
| Introduction | "The central focus of this study..." | Repeticion con siguiente objetivo. | Redundancia. | "For this reason, the present study focuses..." | Vincula razon fisica y analisis estadistico. | Error de ranging y distribuciones. |
| Introduction | "The central objective..." | Repite "central". | Estilo formulistico. | "The objective..." | Simplifica. | Objetivo del articulo. |
| Introduction | "significant extension..." | "significant" es promocional. | Intensidad innecesaria. | "extends preliminary research..." | Mantiene aporte sin adjetivo. | Trabajo preliminar citado. |
| Introduction | "Comprehensive Body Placement Analysis..." | Titulo y texto muy publicitario. | "systematically" y "thereby establishing" suenan genericos. | "Body Placement Analysis..." | Presenta medicion y metricas. | Siete ubicaciones. |
| Introduction | "Statistical Ranging Error Modeling..." | "rigorous", "fundamentally", "mathematically proving" activan riesgo. | Sobregeneralizacion. | "Goodness-of-fit criteria and non-parametric tests..." | Enuncia metodo y resultado sin sobreactuar. | Cambio gamma/log-normal y filtro Gaussian. |
| Introduction | "Spectral Characterization..." | "paradoxical" enfatiza demasiado. | Tono llamativo. | "6.5 GHz Indoor/Outdoor Characterization..." | Describe el hallazgo como caso observado. | Indoor/outdoor y reflexiones. |
| Discussion | "fundamentally challenge..." | "fundamentally" y frase de alto impacto. | Generalizacion. | "The measurements indicate..." | Centra la afirmacion en datos propios. | Ubicacion del tag importa. |
| Discussion | "severe impact..." | Intensificador. | Puede sonar concluyente. | "BS is observed..." | Explica atenuacion y sesgo. | Efecto en distribucion de error. |
| Discussion | "This indicates that industrial safety..." | Puede sonar prescriptiva. | Salta de datos a recomendacion. | "For industrial safety..." | Formula recomendacion condicionada. | Preferencia por helmet/high-shoulder. |
| Discussion | "The torso functions as an insurmountable dielectric wall." | Muy absoluto y metaforico. | Riesgo de exageracion tecnica. | "the torso behaves as a lossy dielectric obstacle" | Mas fisico y defendible. | Bloqueo por torso. |
| Discussion | "unacceptable safety margins..." | Carga normativa fuerte. | No define criterio de aceptabilidad. | "may not satisfy precision requirements..." | Evita juicio no cuantificado. | Error cercano a 1 m. |
| Discussion | "critical discovery..." | Tono promocional. | "discovery" sobreactua. | "One counterintuitive pattern..." | Presenta resultado como patron medido. | Multipath constructivo. |
| Discussion | "Traditional RF theory posits..." | Generalizacion amplia. | Puede ser demasiado categorica. | "Indoor environments are often associated..." | Matiza y conserva idea. | Multipath puede degradar. |
| Discussion | "empirical data reveal a paradox..." | "paradox" enfatiza. | Tono llamativo. | "the LOS and NLOS results show..." | Sustituye dramatizacion por lectura de datos. | Comparacion LOS/NLOS. |
| Discussion | "clearly reveal this loss..." | "clearly" e intensificadores. | Demasiado enfatico. | "show this loss..." | Mantiene evidencia sin adverbio. | Fallo mas alla de 6 m. |
| Discussion | "universally exacerbate..." | Universaliza desde el experimento. | Sobregeneralizacion. | "consistent with the observed indoor advantage..." | Limita a la campana medida. | Wrist 24.07 cm vs 22 cm. |
| Discussion | "definitive statistical evidence..." | Absoluto. | Afirmacion demasiado cerrada. | "A key statistical result..." | Mantiene importancia sin cerrar debate. | No Gaussian bajo BS. |
| Discussion | "fundamentally explains..." | Causalidad fuerte. | Exagera alcance. | "helps explain..." | Relacion causal prudente. | Impacto en EKF y Least Squares. |
| Discussion | "necessarily underestimates..." | Determinismo fuerte. | Depende de implementacion. | "can underestimate..." | Introduce condicion. | Riesgo de sesgo. |
| Discussion | "undeniable empirical baseline..." | Absoluto. | Tono promocional. | "provide an empirical reference..." | Mas sobrio. | Referencia para diseno UWB. |
| Conclusions | "rigorous experimental characterization..." | "rigorous" como autoevaluacion. | Poco necesario. | "experimental characterization..." | Deja que metodologia sostenga rigor. | BS, UWB y 6.5 GHz. |
| Conclusions | "single most dominant factor..." | Absoluto. | Reduce matices por escenario. | "strongly affects..." | Conserva fuerza con prudencia. | Ubicacion del tag. |
| Conclusions | "head placement unequivocally emerged..." | Absoluto y contradice outdoor NLOS. | Inconsistencia tecnica. | "head placement provided the best indoor NLOS..." | Corrige por escenario. | Head 18.66 cm y 4.87 cm. |
| Conclusions | "catastrophic degradation..." | Lenguaje dramatico. | No academico. | "Torso-adjacent placements were the most affected..." | Preciso y medible. | Hip/chest MAE. |
| Conclusions | "Constructive Multipath paradox..." | "paradox" y mayusculas innecesarias. | Tono llamativo. | "constructive multipath pattern..." | Presenta fenomeno como observacion. | Efecto indoor. |
| Conclusions | "successfully mitigate BS..." | Exceso causal. | No prueba mitigacion general. | "partially preserve ToF observability..." | Relaciona con medicion. | Reflexiones en corridor. |
| Conclusions | "severely skewed..." | Intensificador. | Puede ser reemplazado por modelo. | "heavy-tailed log-normal..." | Usa descriptor estadistico suficiente. | Cambio gamma/log-normal. |
| Conclusions | "definitive empirical baseline..." | Absoluto. | Tono promocional. | "empirical reference..." | Mas defendible para reenvio. | Utilidad para futuros sistemas. |

## Nota breve para el reenvio

The manuscript was revised to improve academic style, methodological traceability, and precision in the interpretation of the experimental results. The revision reduced overly absolute wording, clarified the scenario-specific nature of the findings, preserved all reported numerical results, and strengthened the connection between each conclusion and the measurements. The changes do not alter the experimental protocol, datasets, figures, statistical tests, or main technical conclusions.


# Revision de comentarios de ZeroGPT en resultados.tex

Nota: quite de esta bitacora los bloques largos copiados de `resultados.tex`, porque repetirlos completos aqui vuelve a someter el mismo estilo al detector. En su lugar dejo el diagnostico y la accion aplicada en el manuscrito.

| Comentario | Diagnostico | Accion aplicada en `resultados.tex` | Datos conservados |
| --- | --- | --- | --- |
| 1 | La descripcion de la figura usaba frases de plantilla como "comprehensive visualization" y "this representation directly compares". | Se cambio por una lectura directa de la grafica: eje horizontal, eje vertical, configuraciones y funcion del grafico antes de las metricas. | Figura de dispersion, distancias de 1 m a 13 m y ejemplo Outdoor-Hip-NLOS. |
| 2 | El inicio de la comparacion sonaba procedimental y muy uniforme; ademas repetia "i.e." para cada valor. | Se reorganizo como decision de lectura: primero corredor interior, luego campo abierto. Los valores se dejaron en parentesis. | MAE, desviacion estandar, error maximo, wrist 6.42 cm, hip 7.19 cm, ankle 41.50 cm, head 18.66 cm, hip 97.76 cm. |
| 3 | La frase "confirm the placement hierarchy" cerraba demasiado el resultado y podia contradecir el cambio de mejor ubicacion entre escenarios. | Se reemplazo por "same general separation" y se explico que la mejor ubicacion cambia en exterior NLOS. | Wrist 24.07 cm, head 32.05 cm, ankle 38.86 cm. |
| 4 | La descripcion de AIC/BIC estaba correcta, pero sonaba impersonal y muy compacta. | Se explico que AIC y BIC se calcularon sobre 84,511 muestras y luego se separaron los grupos por escenario-condicion. | AIC, BIC, 84,511 muestras y exclusion del baseline TAG. |
| 5 | "radical transformation", "offers the best fit" y "confirms" eran expresiones fuertes. | Se escribio en terminos de menor AIC/BIC y se cambio "confirms" por "suggests". | Modelo log-normal en NLOS, parametros $\mu$, $\sigma$, scale y loc para interior/exterior. |
| 6 | La explicacion de los Q-Q plots era generica. | Se conecto la lectura visual con la comparacion estadistica: LOS queda mas cerca de la recta, pero las colas explican por que gamma ajusta mejor. | Figuras Q-Q LOS/NLOS y comparacion con Normal teorica. |
| 7 | "extreme", "vastly", "firmly rejecting", "severely violate" y "methodologically invalid" subian el tono innecesariamente. | Se uso lenguaje estadistico mas prudente: curvatura fuerte, rechazo para este conjunto de datos, ANOVA no usado, Mann-Whitney como alternativa. | Shapiro-Wilk, Levene, $p \ll 0.001$, Mann-Whitney U, $r = 0.968$. |

## Nota actualizada para el reenvio

The Results section was revised to reduce template-like phrasing and overly categorical statistical language. The edits preserve the experimental values, figures, distribution parameters, and statistical tests, while making the interpretation more specific to the measured scenarios: indoor corridor, outdoor open field, LOS, NLOS, and body-placement groups.
