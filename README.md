# 📊 Telecom X: Análisis de Evasión de Clientes (Churn)

## 🎯 Objetivo del Proyecto
Este proyecto tiene como finalidad analizar el comportamiento de los clientes de la empresa **Telecom X** para identificar los factores críticos que influyen en la evasión (*churn*).  
A través de un **análisis exploratorio de datos (EDA)** y el **procesamiento de datos complejos**, buscamos proporcionar *insights* accionables que permitan al equipo de **marketing y fidelización** reducir la tasa de abandono.

## 📁 Estructura de los Datos
Los datos fueron obtenidos de la **API de Telecom X** en formato **JSON**.  
El dataset original presentaba una estructura anidada que requirió un proceso de **normalización** para extraer información sobre:

- **Datos demográficos**
  - Género  
  - Ciudadanos senior  
  - Socios  
  - Dependientes  

- **Servicios**
  - Telefonía  
  - Múltiples líneas  
  - Internet (DSL, Fibra óptica)  
  - Seguridad online  
  - Soporte técnico  
  - Otros servicios relacionados  

- **Cuenta**
  - Tipo de contrato  
  - Método de pago  
  - Cargos mensuales  
  - Cargos totales  

## 🛠️ Procesamiento y Limpieza
El análisis se realizó en un **Jupyter Notebook**, siguiendo los siguientes pasos clave:

- **Desanidado de JSON**  
  Conversión de diccionarios complejos en columnas tabulares.

- **Tratamiento de Tipos**  
  Conversión de variables de texto a numéricas, especialmente en `TotalCharges`.

- **Ingeniería de Características**  
  Creación de la métrica `Cuentas_Diarias` para analizar el gasto prorrateado.

- **Limpieza de Datos**  
  Filtrado de valores inconsistentes en la variable objetivo `Churn`.
