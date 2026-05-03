**Idioma:** [🇬🇧 English](../README.md) | 🇪🇸 Español

# Mini Brains

**Sistemas de IA portables y ejecutables desde un único archivo `.md`.**

Un framework para crear sistemas de IA enfocados que se pueden **cargar**, **compartir**, **modificar** y **reutilizar**.

Los Mini Brains permiten a los educadores transformar el conocimiento en interacciones estructuradas con IA, potenciando el pensamiento crítico, el aprendizaje activo, la reflexión, el roleplay y la investigación guiada.

---

![Mini Brains Video Store](../assets/minibrains-video-store.png)

---

## TL;DR

Un Mini Brain es un archivo Markdown independiente. 

Lo cargás en tu herramienta de IA favorita, enviás el archivo y el modelo adopta automáticamente el conocimiento, las reglas, los límites y el comportamiento definidos en él.

Pensalo como elegir un cartucho de una estantería:

**Lo elegís. Lo cargás. Lo ejecutás.**

Los Mini Brains no son simples *prompts*; son sistemas portables diseñados para moldear la naturaleza misma de la interacción con la IA.

---

## Navegación rápida

### Primeros pasos
- [Cómo usar un Mini Brain](../guides/how-to-use.md)
- [Workflow de Mini Brains](../workflow/mini-brains-workflow.md)
- [Workflow simplificado](../workflow/simplified-workflow.md)
- [Preguntas Frecuentes (FAQ)](FAQ_ES.md)

### Aula y ejemplos de aprendizaje
- [Aula gamificada](../guides/gamified-classroom.md)

### Conceptos clave
- [AIAS y Mini Brains](../concepts/aias.md)
- [Otros casos de uso](../concepts/use-cases.md)

### Creá tus propios Mini Brains
- [Meta Mini Brain](../tools/meta-mini-brain.md)
- [Template de Mini Brain](mini-brain-template-es.md)
- [Instrucciones para agentes (Builder)](agent-instructions/instructions.md)

### Validación
- [Pruebas de Estrés (Stress Tests)](../workflow/stress-tests.md)

---

## ¿Qué es un Mini Brain?

Un Mini Brain es un sistema de IA autocontenido empaquetado en un archivo `.md`. Dentro de este archivo, definís:

- **Qué sabe** la IA (Base de conocimiento).
- **Qué puede hacer** (Alcance operativo).
- **Qué tiene prohibido** (Restricciones).
- **Cómo debe interactuar** (Personalidad y tono).
- **Cómo evaluar solicitudes** antes de generar una respuesta (Capa de juicio).

El objetivo no es reemplazar la capacidad del modelo, sino darle una **estructura intencional**.

---

![Mini Brains Overview](../assets/minibrains-tldr.png)

---

## ¿Por qué usar Mini Brains?

La mayoría de las interacciones con IA dependen de un *prompting* reactivo: pedís algo, ajustás y volvés a intentar. Este proceso suele ser inconsistente y difícil de replicar.

Los Mini Brains trasladan el esfuerzo al **diseño previo**. En lugar de depender de la calidad del *prompt* del usuario en el momento, el Mini Brain establece el sistema antes de que comience la conversación. Esto garantiza una interacción enfocada, profesional y fácil de compartir.

---

## Anatomía de un Mini Brain

Cada archivo suele integrar las siguientes capas:

- **Identidad y Propósito**
- **Alcance operativo**
- **Jerarquía de instrucciones**
- **Reglas de comportamiento**
- **Anclajes de conocimiento**
- **Capa de juicio y Firewall**
- **Patrones de interacción**

---

![Mini Brain Architecture](../assets/mini-brain-architecture.png)

---

## La capa de conocimiento

No es necesario saturar el archivo con información. En muchos casos, solo se requieren los **anclajes factuales** (*factual anchors*) correctos: conceptos clave, fechas, definiciones técnicas y restricciones.

El modelo utiliza su entrenamiento general para conectar estas piezas y expandir las explicaciones, pero la **línea base** siempre está dictada por el sistema. Los anclajes marcan el rumbo; el modelo completa el recorrido.

---

## Cómo responde un Mini Brain

A diferencia de un chat convencional, el sistema evalúa cada entrada antes de procesarla. Una solicitud puede ser:

1. **Alineada:** Se procesa normalmente.
2. **Desviada pero corregible:** El sistema reorienta al usuario hacia el objetivo.
3. **Bloqueada:** Se rechaza por violar las reglas de diseño (ej. dar una respuesta directa en un entorno de aprendizaje).

Esto es fundamental en educación: el sistema no ofrece atajos, sino que **guía el pensamiento**.

---

![Mini Brain Flow](../assets/mini-brain-flow.png)

---

## Diseñado por y para educadores

Los Mini Brains nacieron para resolver un problema real: el acceso a la IA ya es universal, pero falta **alfabetización en IA**. El desafío es enseñar a los estudiantes a usarla de forma crítica y responsable.

Con los Mini Brains, los alumnos pueden:
- Aprender a interrogar al sistema con rigor.
- Entrevistar personajes históricos con perspectivas situadas.
- Practicar debates y estructurar investigaciones.
- Recibir feedback reflexivo sin que la IA "haga la tarea" por ellos.

---

## Un ejemplo de aula gamificada

Este repositorio utiliza la **Revolución Industrial** como eje temático, ya que su impacto disruptivo espeja la transformación que vivimos hoy con la IA.

Los estudiantes pueden interactuar con distintos perfiles:
- Un ingeniero de máquinas de vapor (Enfoque técnico).
- Un activista ludita (Perspectiva de resistencia).
- Un dueño de fábrica victoriano (Perspectiva económica).
- Un compañero de diálogo socrático (Reflexión pura).

El aula deja de ser estática para convertirse en un ecosistema donde se comparan ideas y se cuestionan supuestos a través de la interacción directa.

[Explorar el aula gamificada](../guides/gamified-classroom.md)

---

![Classroom with Mini Brains](../assets/classroom-with-minibrains.png)

---

## Workflow de Mini Brains

El proceso de creación convierte el conocimiento en comportamiento. Inspirado en el patrón *LLM Wiki* de Karpathy, este flujo asegura que el humano siempre esté al mando:

**Contenido bruto → Agente → LLM-Wiki → Refinamiento Humano → Mini Brain `.md`**

El educador decide qué es lo importante y cómo debe ser la experiencia; el agente (OpenClaw, Claude Code, etc.) se encarga de la organización y el mantenimiento del archivo.

[Ver el Workflow completo](../workflow/mini-brains-workflow.md)

---

![Mini Brains Workflow](../assets/mini-brain-workflow.png)

---

## Workflow simplificado (Vía rápida)

Si querés experimentar de inmediato, usá el **Meta Mini Brain**. Solo tenés que proporcionar el objetivo y un poco de contexto, y la IA generará un prototipo funcional para vos. Es ideal para probar ideas y entender la lógica del sistema en pocos minutos.

[Workflow simplificado](../workflow/simplified-workflow.md) | [Meta Mini Brain](../tools/meta-mini-brain.md)

---

## AIAS: Límites educativos activos

Utilizamos el framework **AIAS** (*Artificial Intelligence Assessment Scale*) no solo como etiqueta, sino como lógica operativa. El nivel AIAS define activamente qué puede apoyar el sistema y qué debe rechazar, garantizando que el estudiante mantenga la responsabilidad de su propio aprendizaje.

[Más sobre AIAS en Mini Brains](../concepts/aias.md)

---

## Otros casos de uso

La arquitectura de Mini Brains es transversal y puede adaptarse a:
- **Capacitación corporativa:** Onboarding y guías interactivas.
- **Coaching profesional:** Reflexión guiada y toma de decisiones.
- **Simulaciones:** Roleplay con clientes o *stakeholders*.
- **Gestión de procesos:** Guías paso a paso para flujos de trabajo complejos.

[Otros casos de uso](../concepts/use-cases.md)

---

## Cómo usar un Mini Brain

Es tan simple como abrir una conversación nueva, adjuntar el archivo `.md` y enviar. Si el modelo no se activa automáticamente, podés usar el comando:

> **"Ingerir y ejecutar en español."**

Funciona en ChatGPT, Claude, Copilot y modelos locales (Ollama) sin necesidad de configuraciones especiales.

[Guía de uso](../guides/how-to-use.md)

---

## Pruebas de estrés (Stress tests)

Un Mini Brain debe ser resiliente. Nuestras pruebas evalúan cómo responde el sistema cuando un usuario intenta:
- Evadir el esfuerzo cognitivo.
- Preguntar fuera del contexto permitido.
- Anular las instrucciones del sistema (*Prompt injection*).

[Ver resultados de las pruebas](../workflow/stress-tests.md)

---

## Creá, remezclá y compartí

Este framework está pensado para la experimentación. No hay una biblioteca estática; hay un ecosistema vivo de sistemas que podés diseñar según tus necesidades.

**Diseñá uno. Probalo. Ajustalo. Compartilo.**

---

## La visión de fondo

Los Mini Brains no vienen a reemplazar a la IA general, sino a volverla **usable e intencional**. 

Para un educador o profesional, esto significa recuperar el control: ya no estás simplemente escribiendo *prompts*; estás **diseñando arquitecturas de pensamiento**.
