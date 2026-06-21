# 🏆 Mundial 2026 – Dashboard de Partidos

Dashboard web en tiempo real para seguir los partidos del **Mundial de Fútbol 2026** día a día. Un único archivo HTML, sin dependencias, sin instalación, sin API key.

![Screenshot del dashboard](screenshot.png)

---

## ✨ Características

- **Datos en vivo** — consume la API pública de ESPN sin necesidad de registro ni API key
- **Auto-refresh inteligente** — cada 60 segundos si hay partidos en vivo; cada 5 minutos si no los hay
- **Secciones automáticas** — separa los partidos en *En vivo*, *Próximos* y *Finalizados*
- **Goleadores** — muestra nombre y minuto de cada gol
- **Titular del partido** — resumen editorial de ESPN al finalizar cada partido
- **Navegación por día** — botones `‹ ›` para ver cualquier jornada del torneo
- **Diseño dark mode** — interfaz oscura, moderna y responsiva
- **Cero dependencias** — HTML + CSS + JS vanilla, no requiere Node, npm ni nada

---

## 🚀 Uso

### Opción A — Abrir directamente (sin servidor)

```
Doble clic en dashboard.html → se abre en el navegador
```

> ⚠️ Algunos navegadores bloquean `fetch()` desde `file://`. Si ves error de CORS, usá la Opción B.

### Opción B — Servidor local (recomendado)

**Con Python** (viene instalado en la mayoría de los sistemas):

```bash
python -m http.server 7860
```

Luego abrir: [http://localhost:7860/dashboard.html](http://localhost:7860/dashboard.html)

**Con Node.js:**

```bash
npx serve .
```

---

## 📡 Fuente de datos

Los datos provienen de la **API no oficial de ESPN**:

```
https://site.api.espn.com/apis/site/v2/sports/soccer/fifa.world/scoreboard?dates=YYYYMMDD
```

- ✅ Gratuita
- ✅ Sin registro
- ✅ Sin API key
- ⚠️ No oficial — puede cambiar sin previo aviso

---

## 📁 Estructura del proyecto

```
agent.partidos/
└── dashboard.html   # Aplicación completa (HTML + CSS + JS en un solo archivo)
└── README.md
```

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura |
| CSS3 (variables, grid, animaciones) | Diseño dark mode |
| JavaScript (Vanilla ES2020) | Lógica, fetch, render |
| ESPN Scoreboard API | Datos del Mundial |
| Google Fonts – Inter | Tipografía |

---

## 📅 Cobertura del torneo

El Mundial 2026 se juega entre el **11 de junio** y el **19 de julio de 2026** en Estados Unidos, Canadá y México. El dashboard cubre todas las fases:

| Fase | Fechas |
|---|---|
| Fase de grupos | 11 – 27 jun |
| Ronda de 32 | 28 jun – 3 jul |
| Octavos de final | 4 – 7 jul |
| Cuartos de final | 9 – 11 jul |
| Semifinales | 14 – 15 jul |
| Tercer puesto | 18 jul |
| **Final** | **19 jul** |

---

## 📸 Capturas

> El dashboard mostrando los partidos del 20 de junio de 2026:
> España vs Arabia Saudita · Bélgica vs Irán · Uruguay vs Cabo Verde

---

## 📄 Licencia

MIT — libre para usar, modificar y distribuir.
