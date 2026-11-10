# Política de Privacidad — TusPlanes (`pe.tusplanes.mobile`)

**Última actualización:** 10 de noviembre de 2026  
**Desarrollador responsable:** Ayrton Neves Estrada (`ayrton.24.6.95@gmail.com`)

---

## 1. Resumen Ejecutivo (Arquitectura por Capas)

- **Capa 1 (Almacenamiento Local / Offline-First — Activa):** En la versión 1.0, **TusPlanes** funciona 100% offline. No recopila, no transmite ni comparte datos personales del usuario con servidores externos ni con terceros.
- **Capa 2 (Integraciones Nativas del Sistema — Activa):** La apertura de ubicaciones utiliza la aplicación de Mapas ya integrada en el dispositivo móvil mediante intents estándar (`geo:`), sin usar claves de rastreo ni almacenar historial de ubicación en servidores.
- **Capa 3 (Servicios en la Nube — Inactiva en v1.0):** El backend no está habilitado en esta versión inicial.
- **Capa 4 (Eliminación de Datos — Activa):** El usuario puede eliminar instantáneamente todos sus planes guardados localmente desde el menú **"Privacidad y Seguridad de Datos (Play) > Eliminar mis planes locales"** dentro de la app o desinstalando la aplicación.

---

## 2. Datos Recopilados y Compartidos

| Categoría de Datos | ¿Se recopila en servidores externos? | ¿Se comparte con terceros? | Uso en el dispositivo |
| :--- | :--- | :--- | :--- |
| Información personal (Nombre, Correo, Teléfono) | **No** | **No** | No se solicita |
| Planes guardados ("Mis Planes") | **No** | **No** | Guardado únicamente en almacenamiento local del teléfono |
| Ubicación / Mapas | **No** | **No** | Solo abre la app de Mapas integrada del dispositivo cuando el usuario lo solicita |
| Identificadores publicitarios / Anuncios | **No** | **No** | La aplicación no contiene anuncios |

---

## 3. Contacto

Para cualquier duda o consulta relacionada con la privacidad en **TusPlanes** o cualquiera de los proyectos asociados a este repositorio:

- **Desarrollador:** Ayrton Neves Estrada
- **Correo electrónico:** [ayrton.24.6.95@gmail.com](mailto:ayrton.24.6.95@gmail.com)
