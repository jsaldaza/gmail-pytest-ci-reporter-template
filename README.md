# Gmail Pytest CI Reporter Template 📬🧪

> ✨ **Bienvenido a tu plantilla PRO de automatización QA**  
> Esta plantilla lista para clonar te permite ejecutar pruebas en GitHub Actions y recibir un reporte automático por correo Gmail con resumen, cobertura y enlace al pipeline.  
>
> 🚀 Solo necesitas configurar 3 secrets (`GMAIL_USER`, `GMAIL_PASSWORD`, `TO_EMAIL`)  
> y estarás recibiendo correos tan profesionales como si los enviara tu equipo de DevOps.  
>
> ✔️ Reutilizable • 🔐 Seguro • 📬 Visual • 🧪 Pytest-ready

---

## 🚀 Quick Start

1. Haz clic en **Use this template** en GitHub
2. Configura estos Secrets:
   - `GMAIL_USER` – tu correo Gmail
   - `GMAIL_PASSWORD` – contraseña de aplicación de Gmail
   - `TO_EMAIL` – destino del correo con el reporte
3. Haz un commit… ¡y observa tu bandeja de entrada! 📬

---

## 📁 Estructura del Proyecto

```
gmail-pytest-ci-reporter-template/
├── .github/workflows/            # GitHub Actions CI workflow
│   └── python-tests-email.yml    # Flujo de test + notificación
├── src/
│   ├── tests/                    # Tests con Pytest (incluye test dummy)
│   └── send_test_email.py        # Script que genera y envía el correo
├── reports/                      # Reportes generados por pytest
├── assets/                       # Imagen de preview del correo (opcional)
├── .gitignore
├── pytest.ini                    # Configuraciones de Pytest
├── requirements.txt
├── requirements-dev.txt
└── README.md                     # Este archivo
```

---

## 🧪 Qué hace esta plantilla

- Ejecuta tus tests automáticamente en cada push a `main`
- Genera un reporte HTML + cobertura de código
- Envía un correo estilizado con:
  - ✅ Resultado del test
  - 📈 Cobertura (si está disponible)
  - 📎 Reporte en HTML como archivo adjunto
  - 🔗 Enlace al pipeline de GitHub Actions

---

## 🔐 Requisitos de configuración (Secrets en GitHub)

| Secret             | Descripción                        |
|--------------------|------------------------------------|
| `GMAIL_USER`       | Correo Gmail que envía el reporte  |
| `GMAIL_PASSWORD`   | Contraseña de aplicación (SMTP)    |
| `TO_EMAIL`         | Correo de destino para notificaciones |

🎯 Se configuran desde Settings → Secrets → Actions → New repository secret.

📌 Para obtener una contraseña segura, habilita [verificación en dos pasos](https://myaccount.google.com/security) y crea una [contraseña de aplicación Gmail](https://support.google.com/accounts/answer/185833).

---

## 📬 Resultado del Correo

Ejemplo real generado por esta plantilla:

![Reporte Preview](./assets/email-preview.png)

---

## 💡 Extras incluidos

- `send_test_email.py` puede ser usado desde GitHub Actions o localmente
- Pytest con configuración de cobertura (`pytest-cov`)
- Soporte para `pytest-html` con adjuntos
- Permite ejecución local para pruebas manuales
- Visual y profesional desde el primer uso

---

## 👨‍💻 Autor
**Juan Andrés Saldarriaga Z.**  
_Software QA Engineer | Automatizador PRO | Sharing knowledge through templates_

---

> ¿Quieres integrarlo con Slack, Notion o dashboards visuales?  
> Esta plantilla es tu punto de partida para automatización real en proyectos reales.

> _“La excelencia está en los detalles.”_

---
