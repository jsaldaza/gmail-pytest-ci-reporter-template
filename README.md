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
├── .github/workflows/
│   └── python-tests-email.yml       # CI/CD completo con Pytest + correo Gmail
├── src/
│   ├── send_test_email.py           # Script de envío con resumen HTML
│   └── tests/
│       └── test_dummy.py            # Test de ejemplo
├── reports/                         # Aquí se guarda el reporte HTML generado
├── assets/
│   └── email-preview.png            # Imagen ejemplo del correo enviado
├── .gitignore
├── pytest.ini                       # Configuración base de Pytest
├── requirements.txt
├── requirements-dev.txt
└── README.md
```

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

## 🧪 ¿Cómo convertir esta plantilla en un proyecto real?

> Esta plantilla es solo el punto de partida. Puedes usarla como base para automatizar cualquier proyecto con tests.

### 🧩 Opción 1: Tienes un nuevo proyecto desde cero
1. Haz `Use this template`
2. Escribe tus tests reales dentro de `src/tests/`
3. Ejecuta tus pruebas normalmente. Los correos se enviarán automáticamente

### 🔁 Opción 2: Tienes un proyecto ya existente
1. Crea un nuevo repo desde esta plantilla
2. Copia tus archivos de pruebas dentro de `src/`
3. Ajusta el `python-tests-email.yml` si es necesario (por ejemplo, para rutas personalizadas)
4. Empieza a trabajar con CI listo

✅ El flujo ya está preparado para usar Pytest, generar reportes HTML, cobertura y enviar emails automáticamente sin tener que configurar desde cero cada vez.

---

## 📬 Resultado del Correo

Ejemplo real generado por esta plantilla:

![Reporte Preview](./assets/email-preview.png)

---

## 📌 Tips para extender esta plantilla

- Integra **Slack o Discord** con Webhooks si quieres alertas en canales
- Personaliza el diseño del correo HTML para que se ajuste a tu equipo o branding
- Cambia el workflow para que también envíe correos solo en `failures`, si así lo prefieres
- Publica esta plantilla en [Dev.to](https://dev.to), [Hashnode](https://hashnode.com) o [LinkedIn](https://linkedin.com)

---

## 🧰 Comandos útiles para trabajar localmente

```bash
# Ejecutar tests manualmente
pytest

# Ejecutar con reporte HTML local
pytest --html=reports/report.html --self-contained-html -v

# Validar formato o correr pre-commit (si usas)
pre-commit run --all-files
```

---

## 👨‍💻 Autor
**Juan Andrés Saldarriaga Z.**  
_Software QA Engineer | Automatizador PRO | Sharing knowledge through templates_

---
