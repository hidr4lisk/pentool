# Hidr4lisk_Pentool

**Guía interactiva de pentesting** — una checklist y cuaderno de notas para pruebas de penetración.
100% del lado del cliente · funciona offline · sin backend · sin rastreo.

🌐 **[Demo en vivo](https://hidr4lisk.github.io/pentool/)** · 🇬🇧 **[Read in English](./README.md)**

---

## Qué es

Una web de una sola página que te lleva por un pentest como una serie de pasos ordenados — a nivel
de red y por objetivo — manteniendo tus notas, las herramientas que usaste y los comandos que
corriste, todo en un mismo lugar. Pensada para estudiar y para trabajos reales: la checklist que
querés tener abierta en el segundo monitor.

Todo vive en tu navegador. Tus hallazgos nunca tocan un servidor. Llevás tu trabajo de una máquina a
otra exportando/importando un archivo — nada más.

## Funciones

| # | Función | Descripción |
|---|---------|-------------|
| 01 | **Dos playbooks guiados** | *Redes* y *Objetivos individuales*, cada uno dividido en fases ordenadas — reconocimiento, enumeración, explotación, post-explotación, reporte… |
| 02 | **+60 herramientas con ejemplos** | Cada paso lista las herramientas como chips. Clic en una herramienta para ver ejemplos de comandos listos para usar; clic en un comando para copiarlo. |
| 03 | **Notas por paso** | Un campo de notas en cada paso, autoguardado mientras escribís, con contador de líneas/caracteres. |
| 04 | **Sesiones múltiples** | Un espacio aislado por trabajo/objetivo — crear, renombrar, duplicar, borrar. Cada una guarda sus propias notas y checklist de herramientas. |
| 05 | **Exportar / Importar** | Markdown (`.md`) por sesión para un reporte limpio, o JSON con *todas* las sesiones — tu respaldo portable. |
| 06 | **Progreso y recorrido** | Barras de progreso por categoría, un recorrido de qué herramienta usaste y dónde, y búsqueda en vivo sobre notas y herramientas. |
| 07 | **Comodidad** | Control de tamaño de letra (A−/A+), layout de 1 o 2 columnas, atajos de teclado, tema oscuro estilo terminal. |

## Privacidad

- **Cero conexiones de red** — la página no carga ningún recurso externo; abrila una vez y anda sin internet.
- Sin cookies, sin analytics, sin fingerprinting, sin backend.
- Todo el estado vive en `localStorage`; tu data de pentest nunca sale de tu navegador.
- La portabilidad es explícita: *vos* decidís cuándo exportar un archivo `.md` / `.json`.
- Todo es un único archivo HTML auditable.

## Cómo se mueve tu data

```
 tu navegador (localStorage)  ──Exportar .md / JSON──▶  un archivo tuyo
         ▲                                                    │
         └────────────────────  Importar  ◀───────────────────┘
```

Sin cuenta, sin sync, sin servidor. Te movés entre máquinas llevando el archivo.

## Stack

- **Vanilla JS** — un único archivo HTML autocontenido, sin dependencias, sin build.
- **Web Storage API** — `localStorage` para el estado en vivo (notas, herramientas, sesiones, preferencias).
- **GitHub Pages** — deploy estático.

## Uso previsto

Solo para pruebas de penetración **autorizadas**, práctica en laboratorio y estudio de seguridad
(CTFs, tus propias redes, trabajos con permiso por escrito). Es una checklist de notas — no corre
ningún escaneo ni ataca nada por sí misma. Usala solo donde estés autorizado.

## Licencia

[MIT](./LICENSE)
