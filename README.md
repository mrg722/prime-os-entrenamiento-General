# Prime OS · Strength Operating System V4.0

Prime OS público transforma días, objetivo, nivel, tiempo, énfasis y ejercicios a evitar en una propuesta de rutina editable y después registra la ejecución real.

## V4.0 — auditoría y mejoras

### Flujo principal
Anamnesis → propuesta → bloque de hoy → registro por serie → descanso → historial → progreso.

### Motor de propuesta
- 1–3 días: Full Body.
- 4 días: Torso / Pierna.
- 5 días: Upper / Lower + Push / Pull.
- 6 días: Push / Pull / Legs × 2.
- El objetivo modifica series, repeticiones, RPE y descanso.
- El tiempo limita la cantidad de ejercicios.
- El énfasis modifica los patrones prioritarios.
- Los ejercicios a evitar se excluyen cuando es posible.
- La propuesta siempre queda editable.

La actualización 2026 de ACSM enfatiza consistencia, individualización y adaptar carga/volumen al objetivo. Fuente: https://acsm.org/resistance-training-guidelines-update-2026/

### Registro
- Peso y reps editables con teclado.
- KG / LB.
- Enter para registrar.
- RPE y descanso.
- Volumen y PR/e1RM.
- Última ejecución visible.
- Los ejercicios de peso corporal aceptan 0 kg.
- Cada serie V4 queda en setsLog con ejercicio, set, kg internos, unidad mostrada, reps, RPE y fecha.

### Dashboard
Se conserva la composición tipo centro de control: próxima sesión, señal de fuerza, estadísticas all-time, carga de 7 días, sesiones recientes y cobertura muscular. El hero del día se conecta con el ejercicio real cuando existe una imagen disponible.

### Móvil
Navegación rápida: Inicio · Entrenar · Rutina · Progreso · 1RM.

### Carta de presentación
La sección personalizada de Martin Reyes se mantiene con WhatsApp, correo y propuesta de planificación individual.

### Biblioteca y media
Prime OS utiliza el dataset público hasaneyldrm/exercises-dataset cuando está disponible. El propio repositorio declara 1.324 ejercicios con imágenes/GIFs y especifica que la media es © Gym visual y está sujeta a condiciones de reutilización:
https://github.com/hasaneyldrm/exercises-dataset

## Bugs lógicos auditados

Corregidos:
1. El generador ignoraba el énfasis.
2. El generador ignoraba ejercicios a evitar.
3. El tiempo no limitaba la cantidad de movimientos.
4. La lógica de objetivos era demasiado plana.
5. Los ejercicios de peso corporal podían ser rechazados por usar 0 kg.
6. No se mostraba contexto de la última ejecución al registrar.
7. El historial era demasiado agregado; V4 conserva datos por serie.
8. El dashboard no conectaba su hero al ejercicio real del día.
9. En móvil el acceso al entrenamiento dependía demasiado del menú lateral.

Conservado:
- 1RM Epley.
- Historial.
- Progreso.
- Importación/exportación.
- Biblioteca.
- Anamnesis.
- Rutina editable.
- PWA.
- Datos locales.
- Carta de presentación.

## Referencias UX
Se contrastó el flujo con patrones actuales de apps de entrenamiento: acceso directo a Today, logging por serie, peso/reps/RPE, descanso, última sesión y progreso histórico.

https://setforward.app/
https://www.tracked.gg/features/workout-tracking

## Estado
Prime OS V4.0 — aplicado directamente sobre main.

Repositorio: mrg722/prime-os-entrenamiento-General
Web: https://mrg722.github.io/prime-os-entrenamiento-General/
