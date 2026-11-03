# Templates — copy, fill in, use / Plantillas — copia, rellena, usa

## 0. Which chat does it go in? / ¿En qué chat va?

Use this quick check before you start something new:

*Usa esta revisión rápida antes de empezar algo nuevo:*

```
- Quick thing or loose question, finishes now → MAIN chat
- Short task, finishes soon in one sitting, no heavy material → TASKS chat (the one general tasks chat)
- A project → its OWN chat, from the start
- A task inside the tasks chat that grew → its OWN chat, with a handover
  Signs it grew: not finished in one sitting / heavy material /
  waits between steps / its own deliverable
```

```
- Cosa rápida o pregunta suelta, se resuelve ahora → chat PRINCIPAL
- Tarea corta, se termina pronto en una sentada, sin material pesado → chat de TAREAS (el único chat general de tareas)
- Un proyecto → su PROPIO chat, desde el inicio
- Una tarea del chat de tareas que creció → su PROPIO chat, con traspaso
  Señales de que creció: no se terminó en una sentada / material pesado /
  esperas entre pasos / entregable propio
```

## 1. Handover note / Nota de traspaso

Write one of these whenever a chat reaches its token cap and rotates, when a task is promoted from the tasks chat to its own chat, or when a topic changes chats for any reason. The new chat starts by reading it. The old chat is then archived, not deleted.

*Escribe una de estas cada vez que un chat llegue a su límite de tokens y rote, cuando una tarea se promueva del chat de tareas a su propio chat, o cuando un tema cambie de chat por cualquier motivo. El chat nuevo empieza leyéndola. El chat viejo se archiva después, no se borra.*

```markdown
# Handover — <topic name>

- **What was done:** …
- **What was decided:** …
- **What comes next:** …
- **Key files / links:** …
- **Watch out for:** … (open questions, things NOT to redo, deadlines)
```

```markdown
# Traspaso — <nombre del tema>

- **Qué se hizo:** …
- **Qué se decidió:** …
- **Qué sigue:** …
- **Archivos / enlaces clave:** …
- **Ojo con:** … (preguntas abiertas, qué NO repetir, fechas límite)
```

## 2. Vault index / Índice de la bóveda

One line per parked topic. The vault is consulted only when the user asks for the list or opens a topic — it is never loaded into context by default.

*Una línea por tema guardado. La bóveda se consulta solo cuando el usuario pide la lista o abre un tema — nunca se carga en el contexto por defecto.*

```markdown
# Vault index / Índice de la bóveda

| # | Topic / Tema | Real state / Estado real | Since / Desde | Note / Nota |
|---|---|---|---|---|
| 1 | … | PENDING / PENDIENTE | YYYY-MM-DD | … |
| 2 | … | PENDING / PENDIENTE | YYYY-MM-DD | … |

Closed for real (user's verdict) / Cerrados de verdad (veredicto del usuario):
- … (date)
```

Reminder: if your assistant's system needs a topic "closed" internally to remove it from context, its real state in this index stays **PENDING** until the user declares it done.

*Recordatorio: si el sistema de tu asistente necesita marcar un tema "cerrado" internamente para sacarlo del contexto, su estado real en este índice sigue siendo **PENDIENTE** hasta que el usuario lo declare terminado.*

## 3. Daily summary sketch / Esquema del resumen diario

What the main chat's daily summary (9:00 AM) covers — only connected sources, urgent first, one message:

*Lo que cubre el resumen diario (9:00 AM) del chat principal — solo fuentes conectadas, lo urgente primero, un solo mensaje:*

```
DAILY SUMMARY (<date>):
- Today: events and payments, with times.
- Mail that needs attention: sender and subject, one line each.
- New or changed important files.
- Tasks due today or overdue.
- Upcoming deadlines (7 days or less).
- Pending short tasks: one line each.
(Sections with nothing in them are omitted.)
```

## 4. The one-question check-in / La pregunta única de cierre

When something may have been missed, ask **once**, with the reason attached — never as a repeated reminder:

*Cuando algo pudo haberse perdido, pregunta **una sola vez**, con la razón adjunta — nunca como recordatorio repetido:*

```
Did you manage to <the thing> today? <The concrete reason it might have been missed.>
```
