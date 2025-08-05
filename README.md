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

### **Tabla de Puntuación Score MAMÁ**

| Puntaje 3 | Puntaje 2 | Puntaje 1 | **Parámetro (Puntaje 0 - Normal)** | Puntaje 1 | Puntaje 2 | Puntaje 3 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| ≤50 | | 51-59 | **FC (lpm): 60-100** | 101-110 | 111-119 | ≥120 |
| ≤70 | 71-89 | | **Sistólica (mmHg): 90-139** | | 140-159 | ≥160 |
| ≤50 | 51-59 | | **Diastólica (mmHg): 60-85** | 86-89 | 90-109 | ≥110 |
| ≤11 | | | **FR (rpm): 12-22** | | 23-29 | ≥30 |
| | ≤35.5 | | **Tº C: 35.6-37.5** | 37.6-38.4 | | ≥38.5 |
| ≤85 | 86-89 | 90-93 | **Sat O₂ (%): 94-100** | | | |
| No responde | Responde al dolor / Estuporosa | | **Estado de Conciencia: Alerta** | Responde a la voz / Somnolienta | Confusa / Agitada | |
| | | | **Proteinuria: Negativo** | Positivo | | |

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
