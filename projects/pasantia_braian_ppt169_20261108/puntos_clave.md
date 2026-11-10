# Puntos clave — Informe de Pasantía (Braian Moreno)

**Propuesta de un sistema de gestión de mantenimiento preventivo para los equipos de refrigeración de CVG Ferrominera Orinoco, C.A.**
UNEG · Ingeniería Industrial · Ciudad Guayana, noviembre 2026
Tutor industrial: Ing. Jorge Rosas · Tutor académico: Ing. Yuswaldo Silva

---

## 01 · Portada
- Sistema de gestión de mantenimiento preventivo
- Equipos de refrigeración · CVG Ferrominera Orinoco
- Br. Braian Moreno · UNEG

## 02 · Introducción
- **La empresa:** CVG Ferrominera Orinoco extrae, procesa y vende mineral de hierro. Es estatal, está activa desde 1976 en el estado Bolívar, tiene las plantas PMH, Pellas y Briquetas, y es el principal proveedor de la siderurgia nacional.
- **La unidad:** Supervisión de Refrigeración Industrial (Gerencia de Servicios, Dpto. de Servicios Industriales), con 21 posiciones y 14 técnicos de frío.
- **La pasantía:** Ingeniería Industrial, UNEG. Tutores: Ing. Jorge Rosas (industrial) e Ing. Yuswaldo Silva (académico). Plan de 9 actividades; el alcance es una propuesta, no la implantación.
- El preventivo solo es efectivo si se **ejecuta, registra, sigue y mide**.
- La refrigeración protege al personal, los documentos, los equipos sensibles y los procesos. En FMO el parque es numeroso y disperso y el control era informal.
 · El problema
- El sistema SAP dejó de funcionar.
- Datos dispersos en WhatsApp y hojas de cálculo.
- Sin historial por equipo.
- Sin indicadores de confiabilidad.
- **Se registra que se trabajó, no qué le pasa a cada equipo.**

## 04 · Objetivo
- Proponer un sistema de gestión de mantenimiento preventivo para los equipos de refrigeración de FMO.
- Alcance: diagnóstico, diseño y propuesta. No incluye implantación definitiva.

## 05 · Ruta de trabajo
1. Diagnóstico
2. Inventario
3. Criticidad
4. Plan preventivo
5. Indicadores
6. Herramienta digital + socialización

## 06 · Diagnóstico (Ishikawa)
- **Métodos:** preventivo solo marca "hecho" (M / 1), no el estado del equipo.
- **Información:** refrigeración mezclada con electricidad; evidencias en el chat.
- **Medición:** solo desempeño y satisfacción; sin MTBF, MTTR ni disponibilidad.
- **Trazabilidad:** avisos por solicitante, no por equipo; preventivo y correctivo desconectados.

## 07 · Inventario
- Punto de partida: Extraplan FERRO-5479 (~457 equipos).
- Depurado con inspecciones, mantenimientos y reportes de falla.
- **671 equipos · 36 áreas.**
- Split 536 · Ventana 94 · Otro 23 · Central 17 · Cava 1.
- Ficha técnica única por equipo (código, tipo, área, refrigerante, criticidad, frecuencia).

## 08 · Criticidad (incluye el Cuadro 3 completo)
- **A:** Gerencia de Calidad, Planta de Briquetas, PMH, Agencia de Buques (Muelle), Ferrocarril, Telemática, Control Central.
- **C:** Desarrollo Endógeno, Centro Cívico, Estadio, C-11, Comisariato, Portón Principal.
- **B:** las 24 áreas restantes, todas listadas en la diapositiva.
- Encuesta al jefe del departamento (26 años de servicio), 37 áreas evaluadas.
- **A · Alta:** 7 áreas · 173 equipos — operación y áreas sensibles.
- **B · Media:** 24 áreas · 446 equipos — confort del personal.
- **C · Baja:** 6 áreas · 52 equipos — menor impacto.
- Cada equipo hereda la criticidad de su área.

## 09 · Plan preventivo (incluye el Cuadro 5 completo)
- Tabla de 15 tareas × 4 tipos de equipo; tareas por tipo: split 12, ventana 11, central 13, cava 13.
- Frecuencia según tipo y criticidad: más atención a la criticidad A.
- Checklist de 15 tareas por tipo: split, ventana, central, cava.
- Filtros, serpentines, refrigerante, temperaturas, conexiones eléctricas.
- El checklist se integra al módulo Registrar.

## 10 · Indicadores
- Cumplimiento = ejecutados ÷ programados × 100
- MTBF = tiempo de operación ÷ n.º de fallas
- MTTR = horas fuera de servicio ÷ n.º de reparaciones
- Disponibilidad = MTBF ÷ (MTBF + MTTR)
- λ = 1 ÷ MTBF
- R(t) = e^(−λt)

## 11 · Herramienta TPM FMO · Refrigeración
- Aplicación web en la nube: celular o PC, sin instalar nada.
- Datos compartidos en tiempo real.
- Módulos: Tablero · Equipos · Registrar · Jornadas · Diario · Análisis.

## 12–17 · Recorrido por módulos (con capturas)
- **Tablero (Fig. 7):** alertas por área; urgentes, próximos, temperatura y pendientes.
- **Equipos (Fig. 8):** inventario por área y alta de equipos; ficha con tipo, capacidad, refrigerante, ubicación, criticidad y frecuencia. Es la base de datos de todo el sistema.
- **Registrar (Fig. 9):** correctivos con causa de falla, horas fuera de servicio y refrigerante cargado; preventivos con checklist; temperaturas; repuestos.
- **Jornadas (Fig. 10):** varios equipos de un área en una sola operación.
- **Diario (Fig. 11):** todo lo atendido en una fecha.
- **Análisis (Fig. 12):** MTBF, MTTR, disponibilidad, Pareto, refrigerante y repuestos.

## 18–20 · Más vistas del sistema
- **Confiabilidad del parque (Fig. 14):** MTBF 866 d · MTTR 10,5 h · disponibilidad 99,9 % · confiabilidad a 30 días 96,6 % · 0,42 fallas por equipo al año. 72 fallas en 693 equipos en 90 días. Muestra los equipos reincidentes, candidatos a intervención de fondo o reemplazo.
- **Refrigerante (Fig. 15):** las recargas repetidas señalan una posible fuga crónica.
- **Repuestos (Fig. 16):** insumo directo para las compras del almacén.
- **Historial (Fig. 17):** 276 atenciones (203 preventivos y 73 correctivos).
- **Equipos instalados (Fig. 18):** 56 equipos instalados en sustitución de otros.

## 21 · Resultados
- Cumplimiento del plan preventivo: **70,1 %** (tablero de Análisis).
- Pareto: 4 causas ≈ **80 %** del tiempo fuera de servicio.
- Fuga de refrigerante 197 h · Compresor 152 h · Contactor 134 h · Breaker 124 h.
- Además controla el consumo de refrigerante y los repuestos.

## 22 · Conclusiones
- Objetivo cumplido: una sola base de datos.
- Inventario depurado y clasificado.
- Indicadores calculados de forma automática.
- Socialización con recepción favorable.

## 23 · Conclusión general
- FMO dispone hoy de una base ordenada e indicadores objetivos para medir su mantenimiento de frío y respaldar decisiones.
- **Aporte a la empresa:** 671 equipos en una sola base de datos, criticidad por área, plan con checklist, indicadores y Pareto automáticos, y TPM FMO lista para adoptarse.
- **Facilidades:** acompañamiento del departamento, un jefe con 26 años de experiencia, acceso a las áreas y el Extraplan como punto de partida.
- **Dificultades:** pérdida del SAP, inventario desactualizado, personal limitado frente al parque y fugas recurrentes.
 · Recomendaciones
- Adoptar TPM FMO de forma progresiva.
- Completar el año de instalación de cada equipo.
- Registrar las lecturas de temperatura.
- Priorizar los preventivos vencidos de criticidad A.
- Atacar las causas vitales del Pareto.
- Avanzar hacia TPM e ISO 55001:2024.

## 25 · Cierre
- Gracias · ¿Preguntas?

---

## Transiciones y animaciones (`animations.json`)
- **Morph (Transformación)** en todas las diapositivas, 0,8 s, con dos objetos continuos:
  - `!!avance`: el panel de la portada se convierte en la barra de progreso y vuelve a expandirse en el cierre.
  - `!!modulo`: el resaltado del módulo activo recorre la lista del 11 al 17.
- **Entradas por objeto** en las 25 diapositivas, en cascada automática (no requieren clic): desvanecer, desplazar, barrido y zoom según el contenido.
- **Salidas en el recorrido de módulos (12–16):** al hacer clic, la captura sale hacia la izquierda; la del siguiente módulo entra por la derecha (efecto carrusel). En esas diapositivas el primer clic retira la captura y el segundo avanza.
