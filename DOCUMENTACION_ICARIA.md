# ICARIA Intelligence Platform – Banco Sabadell (DXC-TDM)

## Descripción

ICARIA Intelligence Platform es una solución modular para análisis, validación y gestión de casos/condiciones de negocio. Centraliza código fuente, datos, outputs, memoria y documentación, asegurando trazabilidad, control de versiones y auditoría.

## Objetivos

- Plataforma web versionada para validaciones y gestión de datos.
- Automatización de outputs y reportes.
- Memoria viva del proyecto: decisiones, roadmap y equipo.
- Facilitar auditoría y colaboración en Banco Sabadell.

## Estructura Detallada

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
│    ├── exportaciones/
│         └── (outputs, reportes, exportaciones reales)
│    ├── plantillas/
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

## Requisitos Técnicos

- Node.js y npm (gestión dependencias JS)
- Navegador web moderno
- Git
- Visual Studio Code (recomendado) u otro editor

## Instalación y Primeros Pasos

```sh
git clone https://github.com/AntonioRodriguezSmith/ICARIA-Intelligence-Platform-1.1.git
cd ICARIA-Intelligence-Platform-1.1
npm install    # Si hay dependencias
npm start      # Si hay script de inicio
# O abrir src/index.html en navegador
```

## Workflow

1. **Carga de datos:** Añadir casos en `datos/entrada/`.
2. **Ejecución lógica:** Usar scripts de `src/js/` para procesar y validar.
3. **Generar outputs:** Aparecen en `outputs/` (revisión y validación), después en `exportaciones/`.
4. **Documentación:** Actualizar `.memoria/` y `docs/analisis/` tras cada hito o cambio importante.

## Confidencialidad

Toda la información es interna y confidencial de Banco Sabadell. Prohibido su uso o divulgación fuera del equipo autorizado.

## Equipo

- AntonioRodriguezSmith
- DXC-TDM / Banco Sabadell (responsables y colaboradores)
- Consultar `.memoria/equipo.json` para historial y roles

## Documentación Clave

- `README.md`: Guía principal
- `.memoria/README.md`: Decisiones y roadmap vivo
- `/docs/analisis/RESUMEN_GLOBAL_PROYECTO.md`: Resumen técnico
- `ESTRUCTURA_PROYECTO.md`: Referencia de estructura

## Enlaces

- [Repositorio Principal](https://github.com/AntonioRodriguezSmith/ICARIA-Intelligence-Platform-1.1)
- [Estructura Detallada](ESTRUCTURA_PROYECTO.md)
- [Checklist Completa](CHECKLIST-COMPLETA.md)