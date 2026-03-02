# 📘 GUÍA DE APRENDIZAJE  
# Administración y Control de Versiones con GitHub

---

## 📌 Información General

**Curso:** Ingeniería de Software II  
**Unidad:** Administración de la Configuración  
**Tema:** Control de versiones aplicado a documentación  

---

## 🎯 Resultado de Aprendizaje

Al finalizar esta sesión el estudiante será capaz de:

- Aplicar control de versiones en documentación.
- Trabajar con ramas y Pull Requests.
- Escribir commits con trazabilidad.
- Documentar requerimientos usando Markdown.
- Gestionar cambios de forma colaborativa.

---

# 1. Fundamentación Teórica

## ¿Qué es control de versiones?

Es el mecanismo que permite:

- Registrar cambios.
- Saber quién hizo cada modificación.
- Recuperar versiones anteriores.
- Trabajar en equipo sin sobrescribir cambios.

En ingeniería de software, la documentación es un elemento de configuración y debe versionarse.

---

## ¿Qué es Git?

Sistema de control de versiones distribuido que:

- Guarda historial.
- Permite trabajo paralelo mediante ramas.
- Facilita integración controlada.

---

## ¿Qué es GitHub?

Plataforma que:

- Aloja repositorios Git.
- Permite colaboración.
- Gestiona Issues, ramas y revisiones.
- Mantiene trazabilidad.

---

# 2. Markdown Básico

## Títulos

```markdown
# Título principal
## Subtítulo
### Sección
```

## Listas

```markdown
- Elemento 1
- Elemento 2
```

## Checklist

```markdown
- [ ] Pendiente
- [x] Completado
```

## Tablas

```markdown
| HU | Descripción | Prioridad |
|----|------------|----------|
| HU-01 | Registro | Alta |
```

# Tabla de Contenido y Redireccionamiento en Markdown

Para que la Tabla de Contenido funcione correctamente en GitHub, debes enlazar cada sección usando enlaces internos.

## ¿Cómo funciona?

GitHub convierte automáticamente los encabezados en enlaces internos.

Ejemplo:

Si tienes este título en tu documento:

```markdown
## 1. Introduccion
```

El enlace interno será:

```
#1-introduccion
```

---

## Cómo crear la Tabla de Contenido

Al inicio del documento, escribe:

```markdown
## 📑 Tabla de Contenido

1. [Introduccion](#1-introduccion)
2. [Descripcion General](#2-descripcion-general)
3. [Requerimientos Funcionales](#3-requerimientos-funcionales)
4. [Requerimientos No Funcionales](#4-requerimientos-no-funcionales)
5. [Trazabilidad](#5-trazabilidad)
```

Luego asegúrate de que las secciones existan exactamente así:

```markdown
## 1. Introduccion
## 2. Descripcion General
## 3. Requerimientos Funcionales
## 4. Requerimientos No Funcionales
## 5. Trazabilidad
```

---

## Reglas Importantes

- No usar tildes en los títulos.
- Usar exactamente el mismo texto en el enlace.
- Los espacios se convierten en guiones.
- Todo va en minúscula.
- Probar que los enlaces funcionen antes de hacer Pull Request.

Si el enlace no funciona, revisa que el texto del título y el enlace coincidan exactamente.

---

# 3. Buenas Prácticas de Trabajo

## 🔹 No trabajar en main

Siempre crear una rama con nombre descriptivo, por ejemplo:

```
docs/hu-01-registro
```

---

## 🔹 Convención de Commits

Formato recomendado:

```
tipo(area): mensaje claro en imperativo
```

Tipos permitidos:

- docs
- fix
- style
- chore

### Ejemplos correctos

```
docs(hu): agrega HU-01 registro de usuario
docs(criterios): añade criterios HU-02
style(srs): mejora estructura de encabezados
```

No se aceptan commits como:

- cambios
- update
- listo

---

## 🔹 Pull Request

Todo cambio debe:

1. Crear rama.
2. Hacer commits claros.
3. Abrir Pull Request.
4. Ser revisado antes de hacer merge a main.

---

# 5. Reflexión Final

Responder en grupo:

1. ¿Qué ventajas tiene usar ramas?
2. ¿Qué aporta un buen commit?
3. ¿Qué pasaría si todos trabajaran en main?
4. ¿Por qué la documentación debe versionarse?

---

## Cierre

El control de versiones no es solo una herramienta técnica.  
Es una práctica de calidad que garantiza trazabilidad, orden y gestión adecuada de la configuración del software.

Prueba
