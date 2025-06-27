
# ⚖️ Asistente Legal Automatizado con IA para Emitir Dictamen Jurídico

Presentación del problema: 

La elaboración de dictámenes jurídicos en organismos públicos suele ser una tarea repetitiva, altamente técnica y consumidora de tiempo. Muchos dictámenes responden a situaciones similares, con marcos normativos estables, lo que vuelve ineficiente la redacción manual desde cero en cada caso. Automatizar esta tarea permitiría liberar recursos profesionales, acelerar procesos administrativos y aumentar la coherencia técnica en los textos producidos. 

Desarrollo de la propuesta de solución: 

La propuesta consiste en diseñar una prueba de concepto (POC) en una Jupyter Notebook que aplique técnicas de Fast Prompting para generar automáticamente dictámenes jurídicos preliminares. Se utilizará la API de OpenAI con prompts optimizados, que incluyan roles definidos, estructura paso a paso y contexto legal relevante. Los resultados serán comparados contra un enfoque tradicional de prompting para demostrar las mejoras en claridad, precisión y estilo jurídico. 

Justificación de la viabilidad del proyecto: 

El proyecto es técnicamente viable porque se basa en herramientas accesibles y ampliamente utilizadas como Python, Jupyter Notebook y la API de OpenAI. No requiere entrenamiento de modelos ni uso de bases de datos confidenciales, y se enfoca en situaciones tipo, legalmente estandarizadas. Además, el enfoque de Fast Prompting permite aprovechar al máximo las capacidades del modelo sin incurrir en múltiples llamadas innecesarias, optimizando también los costos de uso de la API. 

Objetivos 

- Implementar una solución automatizada para generar dictámenes jurídicos preliminares. 
- Aplicar técnicas de Fast Prompting para optimizar la calidad del texto legal generado. 
- Evaluar comparativamente la eficacia del enfoque tradicional vs. Fast Prompting. 
- Demostrar la factibilidad del proyecto para escalar a otros tipos de documentos legales. 

Metodología 

1. Análisis de un caso administrativo tipo donde se solicita el otorgar un legitimo abono a un proveedor para abonar una factura de un ejercicio anterior al vigente. 
2. Generación de un dictamen con un prompt tradicional para establecer una línea base. 
3. Redacción de un prompt optimizado utilizando Fast Prompting (instrucciones detalladas, rol, estructura). 
4. Ejecución de ambos prompts en ChatGPT vía Jupyter Notebook. 
5. Comparación cualitativa de los resultados. 
6. Reflexión sobre mejoras observadas y posibles ajustes futuros. 

Herramientas y tecnologías 

- Python 3.10 
- Jupyter Notebook 
- OpenAI API (modelo GPT-3.5) 
- Librerías: openai, dotenv 
- Fast Prompting (técnica de ingeniería de prompts con contexto estructurado y guía de roles) 
- NightCafe o DALL·E (opcional, para visualización de esquemas complementarios) 

Implementación 

Se desarrollaron dos prompts: 
 
1. Prompt tradicional: 
   "Redactá un dictamen jurídico sobre un legítimo abono a un proveedor para abonar una factura de un ejercicio anterior al vigente." 
 
2. Prompt con Fast Prompting: 

   Rol: Sos abogado de la Subsecretaría Legal y Técnica del Municipio de Vicente López, Provincia de Buenos Aires, especializado en derecho administrativo. Entra a consulta un expediente sobre la viabilidad de otorgar un legítimo abono a un proveedor que se le debe abonar una factura. Analiza si corresponde o no, en base a la siguiente instrucción:  
   Instrucción: 
    
    Antecedentes a verificar en el expediente:  

Contar con orden de compra 

Factura firmada por el secretario del área ejecutora 

Informe del área ejecutora 

Informe de la Dirección General de Contaduría que indique el ejercicio que hubiera correspondido  

   Normativa aplicable: Ley Orgánica de las Municipalidades de la Provincia de Buenos Aires y Artículo 140 del Reglamento de Contabilidad y Disposiciones de Administración. 

Respuestas:  

- Positiva: Es de un ejercicio anterior al vigente y no fue abonada en tiempo y forma, corresponde el legítimo abono por cumplir con las disposiciones del artículo 140 del Reglamento de Contabilidad y Disposiciones de Administración, sugiriendo sean remitidos al Honorable Conejo Deliberante a fin de sancionar la ordenanza pertinente.  

-Negativa: Es del ejercicio vigente y no fue abonada, no corresponde el legítimo abono.  

   Objetivo: Emitir un dictamen breve, claro y fundado jurídicamente. 

## 🖼️ Visual institucional 

Este proyecto incluye una imagen generada con la API de Google Gemini como cierre institucional del servicio automatizado.

![Gracias por usar este servicio](gracias_servicio.png)
