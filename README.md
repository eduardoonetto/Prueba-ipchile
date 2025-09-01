# Proyecto FastAPI

Este proyecto sirve como base para construir **APIs RESTful robustas y escalables** usando FastAPI.

---

## **Requisitos**

- Python 3.10+  
- pip actualizado

---

## **Instalación**

1. Crear y activar un entorno virtual (recomendado):

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

pip install -r requirements.txt
```
app/
├─ main.py           # Entry point
├─ routers/
│  ├─ users.py
│  └─ items.py
├─ models/
│  ├─ user.py
│  └─ item.py
├─ services/
│  └─ user_service.py
├─ dependencies/
│  └─ auth.py
└─ core/
   ├─ config.py
   └─ security.py
```

uvicorn app.main:app --reload



Buenas prácticas

Separar routers por funcionalidad.

Usar servicios para lógica de negocio.

Validar datos con Pydantic.

Usar async/await para endpoints que consumen I/O intensivo.

Manejar errores y excepciones globalmente.

Implementar tests unitarios y de integración.

Mantener configuración sensible en variables de entorno.
