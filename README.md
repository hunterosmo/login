# Sistema de Login con jBCrypt

**Creado por:** Hunterosmo

## Credenciales de Acceso
- **Usuario:** admin
- **Clave:** 123

---

## Descripción del Proyecto

Este es un proyecto de sistema de login que implementa autenticación segura utilizando las siguientes tecnologías:

### Stack Tecnológico
- **Librería de encriptación:** jBCrypt-0.4.1.jar
- **IDE:** NetBeans 8.2
- **Framework UI:** PrimeFaces
- **ORM:** Hibernate
- **Servidor de aplicaciones:** GlassFish Server 4.1.1

---

## ¿Qué es jBCrypt?

La biblioteca **jBCrypt** (Java BCrypt) es una implementación del algoritmo BCrypt para Java, diseñada específicamente para el almacenamiento seguro de contraseñas.

### Características Principales del Algoritmo BCrypt

#### **Seguridad Avanzada**
BCrypt utiliza un esquema de "costo de trabajo" adaptable que permite ajustar la complejidad computacional del proceso de hash. Esto hace que sea extremadamente resistente a:
- Ataques de fuerza bruta
- Ataques de diccionario
- Búsqueda de colisiones

#### **Salt Automático**
- Incorpora automáticamente un "salt" (sal) único y aleatorio para cada contraseña
- El salt se agrega antes de calcular el hash, proporcionando una capa adicional de seguridad
- Previene eficazmente los ataques de tabla arcoíris

---

## Funcionalidades de jBCrypt

### Métodos Principales

#### `hashpw(String password, String salt)`
- **Propósito:** Genera un hash BCrypt seguro de la contraseña
- **Parámetros:** 
  - `password`: Contraseña en texto plano
  - `salt`: Valor salt para el hash
- **Retorna:** Hash BCrypt de la contraseña

#### `checkpw(String candidate, String hashed)`
- **Propósito:** Verifica si una contraseña coincide con un hash almacenado
- **Parámetros:**
  - `candidate`: Contraseña a verificar
  - `hashed`: Hash almacenado en la base de datos
- **Retorna:** `true` si coincide, `false` en caso contrario

---

## Ventajas de Implementación

### **Facilidad de Uso**
- Proporciona una API simple y directa para desarrolladores Java
- Integración sencilla con frameworks existentes como Hibernate y PrimeFaces

### **Compatibilidad**
- Totalmente compatible con aplicaciones web Java
- Funciona perfectamente con servidores de aplicaciones como GlassFish

### **Seguridad Robusta**
- Eliminación de la necesidad de implementar algoritmos de hash personalizados
- Almacenamiento seguro en bases de datos sin exponer contraseñas en texto plano

---

## Casos de Uso Comunes

- **Aplicaciones web empresariales**
- **Sistemas de gestión de usuarios**
- **Plataformas de e-commerce**
- **APIs REST con autenticación**
- **Aplicaciones móviles con backend Java**

---

## Versión Utilizada: jBCrypt-0.4.1.jar

Esta versión específica incluye:
- ✅ Correcciones de errores de versiones anteriores
- ✅ Optimizaciones de rendimiento
- ✅ Actualizaciones de seguridad
- ✅ Compatibilidad mejorada con Java 8+

---

## Conclusión

La implementación de jBCrypt-0.4.1.jar en este proyecto proporciona una solución robusta y confiable para la autenticación de usuarios. Su integración con NetBeans, PrimeFaces, Hibernate y GlassFish Server crea un ecosistema completo y seguro para el manejo de credenciales de usuario, protegiendo contra las amenazas de seguridad más comunes en aplicaciones web modernas.
