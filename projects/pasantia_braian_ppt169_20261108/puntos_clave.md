# Puntos clave — Informe de Pasantía (Braian Moreno)

**Propuesta de un sistema de gestión de mantenimiento preventivo para los equipos de refrigeración de CVG Ferrominera Orinoco, C.A.**
UNEG · Ingeniería Industrial · Ciudad Guayana, noviembre 2026
Tutor industrial: Ing. Jorge Rosas · Tutor académico: Ing. Yuswaldo Silva

---

## 01 · Portada
- Sistema de gestión de mantenimiento preventivo
- Equipos de refrigeración · CVG Ferrominera Orinoco
- Br. Braian Moreno · UNEG

## 02 · El problema
- El sistema SAP dejó de funcionar.
- Datos dispersos en WhatsApp y hojas de cálculo.
- Sin historial por equipo.
- Sin indicadores de confiabilidad.
- **Se registra que se trabajó, no qué le pasa a cada equipo.**

## 03 · Objetivo
- Proponer un sistema de gestión de mantenimiento preventivo para los equipos de refrigeración de FMO.
- Alcance: diagnóstico, diseño y propuesta. No incluye implantación definitiva.

## 04 · Ruta de trabajo
1. Diagnóstico
2. Inventario
3. Criticidad
4. Plan preventivo
5. Indicadores
6. Herramienta digital + socialización

## 05 · Diagnóstico (Ishikawa)
- **Métodos:** preventivo solo marca "hecho" (M / 1), no el estado del equipo.
- **Información:** refrigeración mezclada con electricidad; evidencias en el chat.
- **Medición:** solo desempeño y satisfacción; sin MTBF, MTTR ni disponibilidad.
- **Trazabilidad:** avisos por solicitante, no por equipo; preventivo y correctivo desconectados.

## 06 · Inventario
- Punto de partida: Extraplan FERRO-5479 (~457 equipos).
- Depurado con inspecciones, mantenimientos y reportes de falla.
- **671 equipos · 36 áreas.**
- Split 536 · Ventana 94 · Otro 23 · Central 17 · Cava 1.
- Ficha técnica única por equipo (código, tipo, área, refrigerante, criticidad, frecuencia).

## 07 · Criticidad
- Encuesta al jefe del departamento (26 años de servicio), 37 áreas evaluadas.
- **A · Alta:** 7 áreas · 173 equipos — operación y áreas sensibles.
- **B · Media:** 24 áreas · 446 equipos — confort del personal.
- **C · Baja:** 6 áreas · 52 equipos — menor impacto.
- Cada equipo hereda la criticidad de su área.

## 08 · Plan preventivo
- Frecuencia según tipo y criticidad: más atención a la criticidad A.
- Checklist de 15 tareas por tipo: split, ventana, central, cava.
- Filtros, serpentines, refrigerante, temperaturas, conexiones eléctricas.
- El checklist se integra al módulo Registrar.

## 09 · Indicadores
- Cumplimiento = ejecutados ÷ programados × 100
- MTBF = tiempo de operación ÷ n.º de fallas
- MTTR = horas fuera de servicio ÷ n.º de reparaciones
- Disponibilidad = MTBF ÷ (MTBF + MTTR)
- λ = 1 ÷ MTBF
- R(t) = e^(−λt)

## 10 · Herramienta TPM FMO · Refrigeración
- Aplicación web en la nube: celular o PC, sin instalar nada.
- Datos compartidos en tiempo real.
- Módulos: Tablero · Equipos · Registrar · Jornadas · Diario · Análisis.

## 11 · Resultados
- Cumplimiento del plan preventivo: **70,1 %** (tablero de Análisis).
- Pareto: 4 causas ≈ **80 %** del tiempo fuera de servicio.
- Fuga de refrigerante 197 h · Compresor 152 h · Contactor 134 h · Breaker 124 h.
- Además controla el consumo de refrigerante y los repuestos.

## 12 · Conclusiones
- Objetivo cumplido: una sola base de datos.
- Inventario depurado y clasificado.
- Indicadores calculados de forma automática.
- Socialización con recepción favorable.

## 13 · Recomendaciones
- Adoptar TPM FMO de forma progresiva.
- Completar el año de instalación de cada equipo.
- Registrar las lecturas de temperatura.
- Priorizar los preventivos vencidos de criticidad A.
- Atacar las causas vitales del Pareto.
- Avanzar hacia TPM e ISO 55001:2024.

## 14 · Cierre
- Gracias · ¿Preguntas?

---

## Transiciones configuradas (`animations.json`)
- **Morph (Transformación)** en todas las diapositivas, 0,8 s.
- Objeto continuo `!!avance`: el panel azul de la portada se encoge hasta convertirse en la barra de progreso superior. Avanza en cada diapositiva y vuelve a expandirse en el cierre.
- Sin animaciones de objeto: cada diapositiva aparece completa.
