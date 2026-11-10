# 🛡️ Privacy Policies Hub (`privacy-policies`)

Repositorio centralizado y modular (arquitectura por capas) de **Políticas de Privacidad** y **Términos de Uso de Datos** para aplicaciones móviles (Google Play Store / Apple App Store) y plataformas web.

## 🌐 Estructura por Capas (Multi-Proyecto)

Este repositorio funciona como **eje central** para múltiples proyectos mediante una arquitectura de privacidad por capas:

- **Capa 1 — Base Local / Offline-First**: Aplicaciones que procesan y almacenan información exclusivamente en el dispositivo del usuario sin transmitir datos personales a servidores externos.
- **Capa 2 — Integraciones Nativas del Sistema**: Uso bajo demanda de aplicaciones del sistema operativo (Mapas integrados del dispositivo, navegador externo, compartir) sin SDKs de rastreo.
- **Capa 3 — Servicios en la Nube y Sincronización (Opcional por proyecto)**: Autenticación, respaldo en la nube y notificaciones push cuando el proyecto lo habilite.
- **Capa 4 — Eliminación y Control de Datos (Data Safety)**: Mecanismos claros dentro de la aplicación y canales de contacto directo para eliminación de datos locales o remotos.

---

## 📱 Proyectos Activos

| Proyecto | Identificador / Paquete | Estado | Enlace directo de Política de Privacidad |
| :--- | :--- | :--- | :--- |
| **TusPlanes** | `pe.tusplanes.mobile` | Producción / v1.0 Offline | [`/tusplanes/`](./tusplanes/index.html) · [`tusplanes/PRIVACY_POLICY.md`](./tusplanes/PRIVACY_POLICY.md) |
| **Plantilla Base Multi-Proyecto** | `pe.<proyecto>.app` | Plantilla Reutilizable | [`/template/`](./template/index.html) |

---

## 🚀 Cómo agregar un nuevo proyecto

1. Duplica la carpeta [`template/`](./template/) con el nombre corto de tu nuevo proyecto (por ejemplo, `mi-nueva-app/`).
2. Edita `mi-nueva-app/index.html` activando únicamente las capas que apliquen a esa versión (Capa 1 Offline, Capa 2 Integraciones, Capa 3 Nube, etc.).
3. Agrega el enlace en la tabla de este `README.md` y en [`index.html`](./index.html).
4. Haz `git push`: GitHub Pages publicará automáticamente la URL `https://<usuario>.github.io/privacy-policies/<proyecto>/` lista para pegar en **Google Play Console**.

---

## 📬 Contacto del Desarrollador / Responsable

- **Desarrollador**: Ayrton Neves Estrada
- **Correo de soporte y privacidad**: [ayrton.24.6.95@gmail.com](mailto:ayrton.24.6.95@gmail.com)
