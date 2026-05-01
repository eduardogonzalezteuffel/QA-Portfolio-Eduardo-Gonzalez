# Historia de Usuario: Registro de Nuevo Usuario

**ID:** US-001
**Título:** Implementación de registro con validación de seguridad.

### 📝 Descripción
**Como** usuario interesado en el portal,
**Quiero** registrarme mediante un formulario con nombre, email y contraseña,
**Para** acceder a las funcionalidades exclusivas de la plataforma.

### ✅ Criterios de Aceptación
* **Validación de Campos:** El sistema debe impedir el registro si el email no tiene un formato válido (ej: usuario@dominio.com).
* **Seguridad de Contraseña:** La contraseña debe tener un mínimo de 8 caracteres, incluyendo al menos una mayúscula y un número.
* **Feedback de Usuario:** Al completar el registro exitosamente, el sistema debe redirigir al Dashboard en menos de 2 segundos.
* **Manejo de Errores:** Si el email ya existe, el sistema debe mostrar un mensaje de alerta: "Este correo ya se encuentra registrado".

### ⚙️ Notas Técnicas
* La información debe persistir en la base de datos siguiendo los estándares de seguridad.
* Considerar el comportamiento del sistema en condiciones de alta latencia (según reportes de QA previos).
