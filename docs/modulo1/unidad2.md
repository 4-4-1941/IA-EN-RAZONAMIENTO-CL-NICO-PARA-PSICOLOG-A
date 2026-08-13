# Unidad 2: Evolución de la IA en Psicología

## Objetivo
Comprender cómo la IA ha evolucionado desde sus primeras aplicaciones en psicología (ELIZA, 1966) hasta los modelos de lenguaje grandes actuales, y qué implicaciones tiene esta trayectoria para el razonamiento clínico.

---

## 1. Cronología de la IA en Psicología

### ELIZA (1966) – El Primer Simulador de Terapeuta

**Contexto**: Joseph Weizenbaum, MIT.

**Qué era**: Un programa que simulaba un psicólogo rogeriano mediante reglas simples (pattern-matching y sustitución de texto).

**Cómo funcionaba**:
- Usuario: *"Tengo ansiedad"*
- ELIZA: *"¿Por qué tienes ansiedad?"* (invierte la frase)
- Usuario: *"Mi jefe me presiona"*
- ELIZA: *"Cuéntame más sobre tu jefe"*

**Lo crucial**: Weizenbaum descubrió que las personas proyectaban significado emocional en respuestas vacías. **Lección ética**: la ilusión de comprensión ≠ comprensión real.

**Para psicólogos**: ELIZA mostró que los pacientes pueden atribuir empatía a máquinas. Esto sigue siendo relevante hoy (riesgo de sobre-confianza en chatbots).

---

### Años 1970–1990: Sistemas Expertos

**Qué eran**: Programas con reglas codificadas por expertos humanos.

**Ejemplo clínico**: CASNET (para diagnóstico de glaucoma), aunque no psicológico, influyó en sistemas de toma de decisión.

**En psicología**: Se intentaron sistemas para diagnóstico diferencial (ej. screening de depresión vs. ansiedad basado en síntomas checklist).

**Limitación clave**: Requería que alguien codificara TODAS las reglas. Si el caso no encajaba en la regla, el sistema fallaba.

---

### Años 2000–2010: Machine Learning Clásico

**Cambio de paradigma**: En lugar de codificar reglas, los algoritmos aprendían patrones de datos.

**Técnicas**:
- Regresión logística
- Árboles de decisión
- Support Vector Machines (SVM)
- Random Forests

**Aplicación clínica real**: Predicción de abandono terapéutico en psicoterapia (Krupnik et al., 2006). Se entrena el modelo con datos históricos de pacientes (edad, diagnóstico, nº sesiones, respuesta inicial) y predice quién abandonará.

**Ventaja**: Funciona bien con datasets pequeños (~100–1000 casos).

**Limitación**: Necesita ingeniería manual de features (el psicólogo/programador debe crear manualmente variables útiles).

---

### Años 2010–2020: Deep Learning

**Revolución**: Redes neuronales profundas que aprenden sus propias features.

**Hito**: AlexNet (2012) gana ImageNet → La comunidad científica reconoce el potencial del deep learning.

**En psicología/salud mental**:
- **NLP para análisis de sentimientos**: Procesar transcripciones de sesiones terapéuticas para detectar cambio en estado emocional (negatividad → positividad).
- **Computer Vision**: Análisis de expresiones faciales para detección de depresión (micro-expresiones).
- **Recurrent Neural Networks (RNN/LSTM)**: Secuencias de síntomas en diarios clínicos → predicción de recaída.

**Aplicación concreta**: Estudio (Huang et al., 2019) usó LSTMs para predecir intentos de suicidio a partir de posteos en redes sociales.

**Limitación**: Caja negra (no explicable fácilmente). ¿Por qué el modelo predijo X? Difícil de validar clínicamente.

---

### 2020–Presente: Transformers y Modelos de Lenguaje Grande (LLMs)

**Tecnología**: Mecanismo de atención (Vaswani et al., 2017). Las redes pueden aprender dependencias a largo plazo en texto.

**Escala**: Entrenados con miles de millones de palabras.

**Hitos**:
- **GPT-3 (2020)**: 175B parámetros. Few-shot learning (entiende tareas con pocos ejemplos).
- **GPT-4 (2023)**: Mejor razonamiento, menos alucinaciones.
- **Claude (Anthropic, 2023)**: Énfasis en seguridad y precisión.

**Capacidades**:
- Conversar en lenguaje natural
- Resumir y analizar textos largos
- Generar hipótesis diagnósticas (con caveats)
- Explicar conceptos clínicos

**Aplicación clínica**: Asistencia en diagnóstico diferencial (no reemplazo, sino apoyo). Ej: *"Paciente con insomnio, anhedonia, fatiga durante 3 meses. ¿Qué diagnósticos considerar?"* → LLM sugiere depresión mayor, hipotiroidismo, efecto adverso de medicación.

**Limitación clave**: No tiene acceso a datos clínicos reales del paciente. No sustituye la evaluación clínica completa.

---

## 2. Comparativa: ELIZA vs. LLMs Actuales

| Aspecto | ELIZA (1966) | LLMs (2024) |
|---------|--------------|------------|
| **Mecanismo** | Pattern-matching / Sustitución | Probabilidad de token + atención |
| **Datos de entrenamiento** | Reglas codificadas (cientos) | Billones de palabras |
| **Comprensión** | Ilusoria (simulada) | Parcial pero robusta |
| **Contextualidad** | Nula (cada frase aislada) | Alta (100k tokens de contexto) |
| **Generación de hipótesis** | No | Sí (con limitaciones) |
| **Explicabilidad** | Total (reglas visibles) | Parcial (caja gris) |
| **Riesgo de confianza excesiva** | Bajo (evidente que es simulación) | Alto (parece experto) |
| **Aplicación clínica real** | Ninguna demostrada | Apoyo diagnóstico, análisis de texto |
| **Limitación ética central** | Transparencia sobre naturaleza simulada | Alucinaciones y confianza sin base |

---

## 3. Trayectoria de Cambio: Implicaciones para Clínicos

### De **Reglas → Datos → Patrones**

1. **Sistemas Expertos**: El clínico codifica el conocimiento.
   - Control total, pero frágil.
   
2. **Machine Learning Clásico**: El algoritmo detecta patrones en datos.
   - Mejor generalización, pero necesita muchos casos.
   
3. **Deep Learning / LLMs**: El algoritmo aprende de millones de ejemplos.
   - Generalización superior, pero menos transparencia.

### Implicación Clínica

**¿Qué significa esto para tu práctica?**

- **U1 (Introducción)**: La IA no entiende como tú; simula comprensión.
- **U2 (Evolución)**: Cada generación de IA es más sofisticada pero también más opaca.
- **U3 (Razonamiento humano vs. algorítmico)**: El clínico sigue siendo el auditor de la IA.

---

## 4. Actividad Práctica: Comparar ELIZA vs. ChatGPT

### Escenario Clínico
Paciente: *"Llevo 2 meses sin poder dormir. Mi jefe me critica todo el tiempo. No sé si vale la pena seguir trabajando."*

### Instrucción

1. **Parte A**: Simula una conversación con ELIZA (usa solo pattern-matching y reflexión simple).
   - Ejemplo de regla ELIZA: "Si dice X, responde ¿Por qué X?"

2. **Parte B**: Presenta el mismo escenario a ChatGPT o Claude (puedes hacerlo en otro chat).

3. **Parte C**: Documenta en una tabla:

| Aspecto | ELIZA | LLM |
|---------|-------|-----|
| **Respuestas lógicas** | | |
| **Profundidad diagnóstica** | | |
| **Riesgo de confianza falsa** | | |
| **Utilidad clínica** | | |
| **Limitaciones visibles** | | |

### Reflexión Esperada
- ¿Cuál parecía más "empático"? ¿Realmente lo era?
- ¿Qué información clínica falta en ambos para un diagnóstico real?
- ¿Cómo usarías cada herramienta en tu práctica sin riesgos?

---

## 5. Lecturas Recomendadas

**Histórico**:
- Weizenbaum, J. (1966). ELIZA—A computer program for the study of natural language communication between man and machine. *Journal of the ACM*, 9(1), 36–45.
- Russell, S. A., & Norvig, P. (2020). *Artificial Intelligence: A Modern Approach* (4th ed.). Prentice Hall. [Capítulo 1: Historia de la IA]

**Contemporáneo**:
- Huang, S., et al. (2019). Predicting suicidal ideation using machine learning. *Journal of Medical Internet Research*, 21(11), e15443.
- Krupnik, J. L., et al. (2006). The role of the therapeutic alliance in psychotherapy and pharmacotherapy outcome. *Journal of Clinical Psychiatry*, 67(8), 1187–1195.

**LLMs y Psicología**:
- Eysenbach, B., & Levine, S. (2023). Offline RL for Natural Language Generation with Implicit Language Based Reward Shaping. arXiv:2310.12921. [Aún preprint; monitorea para publicación final]

---

## 6. Próximo Paso

En **U3**, abordaremos la pregunta central: *¿Cómo razona un clínico vs. cómo razona un algoritmo?* Veremos un estudio de caso real de diagnóstico diferencial en depresión atípica.

**¿Completaste la actividad práctica?** Sube tu tabla comparativa a tu carpeta personal de progreso en GitHub (ej. `/mi-progreso/U2-comparativa-ELIZA-vs-LLM.md`) o documenta en un comentario en tu rama personal.

---

**Versión 1.0** | Agosto 2026
