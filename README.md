# Presupuestos y APU

App web instalable (celular y PC) para armar presupuestos de obra con análisis de precios unitarios. Funciona sin internet; los datos viven en el equipo (IndexedDB) y se respaldan en un archivo.

Dirección (cuando GitHub Pages esté activo): https://handeress.github.io/Presupuestos/

## Fase 1 (esta versión)
- Biblioteca de APU con capítulos, búsqueda, APU básicos anidados (concretos, morteros, formaleta).
- Mano de obra en 3 modos: cuadrilla con rendimiento, contratista a valor fijo y por días. Herramienta menor como % de la MO.
- Duplicar un APU marca su origen y muestra qué cambió.
- Insumos con precio con IVA, fuente, fecha y marca "estimado sin verificar". Jornales y cuadrillas editables.
- Presupuestos por capítulos, AIU, IVA escogible (no aplica / sobre utilidad / pleno), total redondeado al millar.
- Ítems rápidos para trabajos pequeños y muebles; se pueden pasar a la biblioteca.
- Aprobar congela los precios; volver a borrador los libera.
- PDF para el cliente (texto del presupuesto) y PDF de APU aparte. Nunca salen valores de ejecución.
- Autoguardado, versiones cada 10 minutos (últimas 15) y respaldo en archivo.

## Datos iniciales
`datos-base.json`: 160 insumos, 4 cargos, 8 cuadrillas, 7 APU básicos y 209 APU de actividades (lista aprobada rev4). Lo marcado `est: true` está sin verificar.

## Fases siguientes
2: versiones y opciones de presupuesto, adicionales, precio de ejecución, explosión de insumos hacia Gestión de materiales.
3: importación Revit/IFC con "Código APU", rendimientos reales de la Bitácora y cronograma.

- 23-nov-2026: atrás por niveles (subpágina → elemento → lista o inicio → cierra la app); botón Instalar en el celular.
