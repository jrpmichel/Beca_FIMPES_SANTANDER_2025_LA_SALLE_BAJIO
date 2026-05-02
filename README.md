# Micrositio FIMPES 2025 — Paquete de Entregables

## Estructura de archivos

```
micrositio-fimpes/
├── index.html                  ← este micrositio
├── logo_lasalle.png            ← opcional (mismo nombre del LaTeX)
├── Santander.jpg               ← opcional
├── logoFimpes.jpg              ← opcional
└── docs/                       ← carpeta con los entregables
    ├── A1_Propuesta_Tecnica_original.pdf
    ├── A2_Informe_Diagnostico_Alineacion.pdf
    ├── A3_Analisis_Funcional_Perfiles_Tecnicos.pdf
    ├── A4_Diseno_del_marco_de_competencias_tecnicas.pdf
    ├── A5_Estructura_Curricular_de_Microcredenciales.pdf
    ├── A6_Marco_de_Referencia_y_Taxonomia_MMX_FP_CT_ND.pdf
    ├── A7_Cedula_Sintesis_Proyecto_FIMPES_DIC_INV.xlsx
    ├── A8_Checklist_Maestro_de_Microcredenciales.pdf
    ├── B1_Manual_tecnico_DIC_Prueba_Piloto.pdf
    ├── B2_Manual_tecnico_INV_Prueba_Piloto.pdf
    ├── B3_Manual_Extendido_FEA_Referencia.pdf
    ├── C1_Instrumentos_Evaluacion_DIC.pdf
    ├── C2_Instrumentos_Evaluacion_INV.pdf
    ├── D1_Formato_Microcredencial_DIC.xlsx
    ├── D2_Formato_Microcredencial_INV.xlsx       ← typo corregido
    ├── E1_DIC_2D_V3.1.zip
    ├── E2_Manual_Codigo_DIC_2D_V3.pdf
    ├── F1_Articulo_Q1_Optics.pdf                  ← sin acento (portabilidad)
    ├── F2_Articulo_de_congreso_ICECET_2026.pdf    ← sin acento, sin espacio
    ├── F3_Perfil_Unico_del_Investigador.pdf
    └── G2_Carta_respuesta_UniLaSalle_Amiens.pdf
```

## Notas sobre nombres de archivo

El `index.html` espera los nombres **sin acentos ni espacios** para evitar problemas de URL. Renombrar antes de subir:

| Original                                       | En `docs/`                                     |
|------------------------------------------------|------------------------------------------------|
| `B1_Manual_técnico_DIC_Prueba_Piloto.pdf`     | `B1_Manual_tecnico_DIC_Prueba_Piloto.pdf`      |
| `B2_Manual_técnico_INV_Prueba_Piloto.pdf`     | `B2_Manual_tecnico_INV_Prueba_Piloto.pdf`      |
| `D2_Formato_Microcredencia_INVl.xlsx`          | `D2_Formato_Microcredencial_INV.xlsx`          |
| `F1_Artículo_Q1_Optics.pdf`                   | `F1_Articulo_Q1_Optics.pdf`                    |
| `F2_Artículo_de_congreso_ICECET 2026.pdf`     | `F2_Articulo_de_congreso_ICECET_2026.pdf`      |

## Personalización

- **Cambiar carpeta de docs**: editar `const DOC_PATH = "docs/";` cerca del final del `<script>` en `index.html`.
- **Logos**: poner `logo_lasalle.png`, `Santander.jpg`, `logoFimpes.jpg` en la raíz. Se detectan automáticamente.

## Tamaño estimado

- B1 (~24 MB) + B2 (~19 MB) + E2 (~5 MB) + resto (~30 MB) ≈ **80–100 MB total**
- Cabe sin problema en GitHub Pages (límite blando 1 GB / archivo 100 MB), Netlify (100 MB/archivo), Cloudflare Pages (25 MB/archivo — necesita comprimir B1 y B2 si se usa).
