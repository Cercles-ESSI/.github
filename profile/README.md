# **CERCLES**

## **Descripción del Proyecto**

CERCLES (Creació d'Equips i seguiment del Rendiment i CoL·laboració En projectes d'Enginyeria del Software) es una herramienta diseñada para facilitar la evaluación de las contribuciones individuales en proyectos colaborativos de ingeniería de software. Su principal objetivo es centralizar la información obtenida de GitHub y proporcionar a profesores y estudiantes una visión clara y objetiva de la participación de cada miembro del equipo. Esta solución mejora la transparencia, la equidad y la eficiencia en la evaluación de los proyectos grupales.

---

## **Componentes**

| Repositorio                                     | Nombre                        | Descripción                                          |
|-------------------------------------------------|-------------------------------|------------------------------------------------------|
| [cercles-ESSI-frontend](https://github.com/Cercles-ESSI/cercles-ESSI-frontend)  | CERCLES Frontend              | Frontend de la aplicación CERCLES, desarrollado con React. |
| [cercles-ESSI-backend](https://github.com/Cercles-ESSI/cercles-ESSI-backend)    | CERCLES Backend               | Backend de la aplicación CERCLES, desarrollado con Spring Boot. |

---

---

## **Requisitos de Instalación**

Antes de proceder con la instalación de CERCLES haciendo uso de Docker Compose, asegúrate de cumplir con los siguientes requisitos según tu sistema operativo:

1.**Docker y Docker Compose**:
  
  1.1 En Windows: Descargar e instalar Docker Desktop desde [Docker](https://www.docker.com/products/docker-desktop/).Reinicia el sistema tras completar el proceso.
  
  1.2 En Linux (Ubuntu): Instalar mediante terminal:
  ```bash
    sudo apt-get update
    sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
  ```
  (Opcional: Añade tu usuario al grupo docker con sudo usermod -aG docker $USER para ejecutar comandos sin sudo).
  
2. **IDE** (Opcional para despliegue): Visual Studio Code (VSC) o cualquier otro IDE para proyectos backend y frontend (como IntelliJ o Eclipse).

---

## **Pasos de Instalación**

### **1. Configurar el correo para el primer login**

Edita el archivo `application-secret.properties`, ubicado en `src/main/resources` del proyecto backend.

En este archivo debes definir tu correo de Google y tu nombre para poder entrar la primera vez. Un ejemplo sería: 

```properties
# Reemplazar por el correo de Google con el que harás el primer login
app.initial-email=maryx51202@gmail.com
app.initial-name=Mary Ojuyenum
```

### **2. Iniciar el proyecto**

Inicia el docker  y verifica que la aplicación esté funcionando accediendo a `http://localhost:3030`.

---

## **Documentación**

---

| Archivo                                                      | Nombre                             | Descripción                                                |
|--------------------------------------------------------------|------------------------------------|------------------------------------------------------------|
| [Manual de usuario](https://github.com/cercles-tfg/cercles-tfg-frontend/blob/main/docs/Manual%20de%20usuario.pdf) | Manual de usuario                  | Guía para los usuarios de la aplicación CERCLES, explicando cómo usar las funcionalidades. |
| [Swagger API](https://cercles-essi.github.io/cercles-ESSI-backend/) | Documentación Swagger API           | Acceso al Swagger que describe la API RESTful de CERCLES, creado mediante una GitHub Page |

---

## **Licencia**

This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/cercles-tfg/.github/blob/main/LICENSE) file for details.

---
