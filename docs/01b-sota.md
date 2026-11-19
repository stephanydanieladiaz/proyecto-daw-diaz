# 01b · Estado del arte (SOTA) de mi proyecto

> **Plantilla.** En **H1 (26-nov-2026)** entregas una **versión breve** (2-3 páginas: apartados **1, 2 y 5**), junto al `01-analisis.md`. Los apartados 3, 4, 6, 7 y 8 se completan en **H2 (21-ene-2027)** hasta las **4-6 páginas** del documento final. Aquí estudias qué soluciones, **modelos de negocio** y **herramientas** existen ya para el problema que has elegido, y justificas tus decisiones con ello. Cada apartado indica el criterio de evaluación (CE) que alimenta. Borra los bloques «Guía» al rellenar.

> **Guía.** Calendario de H1: **ciclo 1, hasta el jueves 19-nov:** preguntas de búsqueda y tabla de soluciones (apartados 1 y 2) · **ciclo 2, hasta el jueves 26-nov:** hueco y diferenciación (apartado 5). Los apartados 3, 4, 6, 7 y 8 son de H2.
>
> **Reglas.**
>
> - Solo cuenta lo que tiene **enlace y fecha de acceso**.
> - Si usas IA para buscar, **abre cada fuente** y comprueba que existe y dice lo que te cuenta la IA. Puede inventar productos, precios o referencias. Anótalo en `asistenciaIA/bitacora.md`.
> - Usa **solo información pública** de las soluciones que estudias. **Nada** de la empresa de prácticas ni de clientes reales.
> - Compara herramientas con **los mismos criterios**, no por opinión. Salvo razón argumentada, prefiere lo que has visto en el ciclo (Java 21, Spring Boot, SQL).
> - Si algo no lo has podido comprobar, dilo en el apartado 8.

## 1. Problema y preguntas de búsqueda (CE 1c)

**Problema:** Los diseñadores gráficos, ilustradores y creadores visuales sufren la pérdida de atribución de autoría en internet y tienen dificultades para encontrar inspiración visual organizada por gamas cromáticas y procesos creativos reales (bocetos y fases de trabajo), ya que las plataformas actuales priorizan el contenido masivo sin proteger al autor original.

| # | Pregunta | Dónde busqué | Fecha |
|---|---|---|---|
| 1 | ¿Qué plataformas existen actualmente para portafolios creativos? | Buscador web, App Store | 19-11-2026 |
| 2 | ¿Qué modelos de negocio utilizan (gratis, publicidad,suscripción)? | Webs oficiales de las soluciones | 19-11-2026 |
| 3 | ¿Qué tecnologías o carencias tienen que mi proyecto pueda mejorar? | Foros de diseño y reseñas | 19-11-2026 |

## 2. Soluciones existentes (CE 1a, 1c, 2a)

| Solución | Para quién | Qué hace | Modelo de precio | Enlace y fecha de acceso | Estado (`leído` / `sin leer`) |
|---|---|---|---|---|---|
| Pinterest | Público general y creadores visuales | Permite recopilar, organizar y descubrir imágenes mediante tableros y pines estéticos. | Gratuito con publicidad / Planes de pago empresariales | https://pinterest.com (acceso 19-11-2026) | `Leído` |
| Behance | Diseñadores y agencias de todo el mundo | Red de portafolios profesionales para mostrar proyectos creativos completos y buscar empleo. | Gratuito (propiedad de Adobe) | https://behance.net (acceso 19-11-2026 | `Leído` |
| Dribbble | Diseñadores UI/UX e ilustradores | Plataforma de exposición de trabajos cortos ("shots") y contratación de talento creativo. | Gratuito / Suscripción Pro mensual | https://dribbble.com (acceso 19-11-2026) | `Leído` |
| Coolors | Diseñadores y desarrolladores web | Generador rápido de paletas de colores y explorador de tendencias cromáticas. | Freemium (gratis con limitaciones / suscripción Pro) | https://coolors.co (acceso 19-11-2026) | `Leído` |
| Carpetas locales / Libretas | Cualquier creador gráfico o ilustrador | Almacenamiento local de archivos en el ordenador o bocetos en papel físico. | Gratis (recurso propio) | no aplica (solución no digital), 19-11-2026 | `Leído` |


*Esquema de posicionamiento de las soluciones:*
- **Redes masivas / Alto tráfico (Pinterest):** Enfoque generalista, sin control de autoría y con alta presencia publicitaria.
- **Portafolios profesionales (Behance, Dribbble):** Enfoque laboral y estático, orientados a grandes agencias o perfiles consolidados.
- **Herramientas de apoyo específico (Coolors):** Utilidades concretas de una sola función (color) sin gestión de proyectos completos.
- **Propuesta propia (Kreato):** Foco en el proceso creativo (bocetos y paletas) con verificación estricta de autoría para creadores independientes.

## 3. Modelos de negocio (CE 1d, 1e)

| Patrón | Soluciones que lo usan | Ventaja | Riesgo |
|---|---|---|---|
| Freemium / Gratuito con funciones Pro | Coolors, Dribbble | Atrae a una gran masa de usuarios gracias a su uso libre y monetiza a los profesionales que exigen herramientas avanzadas. | Que los límites gratuitos frustren al usuario y abandonen la plataforma antes de pagar. |
| Publicidad y monetización de datos | Pinterest | Genera ingresos masivos a través de anuncios segmentados sin cobrar directamente al usuario final. | Puede sobrecargar la interfaz visual y deteriorar la experiencia limpia que busca un creativo. |
| Plataforma corporativa / Ecosistema | Behance (Adobe) | Se integra como escaparate dentro de un ecosistema de software de pago mayor (Adobe Creative Cloud). | Dependencia directa de una gran corporación y enfoque menos independiente. |

- Modelo para el proyecto: Kreato se plantea como una plataforma web abierta y gratuita para la comunidad de creadores, enfocada a poner en valor el proceso artístico y la autoría, sin ánimo de lucro estricto en su fase de lanzamiento académico (modelo de servicio libre para la comunidad).

## 4. Herramientas y tecnologías (CE 2a, 2b)

Para cada decisión técnica importante del proyecto, se han valorado distintas opciones según su madurez, licencia, coste, curva de aprendizaje y el encaje con los requisitos del ciclo formativo:

| Decisión | Opción | Madurez | Licencia | Coste | Curva de aprendizaje | Encaje con el ciclo | Elegida |
|---|---|---|---|---|---|---|---|
| **Frontend / Maquetación** | HTML5 / CSS3 / Tailwind CSS | Alta | MIT / Código abierto | 0 € | Baja / Media | Muy alto (estándar del ciclo formativo y diseño moderno) | **X** |
| | React / Next.js | Muy alta | MIT | 0 € | Media / Alta | Alto, pero más complejo para una primera versión estática/interactiva | |
| **Lógica interactiva** | JavaScript Vanilla (ES6+) | Muy alta | Estándar web | 0 € | Baja | Excelente para manipulación del DOM y filtros locales de color | **X** |
| | TypeScript | Alta | Apache 2.0 | 0 € | Media | Adecuado, aunque añade sobrecarga de configuración inicial | |
| **Almacenamiento (Mock)** | JSON / LocalStorage | Alta | Estándar navegador | 0 € | Muy baja | Ideal para simular persistencia de datos de forma rápida en entorno educativo | **X** |
| | Firebase / MongoDB | Alta | Propietaria / Open Source | Gratuito (capa base) | Media | Muy útil para bases de datos reales, pero excede los requisitos mínimos del MVP | |

*Cada decisión importante se registrará formalmente en la carpeta `decisiones/` del repositorio.*

## 5. Hueco y diferenciación (CE 1e)

Las plataformas masivas actuales (como Pinterest o Instagram) ofrecen millones de imágenes, pero fallan gravemente en la atribución de autoría (provocando plagios o pérdidas de crédito al creador) y no permiten filtrar la inspiración por paletas de colores asociadas a emociones o por fases del proceso de trabajo (bocetos y evolución). Por otro lado, portafolios como Behance son demasiado rígidos o corporativos.
Kreato cubre ese hueco combinando un feed visual optimizado con un sistema estricto de verificación de autor original y un desglose obligatorio del proceso creativo (de la paleta inicial al resultado final). Para buscar catálogos masivos generales, Pinterest seguirá siendo superior; pero para encontrar inspiración técnica real y proteger al autor, Kreato ofrece una alternativa única.

## 6. Decisiones derivadas (CE 1e, 1f, 2b)

**Tipo de proyecto elegido:** Aplicación web interactiva de portafolio y filtrado visual para creativos.

**Requisitos que salen del estudio:**

- RF-01: Visualización de proyectos en formato masonry o cuadrícula adaptable.
- RF-02: Filtrado de obras por paletas de color y etiquetas de estilo.
- RF-03: Sistema de credenciales e insignia de autoría verificada.

**Decisiones técnicas**: Registradas en la carpeta decisiones/ (elección de Tailwind CSS para el diseño visual limpio y JavaScript vainilla para el filtrado dinámico del cliente).

## 7. Fuentes y calidad (CE 2a)

*Al menos **2 fuentes independientes** (no dos páginas de la misma empresa). Datos oficiales o primarios antes que blogs.*

| # | Fuente (enlace) | Tipo | Fecha de acceso | Fiabilidad (alta / media / baja) y por qué |
|---|---|---|---|---|
| F1 | https://help.pinterest.com | Web oficial / Documentación | 19-11-2026 | Alta: Documentación directa de la plataforma de referencia sobre su funcionamiento de pines y tableros. |
| F2 | https://www.behance.net | Plataforma de sector | 19-11-2026 | Alta: Análisis directo del estándar de mercado para portafolios de diseño gráfico. |

## 8. Límites

Durante la elaboración de este estudio y el planteamiento inicial del proyecto, se han encontrado las siguientes limitaciones reales:

- **Concurrencia y rendimiento:** No ha sido posible realizar pruebas de estrés ni comprobar el comportamiento del sistema bajo cargas masivas de tráfico o subidas simultáneas de archivos multimedia pesados por miles de usuarios, al tratarse de una fase de desarrollo de Producto Mínimo Viable (MVP).
- **Métricas de mercado exactas:** Los datos cuantitativos sobre el volumen total de autónomos en el sector del diseño especializado en España son estimaciones basadas en informes generales del INE y Cifras PYME, ya que no existen censos públicos en tiempo real específicos únicamente para plataformas web de inspiración creativa.
- **Validación con usuarios reales:** Las necesidades detectadas provienen de la observación de quejas en foros públicos y análisis de la competencia, a falta de una ronda de entrevistas directas a gran escala con estudios de diseño locales debido al margen temporal del proyecto.

---

## Criterios de evaluación que alimenta este documento (texto literal)

- **1a)** Se han clasificado las empresas del sector por sus características organizativas y el tipo de producto o servicio que ofrecen.
- **1c)** Se han identificado las necesidades más demandadas a las empresas.
- **1d)** Se han valorado las oportunidades de negocio previsibles en el sector.
- **1e)** Se ha identificado el tipo de proyecto requerido para dar respuesta a las demandas previstas.
- **1f)** Se han determinado las características específicas requeridas al proyecto.
- **2a)** Se ha recopilado información relativa a los aspectos que van a ser tratados en el proyecto.
- **2b)** Se ha realizado el estudio de viabilidad técnica del mismo.

> El SOTA **no añade criterios de evaluación**: reúne en un solo sitio lo que 1a-1f y 2a-2b ya piden. La evaluación sigue las listas de cotejo de H1 y H2.
