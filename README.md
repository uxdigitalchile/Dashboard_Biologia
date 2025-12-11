# 📊 Reporte Agente Virtual de Biología

<p align="center">
  <img src="logo.png" alt="UXDigital Logo" width="200">
</p>

Dashboard de analíticas en tiempo real para el chatbot de biología educativa con inteligencia artificial desarrollado por **UXDigital**.

## 🚀 Acceso al Dashboard

**[🔗 Abrir Reporte](https://uxdigitalchile.github.io/Dashboard_Biologia/)**

---

## 📈 Funcionalidades

### Métricas en Tiempo Real
- ✅ **Total de Conversaciones**: Cantidad total de interacciones registradas
- 👥 **Sesiones Únicas**: Número de usuarios diferentes que han usado el chatbot
- ⭐ **Rating Promedio**: Calificación promedio otorgada por los usuarios (escala 1-5)
- 📊 **Total de Calificaciones**: Cantidad de evaluaciones recibidas

### Visualizaciones Interactivas
- 📅 **Conversaciones por Día**: Gráfico de línea que muestra la evolución temporal
- ⏰ **Conversaciones por Hora**: Distribución de uso durante las 24 horas del día
- ⭐ **Distribución de Calificaciones**: Gráfico de barras con ratings del 1 al 5
- 📈 **Ratings por Día**: Evolución temporal del promedio de calificaciones

### Gestión de Datos
- 📧 **Emails de Usuarios**: Visualización de correos recopilados automáticamente
- 💬 **Historial de Conversaciones**: Tabla detallada con todas las interacciones
- 🕐 **Zona Horaria Chile**: Fechas en hora local de Chile (UTC-3/UTC-4)
- 📄 **Paginación**: Visualización de 25 registros por página
- 💾 **Exportación CSV**: Descarga completa de datos para análisis externo

### Diseño Responsive
- 📱 **Optimizado para móviles**: Interfaz adaptable a smartphones
- 💻 **Compatible con tablets**: Diseño responsive para todo tipo de pantallas
- 🖥️ **Desktop**: Experiencia completa en computadores

---

## 🔑 Configuración

### Primera Configuración

1. Abre el [dashboard](https://uxdigitalchile.github.io/Dashboard_Biologia/)
2. Ingresa tu **URL de Supabase** (ej: `https://tuproyecto.supabase.co`)
3. Ingresa tu **API Key pública** (anon key)
4. Haz clic en **"Conectar y Cargar Datos"**

Las credenciales se guardan automáticamente en tu navegador para futuras visitas.

---

## 🛠️ Tecnologías

### Frontend
- **HTML5, CSS3, JavaScript** - Interfaz responsive
- **Chart.js** - Visualizaciones interactivas

### Backend & Base de Datos
- **Supabase (PostgreSQL)** - Base de datos con API REST
- **Row Level Security (RLS)** - Seguridad de acceso
- **Triggers automáticos** - Extracción de emails y ratings

### Automatización & AI
- **n8n** - Workflow automation
- **OpenAI GPT** - Modelo de lenguaje
- **Google Gemini File Search** - Sistema RAG

---

## 📊 Arquitectura

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

---

## 📁 Estructura de Archivos

```
Dashboard_Biologia/
├── README.md      # Documentación
├── logo.png       # Logo de UXDigital
├── index.html     # Dashboard principal ⭐
└── ...           # Versiones anteriores
```

**Nota**: `index.html` es la página principal que se carga automáticamente.

---

## 🔒 Seguridad

- ✅ RLS habilitado en Supabase
- ✅ Solo lectura mediante API Key pública
- ✅ Sin acceso a escritura/eliminación
- ✅ Credenciales almacenadas localmente

---

## 📞 Soporte

**UXDigital**  
🌐 [uxdigital.cl](https://uxdigital.cl)

---

## 📝 Notas de Versión

### v3.1 (Actual)
- 🎨 Logo embebido en HTML (carga instantánea)
- 🔗 URL simplificada: index.html
- ✅ Sin dependencias externas para logo

### v3.0
- ✨ Título: "Reporte Agente Virtual de Biología"
- 📱 Diseño responsive completo
- 🕐 Zona horaria Chile corregida
- ⭐ Sistema de ratings 1-5

### v2.0
- 📊 Gráficos interactivos
- 📄 Paginación y CSV
- 🎨 Mejoras UX

### v1.0
- 🚀 Lanzamiento inicial

---

<p align="center">
  Desarrollado con ❤️ por <strong>UXDigital</strong>
</p>
