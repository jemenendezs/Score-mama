# 🖥️ Calculadora Score MAMÁ 🤰

Este proyecto implementa una calculadora interactiva en Python del **Score MAMÁ (Modelo de Alerta Materna Andina)**, una herramienta clínica utilizada por el **Ministerio de Salud Pública del Ecuador** para la **detección temprana de riesgo materno** en pacientes embarazadas, especialmente a partir de las 20 semanas de gestación.

## 🎯 Objetivo
Clasificar la gravedad de las pacientes obstétricas de forma objetiva, permitiendo una toma de decisiones oportuna mediante el uso de parámetros fisiológicos clave.

## ⚙️ ¿Qué hace el programa?

- Solicita al usuario ingresar 8 parámetros clínicos:
  1. Frecuencia cardíaca
  2. Presión arterial sistólica
  3. Presión arterial diastólica
  4. Frecuencia respiratoria
  5. Temperatura corporal
  6. Saturación de oxígeno (sin oxígeno suplementario)
  7. Estado de consciencia
  8. Proteinuria en orina

- Asigna a cada variable un puntaje de **0 a 3**, según los valores de referencia oficiales del MSP.
- Suma el puntaje total y clasifica el **riesgo materno**:
  - **0–1 puntos**: Riesgo **bajo**
  - **2–4 puntos**: Riesgo **intermedio**
  - **≥5 puntos**: Riesgo **alto** – alerta materna

## 🧠 Lógica clínica implementada

El código se basa en los rangos definidos por el **MSP del Ecuador**, como se observa en la tabla oficial del Score MAMÁ. 

## 📝 Licencia

Este software está liberado bajo la **Licencia MIT en español**, permitiendo su uso, modificación y distribución con libertad.

## 💻 Requisitos

- Python 3.7 o superior

## 📦 Archivos incluidos

- `score mama.py`: Código fuente del programa.
- `README.md`: Explicación del proyecto.

## 🩺 Utilidad clínica

Una herramienta útil para:
- Médicos en áreas de emergencia o gineco-obstetricia
- Estudiantes de medicina
- Personal de salud en zonas rurales

## 📚 Referencias 

- Ministerio de Salud Pública: Control Prenatal. Guía de Práctica Clínica. Primera Edición. Quito: Dirección Nacional de Normatización; 2015. Disponible en: 
https://www.salud.gob.ec/wp-content/uploads/2014/05/GPC-CPN-final-mayo-2016-DNN.pdf
