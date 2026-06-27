# 🏆 Mundial 2026 GodMode - Seguimiento en Tiempo Real

[![Estado](https://img.shields.io/badge/estado-activo-brightgreen)](https://airam92.github.io/mundial-2026-Tenerife/)
[![Licencia](https://img.shields.io/badge/licencia-MIT-blue)](LICENSE)
[![Demo](https://img.shields.io/badge/demo-en%20vivo-orange)](https://airam92.github.io/mundial-2026-Tenerife/)

## 📊 Descripción

Web **100% gratuita y sin dependencias externas** para el seguimiento en tiempo real del Mundial de Fútbol 2026 (México, EE.UU., Canadá). Un solo archivo `.html` que lo hace todo: resultados en vivo, goleadores con banderas, clasificaciones por grupos, y mucho más.

**🌐 Demo en vivo:** [airam92.github.io/mundial-2026-Tenerife](https://airam92.github.io/mundial-2026-Tenerife/)

## 🚀 Características

### 🔴 Partidos en Vivo
- Actualización automática cada 60 segundos cuando hay partidos en juego
- Minuto a minuto con indicador visual de "EN VIVO"
- Resultados parciales en tiempo real

### ⚽ Goleadores con Banderas
- Lista detallada de goleadores por partido
- Banderita del equipo al lado de cada goleador 🇦🇷🇧🇷🇪🇸
- Detección automática del equipo correcto (local/visitante)
- Soporte para penaltis y autogoles

### 📅 Partidos del Día y Próximos
- Vista de todos los partidos programados para hoy
- Próximos encuentros ordenados cronológicamente
- Fechas formateadas en español con zona horaria WEST (Tenerife)

### ⏪ Partidos Pasados
- Historial completo de resultados
- Carga automática de goleadores sin intervención manual
- Sistema de caché inteligente para acceso instantáneo

### 📊 Clasificaciones por Grupos
- Tablas completas de los 12 grupos (A-L)
- PJ, G, E, P, GF, GC, DG, PTS
- Indicador visual de equipos clasificados (verde)
- Banderas de cada selección

### ⏰ Reloj en Tiempo Real
- Hora actual de Tenerife (WEST)
- Fecha completa en español
- Actualización cada segundo

## 🛠️ Sistema de Carga Inteligente

- **Carga progresiva de goleadores**: Prioriza partidos en vivo/hoy, luego carga el resto en segundo plano
- **Auto-refresh inteligente**: Solo se activa cuando hay partidos en juego
- **Indicador de primera carga**: Aviso visual del tiempo estimado de carga inicial (2-3 minutos)
- **Caché multi-capa**: Partidos, goleadores y clasificaciones almacenados localmente

## 💾 Sistema de Caché

- **Caché de partidos**: localStorage con 5 min de duración para carga instantánea
- **Caché de goleadores**: Persistente entre sesiones, no se pierde al cerrar
- **Fallback automático**: Si la API falla, usa datos en caché

## 🛡️ Robustez

- **Fetch con reintentos**: 3 intentos con timeout de 10s y espera exponencial
- **Sanitización de datos**: Protección XSS en todos los datos de la API
- **Gestión de errores**: Banners con botones de reintentar/usar caché
- **Skeleton loaders**: Animaciones de carga mientras se obtienen datos

## 🎨 Diseño

- **Tema oscuro** con detalles en naranja y dorado
- **Diseño responsive**: Adaptado a móviles, tablets y desktop
- **Google Fonts**: Orbitron (títulos) + Inter (textos)
- **Animaciones CSS**: Fuego en header, pulso en vivo, carga progresiva
- **Accesibilidad**: Roles ARIA en navegación y tarjetas de partidos

## 📋 Requisitos

- Navegador moderno con JavaScript habilitado
- Conexión a internet (solo para obtener datos de la API)
- 5-10 MB de espacio en localStorage para caché

🏗️ Tecnologías
HTML5 semántico

CSS3 con variables y animaciones

JavaScript Vanilla (sin frameworks)

API

localStorage para caché local

🎯 Mejoras desde la v1
Sistema de carga progresiva de goleadores (prioriza en vivo/hoy)

Auto-refresh inteligente (solo con partidos en juego)

Banderitas en cada goleador

Indicador de primera carga con tiempo estimado

Skeleton loaders durante la carga

Fetch con reintentos y timeout

Sanitización de datos de la API

Caché multi-capa (partidos, goleadores, clasificaciones)

Diseño responsive mejorado

Roles ARIA para accesibilidad

📝 Créditos
Diseñado y programado por: Airam92

API de datos: wcup2026.org

Fuentes: Google Fonts (Orbitron, Inter)

Banderas: Emojis Unicode


