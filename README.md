# 📊 Reporte Agente Virtual de Biología

<p align="center">
  <img src="logo.png" alt="UXDigital Logo" width="200">
</p>

Dashboard de analíticas en tiempo real para el chatbot de biología educativa con inteligencia artificial desarrollado por **UXDigital**.

## 🚀 Acceso al Dashboard

**[🔗 Abrir Reporte](https://uxdigitalchile.github.io/Dashboard_Biologia/index.html)**

---

## 📈 Funcionalidades

### Métricas en Tiempo Real
- ✅ **Total de Conversaciones**: Cantidad total de interacciones registradas
- 👥 **Sesiones Únicas**: Número de usuarios diferentes que han usado el chatbot
- ⭐ **Rating Promedio**: Calificación promedio otorgada por los usuarios (escala 1-5)
- 📊 **Total de Calificaciones**: Cantidad de evaluaciones recibidas

### Visualizaciones Interactivas
- 📅 **Conversaciones por Día**: Gráfico de línea que muestra la evolución temporal de las interacciones
- ⏰ **Conversaciones por Hora**: Distribución de uso durante las 24 horas del día
- ⭐ **Distribución de Calificaciones**: Gráfico de barras con ratings del 1 al 5
- 📈 **Ratings por Día**: Evolución temporal del promedio de calificaciones

### Gestión de Datos
- 📧 **Emails de Usuarios**: Visualización de correos electrónicos recopilados automáticamente
- 💬 **Historial de Conversaciones**: Tabla detallada con todas las interacciones
- 🕐 **Zona Horaria Chile**: Todas las fechas mostradas en hora local de Chile (UTC-3/UTC-4)
- 📄 **Paginación**: Visualización de 25 registros por página
- 💾 **Exportación CSV**: Descarga completa de datos para análisis externo

### Diseño Responsive
- 📱 **Optimizado para móviles**: Interfaz adaptable a smartphones
- 💻 **Compatible con tablets**: Diseño responsive para todo tipo de pantallas
- 🖥️ **Desktop**: Experiencia completa en computadores

---

## 🔑 Configuración

Para usar el dashboard necesitas configurar:

1. **URL de Supabase**: 
   - Tu URL de proyecto (ejemplo: `https://tuproyecto.supabase.co`)

2. **API Key (Anon/Public)**:
   - Clave pública de Supabase para acceso de lectura

### Primera Configuración

1. Abre el [dashboard](https://uxdigitalchile.github.io/Dashboard_Biologia/index.html)
2. Ingresa tu URL de Supabase
3. Ingresa tu API Key pública
4. Haz clic en "Conectar y Cargar Datos"

Las credenciales se guardan automáticamente en tu navegador (localStorage) para futuras visitas.

---

## 🛠️ Tecnologías

### Frontend
- **HTML5, CSS3, JavaScript**: Interfaz de usuario moderna y responsive
- **Chart.js**: Librería para visualizaciones interactivas de datos

### Backend & Base de Datos
- **Supabase (PostgreSQL)**: Base de datos relacional con API REST
- **Row Level Security (RLS)**: Políticas de seguridad para acceso controlado
- **Triggers automáticos**: Extracción inteligente de emails y ratings

### Automatización & AI
- **n8n**: Workflow automation para orquestación del chatbot
- **OpenAI GPT**: Modelo de lenguaje para respuestas del chatbot
- **Google Gemini File Search**: Sistema RAG para búsqueda en documentos de biología

---

## 📊 Arquitectura del Sistema

```
Usuario → n8n Chatbot → OpenAI GPT + Gemini RAG
                ↓
         PostgreSQL (Supabase)
                ↓
         Trigger Automático
         (Extrae email + rating)
                ↓
         Dashboard (GitHub Pages)
```

### Flujo de Datos

1. **Usuario interactúa** con el chatbot de biología
2. **n8n captura** la conversación y la envía a OpenAI/Gemini
3. **PostgreSQL almacena** cada mensaje en tabla `chat_rag_uxd`
4. **Trigger automático** detecta y extrae:
   - Email del usuario (patrón: `usuario@dominio.com`)
   - Rating (1-5 estrellas) cuando se solicita
5. **Dashboard consulta** datos vía Supabase REST API
6. **Visualización** en tiempo real de métricas y gráficos

---

## 📁 Estructura de Archivos

```
Dashboard_Biologia/
├── README.md                          # Este archivo
├── logo.png                           # Logo de UXDigital
├── dashboard_v3.html                  # Dashboard principal (USAR ESTA)
├── dashboard_v2_fixed.html            # Versión anterior
└── dashboard_Agente_Biologia_V1.html  # Primera versión
```

---

## 🔒 Seguridad

- ✅ RLS (Row Level Security) habilitado en Supabase
- ✅ Solo lectura pública mediante API Key anon
- ✅ Sin acceso a operaciones de escritura/eliminación
- ✅ Credenciales almacenadas localmente (no enviadas a terceros)

---

## 📞 Soporte

Para preguntas o soporte técnico, contacta a:

**UXDigital**  
🌐 Website: [uxdigital.cl](https://uxdigital.cl)

---

## 📝 Notas de Versión

### v3.0 (Actual)
- ✨ Nuevo título: "Reporte Agente Virtual de Biología"
- 🎨 Logo de UXDigital en el header
- 📱 Diseño completamente responsive
- 🕐 Corrección de zona horaria Chile (UTC-3)
- ⭐ Sistema de ratings 1-5 estrellas
- 📧 Extracción automática de emails

### v2.0
- 📊 4 gráficos interactivos con Chart.js
- 📄 Paginación de tabla (25 registros)
- 💾 Exportación a CSV
- 🎨 Mejoras visuales y UX

### v1.0
- 🚀 Lanzamiento inicial
- 📊 Métricas básicas
- 📋 Tabla de conversaciones

---

<p align="center">
  Desarrollado con ❤️ por <strong>UXDigital</strong>
</p>
