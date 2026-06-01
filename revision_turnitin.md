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


# Comentarios generado por un detector de AI:

## Resultados
### Comentario 1
#### Texto: 
Figure \ref{fig:dispersion_mediciones} presents a comprehensive visualization of the measurement dispersion in all experimental configurations. In this scatter plot, the x-axis represents the nominal separation distances evaluated from 1 m to 13 m, while the y-axis lists each scenario-placement-condition combination, such as Outdoor-Hip-NLOS.

### Comentario 2
#### Texto
To determine the most robust tag placement, a comparative analysis of 1D ranging error was performed in the recommended interpretation order: first, the indoor corridor was examined by contrasting LOS and NLOS conditions; then, the outdoor open-field scenario was evaluated using the same LOS/NLOS sequence. The reported metrics are Mean Absolute Error (MAE), Standard Deviation ($\sigma$), and Maximum Error.

Table \ref{tab:resumen_indoor} summarizes the performance metrics for the Indoor Corridor scenario, where multipath effects are strongly present. In indoor LOS, the lowest MAE is obtained at the wrist, i.e., 6.42 cm, followed by the hip, i.e., 7.19 cm, whereas the ankle shows the maximum LOS MAE, i.e., 41.50 cm. In indoor NLOS, the head provides the best body-placement performance, i.e., 18.66 cm, while the hip is the worst case, i.e., 97.76 cm.


### Comentario 3
#### Texto
After the outdoor LOS baseline is established, the outdoor NLOS data confirm the placement hierarchy observed indoors, with the best-performing body placement changing. The wrist placement shows superior outdoor NLOS performance, i.e., MAE = 24.07 cm, followed by the head, i.e., MAE = 32.05 cm, and the ankle, i.e., MAE = 38.86 cm.

### Comentario 4
#### Texto
The fit of these distributions was evaluated using the Akaike Information Criterion (AIC) and Bayesian Information Criterion (BIC) on the body-placement subset of 84,511 samples, excluding the baseline TAG measurements.

The distribution analysis in Table \ref{tab:aic_bic} is reported separately for the indoor corridor and outdoor open-field scenarios under LOS and NLOS conditions, combining the seven body placements within each scenario-condition group. 

### Comentario 5
#### Texto
Table \ref{tab:aic_bic} shows that the log-normal distribution offers the best fit in both indoor and outdoor NLOS, displacing the gamma and exponential distribution models; Figure \ref{fig:ajuste_nlos} provides the corresponding pooled visual reference. The fitted indoor NLOS model is parameterized as $e-\mathrm{loc}\sim\mathrm{Lognormal}(\mu,\sigma)$, with $\mu=-0.9186$, $\sigma=0.8016$, $\mathrm{scale}=\exp(\mu)=0.3991~\mathrm{m}$, and $\mathrm{loc}=-0.0427~\mathrm{m}$; for outdoor NLOS, the parameters are $\mu=-1.0749$, $\sigma=0.5173$, $\mathrm{scale}=0.3413~\mathrm{m}$, and $\mathrm{loc}=0.0372~\mathrm{m}$.

This scenario-specific consistency confirms that the gamma-to-log-normal shift is not an artifact of pooling indoor and outdoor measurements across environments.


### Comentario 6
#### Texto
Figures \ref{fig:qq_los} and \ref{fig:qq_nlos} present the Quantile-Quantile (Q-Q) plots for LOS and NLOS data against a theoretical Normal distribution.


Under LOS conditions, Figure \ref{fig:qq_los} shows that the data points exhibit moderate alignment with the theoretical line. 


### Comentario 7
#### texto
Under NLOS conditions, Figure \ref{fig:qq_nlos} shows extreme curvature and divergence in the upper tail, confirming that large positive errors (biases) are vastly more frequent than a Gaussian model would predict.

The Shapiro-Wilk normality test yielded $p \ll 0.001$ for both conditions, firmly rejecting the Gaussian hypothesis.

\subsection{Non-Parametric Statistical Testing}
Because the data severely violate the assumptions of Gaussianity and homoscedasticity, i.e., Levene's test, $p \ll 0.001$, standard parametric tests such as ANOVA are methodologically invalid for this dataset. 


