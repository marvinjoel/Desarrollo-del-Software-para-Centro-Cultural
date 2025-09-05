# Cotización y Plan de Desarrollo del Software para Centro Cultural

## Visión General
El objetivo es desarrollar un sistema de gestión integral para un centro cultural que incluye módulos para talleres, teatro, cine y alquileres. El software automatizará el registro de alumnos/clientes, la gestión de pagos y generará reportes analíticos, reemplazando el uso actual de Excel y formularios de Facebook. Se utilizará Java, con integración de una API de RENIEC para validación de datos personales. El proyecto se completará en 3 meses, con un enfoque inicial en un MVP que se expandirá según necesidades.

**Notas Importantes:**
- El costo del hosting, dominio y la API de RENIEC no está incluido en esta cotización. Estos son gastos que el cliente debe asumir directamente. Detalles a continuación.

## Plazo y Cotización
- **Duración Estimada**: 3 meses.
- **Horas Estimadas**: 300 horas (100 horas/mes).
- **Costo Total**: $1,800 USD.
  - **Inicial**: $900 (50% al inicio del proyecto).
  - **Intermedio**: $540 (30% a mitad del proyecto).
  - **Final**: $360 (20% al finalizar el proyecto).
- **Pagos**: Según los hitos indicados (sujeto a acuerdo).

## Tareas a Realizar en el Software
### Fase 1: Desarrollo Inicial (Mes 1)
- Configurar un sistema robusto para registrar alumnos en talleres, validando sus datos personales mediante la API de RENIEC.
- Implementar un módulo para registrar y gestionar pagos de matrícula y mensualidades, con actualización automática de deudas pendientes.
- Crear un sistema de inscripción en línea donde los alumnos completen formularios y sus datos se integren directamente al software.
- Entregable: Un módulo funcional para inscripción y gestión de pagos de talleres.

### Fase 2: Expansión y Lanzamiento (Mes 2)
- Ampliar el sistema para incluir registro de clientes y ventas de entradas para teatro y cine, con gestión de pagos asociada.
- Lanzar el software en un entorno de producción accesible para su uso, asegurando una experiencia segura y fluida.
- Configurar un sistema de formularios en línea para compras de entradas, integrando los datos automáticamente.
- Entregable: Módulos completos para teatro, cine y un sistema en producción listo para uso.

### Fase 3: Optimización y Reportes (Mes 3)
- Realizar pruebas finales con el cliente para asegurar que todo funcione correctamente y resolver cualquier problema.
- Optimizar el rendimiento del sistema y monitorear su uso para garantizar una experiencia eficiente.
- Desarrollar reportes detallados de ingresos y análisis por período, con filtros por módulos (talleres, teatro, cine).
- Crear una documentación clara para que el cliente pueda usar y mantener el software fácilmente.
- Entregable: Sistema optimizado, reportes funcionales y documentación completa.

## Reportes e Indicadores
- El software incluirá reportes de ingresos filtrables por día, mes o año, con prioridad en análisis mensual.
- Se podrán generar filtros específicos por módulo (talleres, teatro, cine) para evaluar el rendimiento de cada actividad.
- Los reportes ofrecerán estadísticas analíticas, como totales de ingresos y tendencias, para apoyar la toma de decisiones.

## Costos Adicionales a Cargo del Cliente
### Hosting y Dominio
- El hosting y el dominio (ej. VPS, servidor dedicado) no están incluidos en la cotización.
- El cliente debe contratar y configurar un proveedor (ej. AWS, DigitalOcean, o local en Perú) con un costo estimado de $5-20 USD/mes, dependiendo del plan.

### API de RENIEC
- La integración con la API de RENIEC requiere un paquete de peticiones según el volumen de usuarios. Los costos anuales son:
  - **Free**: PEN 0,00 (1,000 peticiones/mensuales).
  - **10K**: PEN 50,00 (10,000 peticiones/mensuales).
  - **30K**: PEN 80,00 (30,000 peticiones/mensuales).
  - **50K**: PEN 100,00 (50,000 peticiones/mensuales).
  - **75K**: PEN 150,00 (75,000 peticiones/mensuales).
  - **100K**: PEN 200,00 (100,000 peticiones/mensuales).
  - **150K**: PEN 300,00 (150,000 peticiones/mensuales).
  - **200K**: PEN 400,00 (200,000 peticiones/mensuales).
- **Recomendación**: Evaluar el número de alumnos/clientes mensuales para elegir el paquete adecuado. Por ejemplo, para 500-1,000 usuarios/mes, el paquete "10K" (PEN 50,00/año) debería ser suficiente inicialmente.

## Notas Finales
- La cotización asume un desarrollo a tiempo parcial (20-25 horas/semana). Ajustes en el plazo o costo pueden negociarse.
- Se recomienda una reunión inicial para confirmar detalles técnicos (ej. acceso al VPS, volumen de usuarios).
- El proyecto incluye un MVP funcional al final del Mes 1, con expansiones en Meses 2 y 3.

Este documento se actualizará según feedback del cliente o cambios en el alcance.
