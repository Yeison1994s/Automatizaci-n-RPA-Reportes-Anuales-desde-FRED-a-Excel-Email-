# Automatización RPA: Web ➡ Excel ➡ Email

Este proyecto demuestra una solución de automatización RPA desarrollada con **Rocketbot** para la extracción de datos económicos desde el portal FRED, su procesamiento en **Microsoft Excel**, y la entrega final automatizada vía **correo electrónico**.

> ⚙️ Esta automatización fue diseñada por Yeison Estiven López, orientada a mejorar procesos repetitivos de recolección y análisis de datos en entornos empresariales o analíticos.



## Flujo del Proceso

### 1. Extracción Web (FRED)
- Navegación automática a la [serie CORESTICKM159SFRBATL](https://fred.stlouisfed.org/series/CORESTICKM159SFRBATL).
- Configuración de rango dinámico de fechas (ej: 1992-2025).
- Descarga automática del archivo Excel actualizado.

### 2. Procesamiento de Datos en Excel
- Apertura robusta del archivo Excel descargado, con reintentos ante fallos.
- Uso de fórmulas `SUMIFS` para calcular valores anuales por año.
- Creación de una hoja de resumen con:
  - Total anual
  - Variación interanual (en $ y %)
  - Tasa de crecimiento (positivo o negativo)
- Proyección parcial para 2025 basada en datos disponibles (ene-abr).

### 3. Envío Automatizado
- Envío del archivo `.xlsx` procesado como adjunto vía email.
- SMTP seguro (compatible con Gmail y Outlook).
- Mensaje automático personalizado para distribución de reportes.

## Tecnologías y Herramientas Utilizadas

- **Rocketbot** (plataforma RPA)
- **JavaScript** (interacción DOM para campos de fecha)
- **Python embebido** (control de apertura de Excel vía COM)
- **Excel** (formato dinámico y fórmulas integradas)
- **SMTP** (envío automático de correos electrónicos)

## Beneficios para la Empresa

1. Reducción de tiempo operativo en la recolección de datos  
2. Eliminación de errores humanos en cálculos repetitivos  
3. Automatización de reportes listos para distribuir  
4. Escalabilidad para múltiples indicadores o portales  
5. Compatible con procesos de Business Intelligence o Compliance  


## Escenarios de Aplicación

- Finanzas corporativas (seguimiento de indicadores económicos)
- Departamentos de analítica de datos
- Reportes regulatorios o de cumplimiento
- Automatización en procesos de inteligencia de negocios (BI)



## 📬 ¿Quieres saber más?

Este flujo es solo un ejemplo del tipo de soluciones RPA que se pueden desarrollar para aumentar la eficiencia operativa.  

![Diagrama del Proceso](./diagrama-proceso.png)

📧 Contacto: [https://www.linkedin.com/in/yeison-estiven-l%C3%B3pez/]



> 🚫 Nota: Por confidencialidad, el código fuente no se encuentra público. Solo se expone la arquitectura general del proceso.
>

Proyecto desarrollado por **Yeison Estiven López**
Rol: Analista RPA
Herramienta:Rocketbot
Año:2025


