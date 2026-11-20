# Política de Privacidad — SmartLobby (`pe.smartlobby.app`)

**Última actualización:** 20 de noviembre de 2026  
**Desarrollador responsable:** Ayrton Neves Estrada (`ayrton.24.6.95@gmail.com`)

---

## 1. Resumen Ejecutivo (Arquitectura por Capas)

- **Capa 1 (Almacenamiento local / offline-first — Activa):** SmartLobby guarda la operación del edificio en una base SQLite del dispositivo. El desarrollador no recibe esos registros en un servidor propio.
- **Capa 2 (Archivos del sistema — Activa):** La importación y exportación de Excel, y la opción de compartir un archivo, ocurren solo cuando la persona que usa la app lo pide. No hay mapas, anuncios ni SDKs de analítica.
- **Capa 3 (Servicios en la nube — Inactiva):** Esta versión no tiene cuenta en la nube, sincronización, notificaciones push ni backend. El modelo de datos está preparado para una versión futura; esta versión no envía la información.
- **Capa 4 (Eliminación — Activa):** Los registros se borran al limpiar el almacenamiento de la app o al desinstalarla. Android no incluye esta app en la copia de seguridad del sistema (`android:allowBackup="false"`).

---

## 2. Quién usa la aplicación

SmartLobby está dirigida al personal de portería, conserjería y administración de un condominio o edificio. No es una app para el público infantil.

Quien opera el edificio introduce datos de residentes, visitas y pagos. Esa persona o la administración del edificio es responsable de tener una base legal para registrar esos datos. El desarrollador de la app no los recibe.

---

## 3. Datos que se guardan en el dispositivo

| Categoría | Ejemplos | ¿Sale a un servidor del desarrollador? | ¿Se comparte con terceros desde la app? |
| :--- | :--- | :--- | :--- |
| Personas del edificio | Nombre, tipo de residente, teléfono, correo | No | No, salvo que quien usa la app exporte o comparta un archivo |
| Documentos de identidad | DNI, carné de extranjería o pasaporte de residentes y visitas | No | Igual que la fila anterior |
| Operación del edificio | Unidades, vehículos, placas, mascotas, visitas, paquetes, incidencias, áreas comunes, reservas | No | Igual que la fila anterior |
| Pagos de mantenimiento | Periodo, medio de pago, número de operación, nombre de quien paga, número de recibo | No | Igual que la fila anterior |
| Fotos de paquetes | Archivo elegido en el dispositivo, si se adjunta | No | No |
| PIN de conserjería y administración | Solo el hash Argon2id y su sal. La app no guarda el PIN en texto plano | No | No |
| Publicidad e identificadores publicitarios | No se usan | No | No |

La app no pide ubicación, contactos del teléfono, micrófono ni cámara como permiso propio. El selector de archivos del sistema se abre solo para importar o adjuntar un archivo que la persona elige.

---

## 4. Archivos Excel y compartir

Quien administra el edificio puede importar un `.xlsx` del directorio o de las áreas comunes, y exportar o compartir ese archivo con las aplicaciones que elija en el dispositivo. A partir de ese momento, el destino del archivo lo decide esa persona, no SmartLobby.

---

## 5. Eliminación

En esta versión no hay un botón dentro de la app que borre toda la base. Para eliminar los datos locales:

- Ajustes de Android → Aplicaciones → SmartLobby → Almacenamiento → Borrar datos, o
- Desinstalar la aplicación.

Para una consulta sobre privacidad, escribe a [ayrton.24.6.95@gmail.com](mailto:ayrton.24.6.95@gmail.com).

---

## 6. Contacto

- **Desarrollador:** Ayrton Neves Estrada
- **Correo electrónico:** [ayrton.24.6.95@gmail.com](mailto:ayrton.24.6.95@gmail.com)
- **Paquete Android:** `pe.smartlobby.app`
