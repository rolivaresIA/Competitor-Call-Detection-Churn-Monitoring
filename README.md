# Competitor Call Detection & Churn Monitoring

Pipeline end-to-end en BigQuery para el monitoreo de llamadas entrantes provenientes de la competencia, análisis de comportamiento de clientes post-contacto y medición de riesgo de portabilidad (churn) en un horizonte de 5 días.

Este proyecto fue desarrollado como parte de procesos de analítica en el área de Churn & Retention, con foco en entregar insights diarios a equipos de gerencia y VP del mercado Personas.

## 📋 Business Context

En la industria de telecomunicaciones, la competencia utiliza estrategias de contacto directo a clientes mediante llamadas telefónicas con el objetivo de inducir portabilidad (churn).

Dentro del área de Churn & Retention de Claro Chile, existía la necesidad de monitorear diariamente este comportamiento, identificando cuándo un cliente era contactado por números asociados a competidores y evaluando el impacto de dichos contactos en la probabilidad de portabilidad en los días posteriores.

Antes de este desarrollo, no existía un sistema automatizado que permitiera:

- Identificar llamadas entrantes provenientes de operadores competidores
- Relacionar estas interacciones con la cartera de clientes vigente
- Medir el impacto de estas llamadas en la portabilidad dentro de una ventana de 5 días

## 🎯 Objective of the Project

El objetivo de este proyecto es diseñar y automatizar un pipeline de datos en BigQuery que permita identificar, procesar y analizar llamadas entrantes provenientes de operadores competidores, vinculándolas con la cartera de clientes de la compañía.

A partir de esta integración de datos, el sistema permite:

- Detectar clientes contactados por la competencia de forma diaria
- Enriquecer la información de llamadas con datos de cartera (RUT, segmento, estado del cliente)
- Medir el comportamiento de portabilidad dentro de una ventana de 5 días posteriores al contacto
- Analizar el impacto temporal de estas llamadas en la probabilidad de portabilidad
- Segmentar los resultados por duración de llamada y operador de origen
- Generar reportes diarios automatizados para equipos de gestión y alta dirección
