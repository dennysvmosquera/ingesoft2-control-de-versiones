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

# 🧠 1. Fundamentación Teórica

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

# ✍ 2. Markdown Básico

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

---

# 🌿 3. Buenas Prácticas de Trabajo

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

# 🧩 4. Taller Práctico  
## Construcción colaborativa del SRS

---

## 🏢 Contexto del Sistema

Plataforma de reservas de espacios de coworking.

---

## 📌 Enunciados por grupo

Cada grupo debe convertir su enunciado en Historia(s) de Usuario con criterios de aceptación usando Markdown.

---

### 🟢 Grupo 1 – Registro de usuario

El sistema debe permitir crear cuenta con correo y contraseña.  
El correo no puede repetirse.  
La contraseña debe tener mínimo 8 caracteres.  
Debe mostrarse confirmación de registro exitoso.

---

### 🔵 Grupo 2 – Reserva de sala

Un usuario autenticado debe seleccionar sala, fecha y horario disponible.  
No debe permitir reservar sala ocupada.  
Debe mostrar costo antes de confirmar.

---

### 🟣 Grupo 3 – Cancelación de reserva

Debe permitir cancelar con mínimo 2 horas de anticipación.  
Si cancela después, se cobra 50%.  
Debe actualizar disponibilidad.

---

### 🟠 Grupo 4 – Calificación del espacio

Solo usuarios que reservaron pueden calificar.  
Escala de 1 a 5 estrellas.  
Comentario opcional.

---

### 🔴 Grupo 5 – Pago en línea

Debe permitir pago con tarjeta débito o crédito.  
Debe validar aprobación antes de confirmar.  
Si falla, no guardar reserva.

---

# 📝 5. Instrucciones del Taller

Cada grupo debe:

1. Crear un Issue con el nombre:
   ```
   HU-XX - Tema
   ```

2. Crear rama:
   ```
   docs/hu-XX-tema
   ```

3. Editar el archivo:
   ```
   docs/historias-usuario.md
   ```

4. Usar la plantilla:

```markdown
## HU-XX — Título

Como <rol>  
quiero <acción>  
para <beneficio>

### Criterios de aceptación
- Dado que ...
- Cuando ...
- Entonces ...
```

5. Realizar mínimo 2 commits.
6. Crear Pull Request.
7. Revisar el PR de otro grupo.

---

# 📊 6. Criterios de Evaluación

| Criterio | Valor |
|----------|--------|
| Uso correcto de ramas | 20% |
| Commits con convención | 20% |
| Historia clara y no ambigua | 20% |
| Criterios verificables | 20% |
| Uso correcto de Markdown | 20% |

---

# 🔎 7. Reflexión Final

Responder en grupo:

1. ¿Qué ventajas tiene usar ramas?
2. ¿Qué aporta un buen commit?
3. ¿Qué pasaría si todos trabajaran en main?
4. ¿Por qué la documentación debe versionarse?

---

## 🎓 Cierre

El control de versiones no es solo una herramienta técnica.  
Es una práctica de calidad que garantiza trazabilidad, orden y gestión adecuada de la configuración del software.
