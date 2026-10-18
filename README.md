# Mis Finanzas

App personal de ingresos, gastos, presupuesto 50/30/20 y metas de ahorro. Se instala en el iPhone como app (PWA) y guarda los datos en Google Sheets.

- **Abre al instante**: usa la última copia guardada en el iPhone y se actualiza en segundo plano.
- **Guarda al instante**: cada cambio aparece de inmediato y se envía a Sheets en lote. Sin internet, queda en cola y se sincroniza al volver la conexión.
- **Seguro**: la API exige un token que solo vive en tu iPhone (no está en este repositorio).

| Archivo | Para qué |
|---|---|
| `index.html` | App completa |
| `sw.js` | Caché para abrir rápido y offline (sube `VERSION` al publicar cambios) |
| `manifest.webmanifest`, `icon-*.png` | Instalación en iPhone |
| `apps-script/Code.gs` | Backend: se pega en Google Apps Script |
