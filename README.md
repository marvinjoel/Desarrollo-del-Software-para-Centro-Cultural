# Cotización y Plan de Desarrollo del Software para Centro Cultural

## Visión General
El objetivo es desarrollar un sistema de gestión integral para un centro cultural que incluye módulos para talleres, teatro, cine y alquileres. El software automatizará el registro de alumnos/clientes, la gestión de detalles de pagos y generará reportes analíticos, reemplazando el uso actual de Excel y formularios de Facebook. Se utilizará Java spring boot o Python con FastAPI como BackEnd y en diseño para la web se trabajara con React como FrontEnd, con integración de una API de RENIEC para validación de datos personales. El proyecto se completará en 3 meses, con un enfoque inicial en un MVP que se expandirá según necesidades.

**Notas Importantes:**
- El costo del hosting, dominio y la API de RENIEC no está incluido en esta cotización. Estos son gastos que el cliente debe asumir directamente. Detalles a continuación.

## Plazo y Cotización
- **Duración Estimada**: 3 meses (a partir del "la fecha acordada").
- **Horas Estimadas**: 240-300 horas (80-100 horas/mes, asumiendo 20-25 horas semanales).
- **Costo Total**: .....).
  - **Mes 1**: $0-$0 USD (Fase 1: Configuración y desarrollo inicial).
  - **Mes 2**: $0-$0 USD (Fase 2: Despliegue e integración).
  - **Mes 3**: $0-$0 USD (Fase 3: Pruebas, optimización y documentación).
- **Pagos**: 50% al inicio, 30% a mitad del proyecto, 20% al finalizar (sujeto a acuerdo).

## Tareas a Realizar en el Software
### Fase 1: Fundación y Configuración (Mes 1)
- **Tarea 1.1: Configuración del Entorno de Desarrollo Local**
  - Elegir y configurar un stack con Java sping boot o Python y FastAPI.
  - Instalar PostgreSQL localmente para desarrollo y pruebas.
  - Estructurar el proyecto con separación de rutas, controladores y servicios.
- **Tarea 1.2: Integración con API de RENIEC**
  - Investigar y configurar la API de RENIEC para validar datos personales de alumnos/clientes.
  - Crear un script de prueba para conectar y obtener datos básicos (ej. nombres y DNI).
  - Entregable: Confirmación de conexión exitosa con la API de RENIEC.
- **Tarea 1.3: Desarrollo del Endpoint de Registro de Alumnos (POST /inscribir-alumno)**
  - Crear ruta y controlador para registrar alumnos via formulario en línea.
  - Implementar lógica para validar datos con la API de RENIEC y guardar en PostgreSQL.
  - Entregable: Endpoint funcional que registra alumnos con datos validados.
- **Tarea 1.4: Desarrollo del Endpoint de Registro de Pagos (POST /registrar-pago)**
  - Crear ruta y controlador para registrar pagos (matrícula, mensualidades, entradas).
  - Validar datos y actualizar estado (pagado, pendiente, deuda).
  - Entregable: Endpoint funcional que gestiona pagos y muestra deudas.

### Fase 2: Despliegue e Integración (Mes 2)
- **Tarea 2.1: Dockerizar la API**
  - Crear un Dockerfile para la aplicación.
  - Configurar un archivo docker-compose.yml para orquestar servicios.
  - Entregable: Dockerfile y docker-compose.yml listos para despliegue.
- **Tarea 2.2: Despliegue Inicial en el VPS**
  - Conectar al VPS proporcionado por el cliente.
  - Levantar contenedores con docker-compose up -d.
  - Entregable: API corriendo en el VPS.
- **Tarea 2.3: Configuración de Nginx como Reverse Proxy**
  - Instalar Nginx y configurar subdominios (ej. talleres.dominio.com).
  - Redirigir tráfico al puerto interno de la API.
  - Entregable: Servicios accesibles via subdominios.
- **Tarea 2.4: Implementación de SSL/TLS**
  - Usar Certbot para obtener certificados SSL de Let's Encrypt.
  - Configurar renovación automática.
  - Entregable: Conexiones seguras (HTTPS).

### Fase 3: Pruebas y Soporte (Mes 3)
- **Tarea 3.1: Colaboración en Pruebas End-to-End**
  - Monitorear logs mientras se prueban flujos con formularios y pagos.
  - Solucionar bugs y optimizar errores detectados.
- **Tarea 3.2: Optimización y Monitoreo**
  - Verificar rendimiento (CPU, memoria) y optimizar consultas si es necesario.
  - Asegurar que el sistema funcione como esperado.
- **Tarea 3.3: Documentación de la API**
  - Crear documentación con Swagger/OpenAPI o un README.md.
  - Detallar endpoints, parámetros y estructura de datos devueltos.
  - Entregable: Documentación técnica completa.

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
