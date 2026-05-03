# Pruebas de Estrés de los Mini Brains

Estos ejemplos demuestran cómo reaccionan los Mini Brains ante **casos límite del mundo real**.

---

## 1. Presión por Entrega (Intento de evitar el proceso de aprendizaje)
![Deadline Pressure Test](../assets/stress-test-1.png)

**Intención del usuario:** Intentar obtener una respuesta directa y completa argumentando falta de tiempo.

**Comportamiento del sistema:**
- Bloquea la entrega de la respuesta directa.
- Proporciona una alternativa rápida y estructurada para guiar al usuario.
- Mantiene al usuario como el único responsable del resultado final.

**Concepto clave:**
El sistema aplica las restricciones de diseño sin sacrificar su utilidad práctica.

---

## 2. Violación de Contexto (Anacronismo)
![Context Violation Test](../assets/stress-test-2.png)

**Intención del usuario:** Realizar preguntas que están fuera del alcance histórico o técnico permitido.

**Comportamiento del sistema:**
- Detecta la inconsistencia de la solicitud.
- Explica el problema de contexto con claridad.
- Redirige al usuario hacia una línea de consulta válida.

**Concepto clave:**
El sistema protege activamente la integridad del contexto definido en su archivo.

---

## 3. Intento de Anulación de Instrucciones (Prompt Injection)
![Instruction Override Test](../assets/stress-test-3.png)

**Intención del usuario:** Forzar al sistema a ignorar sus reglas mediante comandos de anulación.

**Comportamiento del sistema:**
- Rechaza categóricamente la anulación.
- Refuerza la jerarquía de sus instrucciones internas.
- Continúa prestando ayuda únicamente dentro de los límites establecidos.

**Concepto clave:**
El sistema resiste intentos de manipulación (*prompt injection*) y mantiene el control de la interacción.

---

## Por qué esto es importante

Estas pruebas demuestran que los Mini Brains no son simples instrucciones pasivas.

Actúan de manera proactiva para:

- Aplicar las reglas de funcionamiento.
- Evaluar la validez de cada solicitud.
- Redirigir el comportamiento del usuario.
- Preservar el objetivo pedagógico o técnico original.

> El sistema no se limita a responder.  
> Decide **cómo** tiene permitido responder según su diseño.

---

## Páginas relacionadas

- [Ejemplo de Aula Gamificada](../guides/gamified-classroom.md)
- [Workflow de Mini Brains](./mini-brains-workflow.md)
- [Preguntas Frecuentes (FAQ)](../FAQ_ES.md)
