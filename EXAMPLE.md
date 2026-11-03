# A real example, step by step / Un ejemplo real, paso a paso

> **Anonymity note.** This is a real case, from real daily use in October 2026. The names of the people, companies, and institutions involved have been withheld to protect their privacy; amounts and times are real, names are not given.
>
> **Nota de anonimato.** Este es un caso real, de uso diario real en octubre de 2026. Los nombres de las personas, empresas e instituciones involucradas se reservan para proteger su privacidad; los montos y las horas son reales, los nombres no se dan.

## The setting / El escenario

- One user, one AI assistant with persistent memory, working in Spanish, mostly by voice notes.
- The final chat model in use: the **main chat** (quick things + a 9:00 AM daily summary, kept light), **one general tasks chat** (short tasks), and **one chat per project** (each project in its own chat; a task that grows inside the tasks chat is promoted to its own chat with a written handover).
- A shared memory, a short-task list, and a vault of parked topics — all in files.

*Un usuario, un asistente de IA con memoria persistente, trabajando en español, casi todo por notas de voz. El modelo final de chats en uso: el **principal** (cosas rápidas + resumen diario de las 9:00 AM, liviano), **un chat general de tareas** (tareas cortas), y **un chat por proyecto** (cada proyecto en su propio chat; una tarea que crece dentro del chat de tareas se promueve a su propio chat con traspaso escrito). Una memoria compartida, una lista de tareas cortas y una bóveda de temas en pausa — todo en archivos.*

## What happened / Qué pasó

### 1. A payment falls through the cracks of a busy day / Un pago casi se pierde en un día ocupado

During the day, the user's calendar held a small installment payment: **US $34**, the third of four installments on a purchase from a retail chain, due in the 9:00–10:00 AM window. That same morning the user had an appointment at a government office — he was getting his driver's license — right in the middle of that window.

By night, the assistant checked: everything else from that day had been confirmed closed by the user, but the payment had never been mentioned. Instead of re-reminding him over and over, the assistant asked **once**, in a short message:

> "Did you manage to make today's payment (US $34)? Its 9:00–10:00 window overlapped with your license appointment."

The user answered with one tap: **"No, still pending."** The pending item stayed written in memory — not tied to that chat — ready to be picked up from any chat, on any day, without anyone repeating the story.

*Durante el día, el calendario del usuario tenía un pago pequeño en cuotas: **US $34**, la tercera de cuatro cuotas de una compra en una cadena de tiendas, con ventana de 9:00 a 10:00 AM. Esa misma mañana el usuario tenía una cita en una oficina de gobierno — estaba sacando su licencia de conducir — justo en medio de esa ventana. En la noche, el asistente revisó: todo lo demás del día el usuario ya lo había confirmado cerrado, pero el pago nunca se mencionó. En vez de recordárselo una y otra vez, el asistente preguntó **una sola vez**, en un mensaje corto: "¿Alcanzaste a hacer el pago de hoy (US $34)? La ventana de 9 a 10 se te solapó con la cita de la licencia." El usuario respondió con un toque: **"No, queda pendiente."** El pendiente quedó escrito en la memoria — no atado a ese chat — listo para retomarse desde cualquier chat, cualquier día, sin que nadie repita la historia.*

### 2. An appointment that existed only in a text message / Una cita que solo existía en un mensaje de texto

The same afternoon, a text message had confirmed a **telehealth appointment for Monday at 4:00 PM** with a health-services provider — including a link to upload documents before the visit. The appointment was **not on the user's calendar**. That mattered for a concrete reason: the assistant's Monday 9:00 AM summary reads **only the calendar**, so the appointment would never be reminded — and could easily be missed.

That evening the assistant sent one short message: it said what it had found, why it mattered (the broken reminder chain), and offered the fix, attaching the document-upload link. The user answered with one tap: **"Yes, put it on the calendar."**

The assistant verified there was no duplicate, created the event (Monday, 4:00–5:00 PM, with the upload link and the reschedule phone number inside), verified the event existed, and cancelled a Monday-morning follow-up it had prepared — because with the event on the calendar, the follow-up was no longer needed.

*Esa misma tarde, un mensaje de texto había confirmado una **teleconsulta para el lunes a las 4:00 PM** con un proveedor de servicios de salud — incluido un enlace para subir documentos antes de la cita. La cita **no estaba en el calendario del usuario**. Eso importaba por una razón concreta: el resumen del lunes a las 9:00 AM del asistente lee **solo el calendario**, así que la cita nunca sería recordada — y podía perderse fácilmente. En la noche, el asistente envió un mensaje corto: dijo qué había encontrado, por qué importaba (la cadena de recordatorio rota), y ofreció la solución, adjuntando el enlace de documentos. El usuario respondió con un toque: **"Sí, ponla en el calendario."** El asistente verificó que no hubiera duplicado, creó el evento (lunes, 4:00–5:00 PM, con el enlace de subida y el teléfono de reprogramación adentro), verificó que el evento existía, y canceló un seguimiento del lunes en la mañana que había preparado — porque con el evento en el calendario, el seguimiento ya no hacía falta.*

## What this example shows / Qué muestra este ejemplo

1. **Pending items live in memory, not in a chat.** Either item could be confirmed, closed, or picked up from any chat — the main one, the tasks chat, or a project chat — because the state was written to shared memory the moment it was known.
2. **The assistant asks once, with the reason attached.** One question, one tap to answer, no repeated nagging.
3. **Preparation is silent; action needs a "yes".** The follow-up message and the calendar fix were prepared in advance, but nothing was written to the user's calendar until he approved it.
4. **Finished machinery gets switched off.** The prepared follow-up was cancelled the moment its reason disappeared.
5. **Short things stay light.** Both items were handled from the main chat in minutes, with no new chat opened — exactly as the final model intends: a new chat is for a project, or for a task that has grown, not for every small thing.

*1. **Los pendientes viven en la memoria, no en un chat.** Cualquiera de los dos asuntos se podía confirmar, cerrar o retomar desde cualquier chat — el principal, el de tareas o uno de proyecto — porque el estado quedó escrito en la memoria compartida en el momento en que se supo. 2. **El asistente pregunta una vez, con la razón adjunta.** Una pregunta, un toque para responder, nada de insistencia repetida. 3. **La preparación es silenciosa; la acción necesita un "sí".** El mensaje de seguimiento y el arreglo del calendario se prepararon por adelantado, pero nada se escribió en el calendario del usuario hasta que él lo aprobó. 4. **La maquinaria terminada se apaga.** El seguimiento preparado se canceló en el momento en que su razón desapareció. 5. **Lo corto se mantiene liviano.** Ambos asuntos se resolvieron desde el chat principal en minutos, sin abrir ningún chat nuevo — tal como busca el modelo final: un chat nuevo es para un proyecto, o para una tarea que creció, no para cada cosa pequeña.*
