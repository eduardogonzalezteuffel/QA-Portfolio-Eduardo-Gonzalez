# Reporte de Defecto: Error de Concurrencia en Registro

**📝ID:** TC-001

### Descripción del problema
Al cliquear más de una vez el botón "registrate", el sistema no redirecciona y arroja error al momento de la redirección.

### Pasos para reproducir:
1. Abrir el portal: https://talentolab-test.netlify.app/
2. Cliquear el botón "Registrate" consecutivamente

### Resultados
* **Resultado esperado:** Redireccionar a la sección de completar datos de nuevo usuario.
* **Resultado obtenido:** El sistema arroja un modal de error al momento de redireccionar.

### Clasificación
* **Severidad:** Alta (Riesgo de abandono del portal y falta de seguridad percibida).
* **Prioridad:** Alta (Afecta la conversión de nuevos usuarios).

### Entorno
* **SO:** Windows 10/11
* **Navegadores:** Chrome, Mozilla y Safari

---

# Reporte de Defecto: Error de en Registro sin acceso a internet

**📝ID:** TC-002

### Descripción del problema
Al cliquear el boton "registrate" el sistema no muestra modal de aviso error sin conexion

### Pasos para reproducir:
1. Abrir el portal https://talentolab-test.netlify.app/ 
2. Desactivar el acceso a internet del dispositivo
3. Cliquear el boton "Registrate" 
4. Al desplazarse por el Home Page (no se muestra sintomas de estar sin conexion).

### Resultados
* **Resultado esperado:** Despliegue de modal de aviso con mensaje de Alerta "sin conexion a internet".
* **Resultado obtenido:** El sistema no despliega modal de alerta con mensaje "sin conexion a internet".

### Clasificación
* **Severidad:** Media (ya que esto puede hacer que los usuarios no esten concientes de la falta de conexion y abandonen el sitio).
* **Prioridad:** Alta (Esto podria oacionar que los usuarios abandonen en sitio al no estar al tanto de la falta de conexion).

### Entorno
* **SO:** Windows 10/11
* **Navegadores:** Chrome, Mozilla y Safari

* ---

* # Reporte de Defecto: Latencia excesiva en la redireccion del boton "Registrate"

**📝ID:** TC-003

### Descripción del problema
Al cliquear el boton "Registrate" el sistema redirecciona pasados los 10 segundos

### Pasos para reproducir:
1. Abrir el portal https://talentolab-test.netlify.app/ 
2. Cliquear el boton "Registrate" 
3. Cronometrar el tiempo de respuesta desde el clic hasta la redireccion 


### Resultados
* **Resultado esperado:** El sistema redirecciona en menos de 1 segundo.
* **Resultado obtenido:** El sistema redirecciona pasados los 10 segundos.

### Clasificación
* **Severidad:** Media (esto ocasiona una espera larga para que se ejecute la accion esperada).
* **Prioridad:** Media (esto impactaria en la paciencia del usuario y ocasionaria la ejecucion de la accion por parte de los usuarios en multiples intentos
* o abandono del sitio por parte de los usuarios).

### Entorno
* **SO:** Windows 10/11
* **Navegadores:** Chrome, Mozilla y Safari

