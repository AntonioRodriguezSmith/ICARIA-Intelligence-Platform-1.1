# Estructura de carpetas y archivos del proyecto

```
/
├── .gitignore
├── LICENSE
├── README.md
│
├── .memoria/
│    ├── analisis-casos-v2.json
│    ├── conversaciones.json
│    ├── equipo.json
│    ├── roadmap.json
│    ├── proyecto.json
│    └── README.md
│
├── datos/
│    └── entrada/
│         ├── casos_simplificados.md
│         └── CondicionesIcaria.txt
│    └── exportaciones/
│         └── (outputs, reportes, exportaciones reales)
│    └── plantillas/
│         └── (archivos de ejemplo, si los hubiera)
│
├── docs/
│    └── analisis/
│         ├── RESUMEN_GLOBAL_PROYECTO.md
│         ├── RESUMEN_PR_INICIAL.md
│         ├── ARQUITECTURA_APP.md
│         ├── KPIs.md
│         ├── ANALISIS_GAPS.md
│         └── otros docs de análisis y control
│
├── exportaciones/
│    └── README.md
│    └── (exportaciones y outputs generados por la app)
│
├── src/
│    ├── README.md
│    ├── index.html
│    ├── assets/
│    │     ├── css/
│    │     ├── img/
│    │     └── fonts/
│    ├── js/
│    │     ├── core/
│    │     │     ├── motor-matching.js
│    │     │     ├── parser-md.js
│    │     │     ├── parser-txt.js
│    │     │     ├── detector-formato.js
│    │     │     ├── parser-factory.js
│    │     │     └── scoring.js
│    │     ├── modulos/
│    │     │     ├── mod01-detector/
│    │     │     │     ├── detector.js
│    │     │     │     └── ui-detector.js
│    │     │     ├── mod03-validador/
│    │     │     │     ├── validador.js
│    │     │     │     └── ui-validador.js
│    │     │     ├── arquetipos/
│    │     │     │     ├── gestor.js
│    │     │     │     └── biblioteca.json
│    │     │     ├── chat-ia/
│    │     │     │     ├── chat.js
│    │     │     │     └── motor-ia.js
│    │     ├── utilidades/
│    │     │     ├── exportador-md.js
│    │     │     ├── exportador-pdf.js
│    │     │     └── sanitizador.js
│    │     └── config/
│    │           ├── constantes.js
│    │           └── config.json
│    └── ...
└── ...
```

**Notas:**
- El directorio `src/` agrupa todo el código fuente, scripts centrales, módulos funcionales y recursos de la app.
- `.memoria/` y `docs/` garantizan la trazabilidad y documentación detallada.
- `datos/`, `exportaciones/`, `outputs/`, y `plantillas/` mantienen bien diferenciados los datos fuente, salidas, y recursos auxiliares.
- La estructura favorece auditoría, colaboración y escalabilidad.

Archivo generado automáticamente para documentación interna.