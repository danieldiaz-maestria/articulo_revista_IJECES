# Plan de Verificación de Referencias

## Objetivo
Verificar que cada entrada en `bibliografia/bibliografia.bib` tenga metadatos correctos (autores, título, año, páginas, DOI) y que las afirmaciones en el artículo estén respaldadas por el contenido real de cada paper.

---

## Completado ✅

### Metadatos `.bib` corregidos
| Clave | Corrección aplicada |
|---|---|
| `ref4` | Título, orden de autores y guion en Lopez-Iturri corregidos |
| `ref15` | Autores completamente reemplazados (7 autores reales de Welch et al.) |
| `ref16` | Primer nombre corregido: `Qing` → `Qinglin` |
| `Pradabphon2019` | Año: 2019 → 2005; título: añadido "radio"; páginas: 660-663 → 638-641 |
| `Schimtt2019` | Año: 2019 → 2014 |
| `Ruonan2019` | DOI: eliminado prefijo `https://doi.org/` |
| `Mirama2021` | Reemplazado paper fabricado por survey real (IEEE Access 2021) |
| `Tanghe2023` | Título y primer autor corregidos |
| `ref14` | Eliminado (duplicado de `ref4`) |
| `Falcone2012` | Eliminado (nunca citado) |
| `Muqaibel2006` | **Nueva entrada** agregada (IEEE Trans. Wireless Commun., 2006) |

### Contenido del artículo corregido
| Archivo | Corrección |
|---|---|
| `introduccion.tex` | "up to 15 dB" → "up to 8 dB" (Ruonan2019 dice 8 dB, no 15 dB) |
| `introduccion.tex` | `ref14` eliminado de citas |
| `discusion.tex` | Atribución de "corridors channel energy" movida de Pradabphon2019 a Muqaibel2006; Pradabphon2019 se mantiene como evidencia complementaria |
| `discusion.tex` | `\cite{Otim2019}` eliminado de frase sobre head placement (solo `ref4` lo soporta) |
| `discusion.tex` | Cita Fan2019 → Guvenc para afirmación sobre Least Squares |
| `discusion.tex` | `ref20` removido de afirmación sobre GMM |
| `resultados.tex` | `ref14` eliminado de citas |

### PDFs verificados y resultado
| Paper | Verificación |
|---|---|
| **Pradabphon 2005** (ISCIT) | Paper correcto. No soporta "corridors" — corregido en texto |
| **Ruonan Zhang 2009** (Phys. Commun.) | Paper correcto. Atenuación máxima = 8 dB (no 15 dB) — corregido en texto |
| **Otim 2019** (IEEE LAWP, FDTD) | Paper correcto. `Otim2019` no soporta head placement — cita removida |
| **Welch 2002** (IEEE JSAC) | Paper correcto. 23.6 dB (auditorium) y 6.8 dB (office) — afirmación en discusion.tex ✅ |
| **Kiliç 2012** (WPNC) | Paper correcto. Sin correcciones de contenido necesarias |

---

## Pendiente ⚠️

### Referencias sin verificar con PDF
| Clave | DOI | Afirmación a verificar |
|---|---|---|
| `Tanghe2023` | `10.1109/JSEN.2022.3232103` | Uso de GMM para modelar errores de ranging con body shadowing |
| `Kianfar2020` | `10.1007/s42461-020-00279-6` | Aplicación de UWB en seguridad industrial subterránea |
| `Guvenc` | (pendiente identificar DOI exacto en .bib) | NLOS introduce sesgos sistemáticos que invalidan Least Squares |
| `ref11` (Lee & Scholtz 2002) | `10.1109/JSAC.2002.805060` | Ranging en entornos con multipath denso |
| `ref13` (Ridolfi 2018) | `10.3390/s18061875` | Escalabilidad de soluciones UWB para alta densidad de usuarios |

### Problema pendiente de decisión
| Problema | Descripción |
|---|---|
| `ref6` (Al-Ammar 2014) | DOI `10.1109/CW.2014.41` verificado correcto vía Crossref. Es un survey de indoor positioning. Citado para "sub-decimeter localization accuracy" — el paper sí menciona UWB entre tecnologías de alta precisión, pero no da cifra explícita de sub-decímetro. Requiere decisión: ¿mantener, ajustar la afirmación, o buscar cita más específica? |

---

## Notas del proceso
- Un AI previo había fabricado entradas completas en `.bib` con autores, títulos y años incorrectos.
- Todos los cambios confirmados han sido commiteados a git (`feat: correccion bibliografia`, `feat: corregir imprecisiones en las referencias`).
- El build usa XeLaTeX → BibTeX → XeLaTeX × 2, salida en `build/`.
