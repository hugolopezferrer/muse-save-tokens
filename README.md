🇺🇸 English | 🇪🇸 Español — this guide is bilingual: each section in English first, then Spanish. / Esta guía es bilingüe: cada sección en inglés primero y después en español.

# Muse Save Tokens

**One main chat, one tasks chat, one chat per project — one shared memory. A simple method to keep an AI assistant fast, accurate, and cheap on tokens.**
*Un chat principal, un chat de tareas, un chat por proyecto — una sola memoria compartida. Un método sencillo para mantener un asistente de IA rápido, preciso y económico en tokens.*

A step-by-step guide for anyone — technical or not. No code, no special tools: this is a method of **organization**, born from real daily use of [Muse](https://muse.ai) (Meta's personal AI agent).

> **Draft / Borrador:** This guide is a working draft until its author declares it final. / Esta guía es un borrador hasta que su autor la declare final.

---

## What is this?

A practical guide for working with an AI assistant without the conversation becoming huge, token-expensive, and hard to follow. The core idea: **separate chats by kind of work, one shared memory** — a main chat for quick things and a daily summary, one general tasks chat for short tasks, and one dedicated chat for each project, all of them sharing a single persistent memory.

*Una guía práctica para trabajar con un asistente de IA sin que la conversación se vuelva gigante, cara en tokens y difícil de seguir. La idea central: **separar los chats por tipo de trabajo, con una sola memoria compartida** — un chat principal para lo rápido y un resumen diario, un chat general de tareas para las tareas cortas, y un chat dedicado para cada proyecto, todos compartiendo una única memoria persistente.*

## The problem

If everything happens in one single chat, the history grows without limit. Every new reply "carries" everything before it: the assistant gets slower and less accurate, and token use skyrockets — even when you are only discussing one small thing.

*Si todo se conversa en un solo chat, el historial crece sin parar. Cada respuesta nueva "carga" todo lo anterior: el asistente se hace más lento y menos preciso, y el consumo de tokens se dispara — aunque solo estés hablando de una cosa pequeña.*

## What you need before you start

1. An AI assistant with **persistent memory** (one that saves what matters in files between conversations, not only inside the chat).
2. The ability to open **more than one chat** with the same assistant.
3. Nothing else. You do not need to know how to code.

*Lo que necesitas: (1) un asistente de IA con **memoria persistente** (que guarde lo importante en archivos entre conversaciones, no solo dentro del chat); (2) poder abrir **más de un chat** con el mismo asistente; (3) nada más — no necesitas saber programar.*

## Start here: the setup conversation

Don't want to figure out the setup alone? [SETUP-CONVERSATION.md](SETUP-CONVERSATION.md) shows a complete model conversation — a user and Muse configuring this method from zero, one decision at a time, exactly the way it was built in real use. Read it, or replay it with your own assistant.

*¿No quieres armar la configuración solo? [SETUP-CONVERSATION.md](SETUP-CONVERSATION.md) muestra una conversación modelo completa — un usuario y Muse configurando este método desde cero, una decisión a la vez, exactamente como se construyó en el uso real. Léela, o repítela con tu propio asistente.*

**Contents:** [What is this?](#what-is-this) · [The final model](#the-final-model-at-a-glance) · [The method](#the-method-step-by-step) · [A short real example](#a-short-real-example) · [FAQ](#faq) · [Credits](#credits) · [License](#license)

## The final model, at a glance

1. **Main chat** — quick things, loose questions, and the daily summary. Keep it light.
2. **One general tasks chat** — short tasks live here: things that finish soon and do not generate heavy history.
3. **One chat per project** — each project is born in its own chat.
4. **A task that grows gets its own chat** — if a task inside the tasks chat stretches out, it moves to its own chat with a written handover.
5. **One shared memory** — what is saved in one chat counts in all of them. When you change chats, leave a written handover and nothing is lost.
6. **Rotate heavy chats** — when a chat gets heavy (about 150,000 tokens), write a handover, open a new chat for the same topic, and **archive** the old one. Do not delete it: its name stays as an index of the history.
7. **No documented limit on the number of chats** — the limit that matters is the weight of each chat, not how many chats you have.

*El modelo final, de un vistazo:*
*1. **Chat principal** — cosas rápidas, preguntas sueltas y el resumen diario. Se mantiene liviano.*
*2. **Un chat general de tareas** — ahí viven las tareas cortas: las que se terminan pronto y no generan historia pesada.*
*3. **Un chat por proyecto** — cada proyecto nace en su propio chat.*
*4. **Una tarea que crece pasa a su propio chat** — si una tarea dentro del chat de tareas se alarga, se mueve a su propio chat con traspaso escrito.*
*5. **Una memoria compartida** — lo guardado en un chat vale en todos. Al cambiar de chat se deja traspaso escrito y nada se pierde.*
*6. **Rotar los chats pesados** — cuando un chat se pone pesado (unos 150.000 tokens), se escribe el traspaso, se abre un chat nuevo para el mismo tema y el viejo se **archiva**. No se borra: su nombre queda como índice del historial.*
*7. **Sin límite documentado de cantidad de chats** — el límite que importa es el peso de cada chat, no cuántos chats tengas.*

## The method, step by step

### Step 1 — Keep the main chat light

Use the **main chat** only for quick things, loose questions, and your daily summary. Simple rule: if something will take several steps, it does not go in the main chat.

*Usa el **chat principal** solo para cosas rápidas, preguntas sueltas y tu resumen diario. Regla simple: si algo va a tomar varios pasos, no va en el principal.*

### Step 2 — Put short tasks in the one tasks chat

Use **one general tasks chat** for short tasks — the ones you finish soon, in one sitting, without heavy material. This avoids opening a new chat for every small thing, which would be complicated and hard to follow.

*Usa **un chat general de tareas** para las tareas cortas — las que terminas pronto, en una sentada, sin material pesado. Así evitas abrir un chat nuevo por cada cosa pequeña, que sería complicado y difícil de seguir.*

### Step 3 — Give each project its own chat

Each **project** is born in its own chat, from the start. Do not mix projects, and do not mix a project into the tasks chat: mixing topics is what inflates the context.

*Cada **proyecto** nace en su propio chat, desde el inicio. No mezcles proyectos, ni metas un proyecto en el chat de tareas: mezclar temas es lo que infla el contexto.*

### Step 4 — Promote a task that grows

A task starts in the tasks chat, but sometimes it grows. **Signs of a long task:**

- It does not finish in one sitting.
- It generates heavy material (long documents, many files, long tool outputs).
- There are waits between steps (replies, approvals, appointments).
- It has its own deliverable.

When you see those signs, open its **own chat** for that task, with a **written handover**. The task then behaves like a big topic: one topic, one chat.

*Una tarea empieza en el chat de tareas, pero a veces crece. **Señales de tarea larga:** no se termina en una sentada; genera material pesado (documentos largos, muchos archivos, salidas largas de herramientas); hay esperas entre pasos (respuestas, aprobaciones, citas); tiene entregable propio. Cuando veas esas señales, abre su **propio chat** para esa tarea, con **traspaso escrito**. La tarea pasa entonces a comportarse como un tema grande: un tema, un chat.*

### Step 5 — Cap and rotate each chat

Set a **150,000-token cap per chat** as a practical rotation point. When a chat gets heavy: (a) the assistant warns **once**; (b) it writes a **handover note** with the topic's state (what was done, what was decided, what comes next); (c) a new chat opens and **the same topic** continues there, starting by reading the handover; (d) the old chat is **archived, not deleted** — its name remains as an index of the history.

There is no documented limit on the total number of chats. Rotate by weight, not by count.

*Fija un **límite práctico de 150.000 tokens por chat** como punto de rotación. Cuando un chat se pone pesado: (a) el asistente avisa **una sola vez**; (b) escribe un **traspaso** con el estado del tema (qué se hizo, qué se decidió, qué sigue); (c) se abre un chat nuevo y se continúa **el mismo tema** ahí, empezando por leer el traspaso; (d) el chat viejo se **archiva, no se borra** — su nombre queda como índice del historial. No hay límite documentado de cantidad total de chats. Se rota por peso, no por cantidad.*

### Step 6 — Save every decision in memory, not in the chat

Each chat is a separate room: what is said in one is not heard live in the other. That is why every decision and verdict is saved in the **shared memory** (the assistant's files), so it counts in every chat. If you reply in a different chat, the assistant looks in memory — or reads the other chat — and stays in context.

*Cada chat es un cuarto separado: lo que se dice en uno no se escucha en vivo en el otro. Por eso, cada decisión y cada veredicto se guarda en la **memoria compartida** (archivos del asistente), y así vale en todos los chats. Si respondes en otro chat, el asistente busca en la memoria — o lee el otro chat — y sigue en contexto.*

### Step 7 — Changing chats is not closing the topic

Moving a topic to a new chat is just moving house, not closing. A topic closes only when **you** declare it closed. Closure is the person's verdict, never the assistant's. Archiving a rotated chat is also not closing its topic.

*Mover un tema a un chat nuevo es solo mudanza, no cierre. Un tema se cierra únicamente cuando **tú** lo declaras cerrado. El cierre lo decide la persona, nunca el asistente. Archivar un chat rotado tampoco es cerrar su tema.*

### Step 8 — Park what you are not discussing in the vault

Paused topics are archived in a **vault** (a list kept in files): they leave the context and stop costing tokens. When you want one back, ask for it by name and the assistant reactivates it. Careful: in the vault a topic is listed as **pending**, even if the system internally marks it "closed" to remove it from context — "closed" there does not mean finished.

*Los temas en pausa se archivan en una **bóveda** (una lista guardada en archivos): salen del contexto y dejan de costar tokens. Cuando quieras retomar uno, pídelo por su nombre y el asistente lo reactiva. Ojo: en la bóveda un tema figura como **pendiente**, aunque internamente el sistema lo marque "cerrado" para sacarlo del contexto — "cerrado" ahí no significa terminado.*

### Step 9 — Check your usage now and then

Do not watch the meter constantly: only at natural pauses, after big blocks of work. The savings do not come from watching the number, but from **starting each chat light, with the written handover**.

*No mires el medidor a cada rato: solo en pausas naturales, después de bloques grandes de trabajo. Lo que ahorra no es vigilar el número, sino **empezar cada chat liviano, con el traspaso escrito**.*

## Handover template (copy and fill in)

```
Topic: _______________
What was done: _______________
What was decided: _______________
What comes next: _______________
Key files: _______________
```

More ready-to-copy templates (including a vault index) are in [TEMPLATES.md](TEMPLATES.md).

*Plantilla de traspaso arriba; más plantillas listas para copiar (incluido un índice de bóveda) están en [TEMPLATES.md](TEMPLATES.md).*

## A short real example

> *This is a real case, anonymized: the names of the people, companies, and institutions involved have been withheld to protect their privacy.*
> *Este es un caso real, anonimizado: los nombres de las personas, empresas e instituciones involucradas se reservan para proteger su privacidad.*

One Friday night, a pending installment payment (US $34, owed to a retail chain) was saved into the assistant's memory from the main chat, because that day it could not be paid. The pending item lived in **memory**, not in a chat — so it could be confirmed or closed later from **any** chat, with nothing repeated. That same night, a telehealth appointment for the following Monday — confirmed to the user by text message but missing from his calendar — was flagged by the assistant, and with a single "yes" it was added to the calendar, document-upload link included, in time for the Monday-morning summary to catch it.

The full walkthrough is in [EXAMPLE.md](EXAMPLE.md).

*Una noche de viernes, un pago en cuotas pendiente (US $34, a una cadena de tiendas) quedó guardado en la memoria del asistente desde el chat principal, porque ese día no se pudo pagar. El pendiente vivía en la **memoria**, no en un chat — así que después se podía confirmar o cerrar desde **cualquier** chat, sin repetir nada. Esa misma noche, una teleconsulta del lunes siguiente — confirmada al usuario por mensaje de texto pero ausente de su calendario — fue detectada por el asistente, y con un solo "sí" quedó agregada al calendario, con su enlace para subir documentos, a tiempo para que el resumen del lunes en la mañana la agarrara. El ejemplo completo está en [EXAMPLE.md](EXAMPLE.md).*

## The numbers (measured in real use, 20-Oct-2026)

- Total context window: **350,000 tokens**.
- Permanent files loaded in every conversation: **~13,000 tokens** (the main memory file, ~5,500, is the largest).
- The vault lives on disk and is **never loaded** unless a topic is requested.
- Estimate for a heavy session of ~50 turns: without the method ≈ 11.0 million input tokens; with the method ≈ 4.75 million → **savings ≈ 57%**.

*Los números (medidos en uso real, 20-oct-2026): ventana total 350.000 tokens; archivos permanentes por carga ~13.000 tokens (el de memoria, ~5.500, es el mayor); la bóveda vive en disco y nunca se carga salvo pedido. Estimación para una sesión pesada de ~50 turnos: sin método ≈ 11,0 millones de tokens de entrada; con método ≈ 4,75 millones → **ahorro ≈ 57%**.*

## FAQ

**What if I reply in the other chat?**
Nothing breaks: the assistant understands you just the same, because it searches the shared memory. It only helps if you name the topic; a bare "yes" may force it to check the threads to locate you.

*¿Y si respondo en el otro chat? No pasa nada: el asistente te entiende igual, porque busca en la memoria compartida. Solo ayuda si nombras el tema; un "sí" sin tema puede obligarlo a revisar los hilos para ubicarte.*

**Should every task get its own chat?**
No. That was considered and discarded as too complicated. Short tasks share the one general tasks chat. Only a task that grows — see the signs in Step 4 — gets its own chat.

*¿Cada tarea debería tener su propio chat? No. Eso se evaluó y se descartó por complicado. Las tareas cortas comparten el único chat general de tareas. Solo una tarea que crece — mira las señales del Paso 4 — pasa a su propio chat.*

**How many chats can I have?**
There is no documented limit on the number of chats. The practical limit is the weight of each chat (about 150,000 tokens). When a chat gets heavy, rotate it and archive the old one.

*¿Cuántos chats puedo tener? No hay límite documentado de cantidad de chats. El límite práctico es el peso de cada chat (unos 150.000 tokens). Cuando un chat se pone pesado, rótalo y archiva el viejo.*

**Does a fresh helper agent save the same?**
No: a helper launched from a heavy thread **inherits** that heavy context. What saves tokens is the new chat starting light with the written handover.

*¿Un asistente nuevo (subagente) ahorra lo mismo? No: un ayudante lanzado desde un hilo pesado **hereda** ese contexto pesado. Lo que ahorra es el chat nuevo que arranca liviano con el traspaso escrito.*

**Do I need any special tool?**
Only an assistant with persistent memory and more than one chat. The method is about organization, not software.

*¿Necesito alguna herramienta especial? Solo un asistente con memoria persistente y más de un chat. El método es de organización, no de software.*

## How this differs from other token savers

Other open-source tools save tokens at other layers: some shorten the assistant's **replies**, others compress the **conversation history** for coding agents (for example, [TOMC](https://github.com/ZipengWu365/TOMC)). This guide works at a different layer — **how a person organizes chats, memory, and topics day to day** — and it is written for non-technical users of a personal assistant. The approaches stack; they do not compete.

*Otras herramientas de código abierto ahorran tokens en otras capas: unas acortan las **respuestas** del asistente, otras comprimen el **historial** para agentes de programación (por ejemplo, [TOMC](https://github.com/ZipengWu365/TOMC)). Esta guía trabaja en otra capa — **cómo una persona organiza chats, memoria y temas en el día a día** — y está escrita para usuarios no técnicos de un asistente personal. Los enfoques se suman; no compiten.*

## Credits

- Built for [Muse](https://muse.ai), Meta's personal AI agent — the assistant this method was developed with, in real daily use.
- Compared in the last section: [TOMC](https://github.com/ZipengWu365/TOMC), an open-source token compressor for coding agents.

*Créditos: creado para [Muse](https://muse.ai), el agente personal de IA de Meta, el asistente con el que se desarrolló este método en el uso diario real. Comparado en la última sección: [TOMC](https://github.com/ZipengWu365/TOMC), un compresor de tokens de código abierto para agentes de programación.*

## License

MIT — see [LICENSE](LICENSE). You are free to use, copy, and adapt this method.

*Licencia MIT — ver [LICENSE](LICENSE). Eres libre de usar, copiar y adaptar este método.*
