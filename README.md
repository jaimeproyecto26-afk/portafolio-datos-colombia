# Inteligencia Económica para Todos
### Portafolio de Analista de Datos — Colombia

> Tres dashboards interactivos que transforman datos públicos del gobierno colombiano en herramientas de decisión para ciudadanos, empresas y el sector financiero.

---

## Ver portafolio en vivo

| Recurso | Enlace |
|---|---|
| Página web del portafolio | *Próximamente en GitHub Pages* |
| Dashboard Ciudadano | *Próximamente en Looker Studio* |
| Dashboard Empresarial | *Próximamente en Looker Studio* |
| Dashboard Financiero | *Próximamente en Looker Studio* |

---

## Visión del proyecto

**"Inteligencia Económica para Todos"** nace de una pregunta simple: ¿por qué los datos económicos que publica el gobierno colombiano son tan difíciles de entender para la mayoría de personas?

Este proyecto convierte información técnica y dispersa del **Banco de la República**, la **Superfinanciera**, el **DANE** y la **DIAN** en dashboards interactivos, accesibles y actualizados diariamente — sin costo alguno, usando exclusivamente herramientas y fuentes gratuitas.

**Tres audiencias, tres herramientas:**

- **Ciudadano** — Entiende cómo la inflación, el dólar y el desempleo afectan tu bolsillo
- **Empresarial** — Toma decisiones de comercio exterior, inversión y cobertura cambiaria
- **Financiero** — Monitorea la digitalización, inclusión y fraude del sistema financiero colombiano

---

## Los tres dashboards

### 1. Dashboard Ciudadano

> *"Este dashboard transforma indicadores macroeconómicos en información comprensible y útil para cualquier colombiano."*

**Indicadores:**

| Sección | Visualización | Indicador |
|---|---|---|
| Resumen económico | Tarjetas KPI | IPC anual, TRM, tasa de interés |
| Inflación | Línea doble | IPC mensual vs. anual |
| Tipo de cambio | Línea con puntos | Dólar COP/USD |
| Poder adquisitivo | Barras comparativas | Salario mínimo vs. IPC |
| Desempleo | Mapa de calor | Tasa por región |
| Costo de vida | Tarjetas explicativas | Canasta básica |

**Propuesta de valor:**
- Simulador de impacto de la inflación en alimentos y servicios
- Alertas sobre variaciones en TRM para viajes o compras internacionales
- Visualización de la evolución del salario real vs. inflación

**Fuentes:** Banco de la República · DANE · datos.gov.co

---

### 2. Dashboard Empresarial

> *"Integra indicadores de comercio exterior, inversión y riesgo cambiario para ofrecer a las empresas una visión estratégica del entorno económico colombiano."*

**Indicadores:**

| Sección | Visualización | Indicador |
|---|---|---|
| Comercio exterior | Barras apiladas + mapa | Exportaciones/importaciones por país |
| Balanza comercial | Línea con áreas | Superávit/déficit |
| Inversión extranjera | KPI + barras | IED por sector |
| Reservas internacionales | Línea temporal | Nivel de reservas |
| Riesgo cambiario | Dispersión | TRM vs. volatilidad |
| Confianza empresarial | KPI | Índice de confianza |

**Propuesta de valor:**
- Mapa interactivo de socios comerciales de Colombia
- Análisis de tendencias sectoriales para exportadores
- Panel de riesgo cambiario con escenarios de cobertura

**Fuentes:** Banco de la República · DANE · Ministerio de Comercio

---

### 3. Dashboard Financiero

> *"Muestra la evolución del sistema financiero colombiano y el comportamiento de los medios de pago."*

**Indicadores:**

| Sección | Visualización | Indicador |
|---|---|---|
| Canales de transacción | Barras apiladas | Cajeros, banca móvil, oficinas |
| Medios de pago | Torta + línea | Efectivo, tarjetas, transferencias |
| Banca digital | KPI + mapa | Penetración por región |
| Inclusión financiera | Barras | Indicadores por departamento |
| Fraude financiero | Línea + alertas | Reportes y tendencias |
| Bancarización | KPI | Tasa nacional |

**Propuesta de valor:**
- Panel de digitalización financiera por región
- Alertas sobre tendencias en fraude y seguridad
- Comparador de medios de pago más usados

**Fuentes:** Superfinanciera · Banco de la República · datos.gov.co

---

## Stack técnico — 100% gratuito

| Capa | Herramienta | Propósito |
|---|---|---|
| **Extracción** | Python · requests · openpyxl | Descarga de fuentes oficiales |
| **Transformación** | Pandas · SQLite | Limpieza y modelado de datos |
| **Almacenamiento** | Google Drive · Google Sheets | Data lake y base de datos ligera |
| **Ejecución** | Google Colab | Entorno Python gratuito en la nube |
| **Automatización** | Google Apps Script | Trigger de actualización diaria |
| **Visualización** | Looker Studio | Dashboards interactivos embebibles |
| **Portafolio web** | GitHub Pages | Sitio web gratuito con dominio .github.io |

---

## Cómo funciona la actualización automática

```
06:00 AM (diario)
    ↓
Google Apps Script activa el trigger
    ↓
Google Colab ejecuta los notebooks de extracción
    ↓
Python descarga los últimos datos de las fuentes oficiales
    ↓
Pandas limpia y transforma los datos
    ↓
Los resultados se escriben en Google Sheets
    ↓
Looker Studio lee los Sheets automáticamente
    ↓
Los dashboards en la web se actualizan en tiempo real ✓
```

---

## Fuentes de datos oficiales

Toda la información de este proyecto proviene exclusivamente de fuentes gubernamentales verificadas:

| Fuente | Portal | Datos |
|---|---|---|
| **Banco de la República** | [banrep.gov.co](https://www.banrep.gov.co/es/estadisticas-economicas) | IPC, TRM, tasa de interés, reservas, IED, balanza comercial |
| **DANE** | [dane.gov.co](https://www.dane.gov.co) | Desempleo, pobreza monetaria, canasta básica |
| **Superfinanciera** | [superfinanciera.gov.co](https://www.superfinanciera.gov.co) | Tarjetas, transacciones, fraude, bancarización |
| **DIAN** | [dian.gov.co](https://www.dian.gov.co/cifras-y-gestion/estadisticas) | Estadísticas transaccionales |
| **Datos Abiertos Colombia** | [datos.gov.co](https://datos.gov.co) | APIs complementarias |

> **Nota de transparencia:** Este proyecto no inventa ni simula datos. Toda cifra mostrada en los dashboards es extraída directamente de las fuentes oficiales listadas arriba, sin modificación de su contenido.

---

## Cómo ejecutar el proyecto localmente

### Requisitos

- Cuenta de Google (para Drive, Colab, Sheets y Looker Studio)
- Cuenta de GitHub

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/portafolio-datos-colombia.git

# 2. Abrir el notebook de extracción en Google Colab
# (File → Open notebook → GitHub → pegar la URL del repositorio)

# 3. Ejecutar las celdas en orden
# El notebook monta Drive, descarga los datos y los procesa automáticamente
```

---

## Notebooks disponibles

| Notebook | Descripción | Estado |
|---|---|---|
| `extraccion_banrep.ipynb` | Descarga series del Banco de la República | 🔄 En construcción |
| `extraccion_dane.ipynb` | Descarga datos del DANE vía API | 🔄 En construcción |
| `extraccion_superfinanciera.ipynb` | Procesa informes de la Superfinanciera | 🔄 En construcción |
| `modelo_ciudadano.ipynb` | ETL completo + SQLite + exportación a Sheets | 🔄 En construcción |
| `modelo_empresarial.ipynb` | ETL completo + SQLite + exportación a Sheets | 🔄 En construcción |
| `modelo_financiero.ipynb` | ETL completo + SQLite + exportación a Sheets | 🔄 En construcción |

---

## Sobre el autor

**Analista de datos** con enfoque en inteligencia económica y visualización de información pública Colombiana.

Este portafolio demuestra competencias en:

- ✅ Extracción de datos desde fuentes oficiales (web scraping, APIs REST, archivos Excel)
- ✅ Limpieza y transformación de datos con Python (Pandas) y SQL (SQLite)
- ✅ Modelado relacional de datos (esquema estrella: dimensiones y hechos)
- ✅ Visualización interactiva con Looker Studio y Power BI
- ✅ Automatización de pipelines de datos
- ✅ Contextualización del entorno económico colombiano

---

## Contacto

- 📧 Email: *andres_j256@hotmail.com*
- 💼 LinkedIn: *www.linkedin.com/in/jaime-ruiz-dorado*
- 🌐 Portafolio: *github.com/jaimeproyecto26-afk/portafolio-datos-colombia*

---

## Licencia

Este proyecto es de uso libre para fines educativos y de portafolio.
Los datos pertenecen a sus respectivas fuentes oficiales del gobierno colombiano.

---

<div align="center">

**Hecho con datos reales · Actualizado diariamente · Costo: $0**

*Banco de la República · DANE · Superfinanciera · DIAN*

</div>
