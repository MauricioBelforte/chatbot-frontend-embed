
## 🧩 chatbot-frontend-funcional

**Frontend funcional del chatbot IA**, con lógica desacoplada y presentación autónoma. Diseñado para mostrar el comportamiento del motor IA en producción, incluyendo armado de prompts, extracción de contexto y renderizado estilo chat.

Este front se conecta con el fetch en `https://motor-ia-backend.vercel.app/api/chatbotApi`

---

### 🚀 ¿Qué incluye este módulo?

Este repositorio contiene una interfaz completa que permite:

- Renderizar respuestas IA en pantalla tipo chat (`chatbotVisual.js`)
- Construir prompts personalizados (`lib/armarPrompts.js`)
- Extraer y procesar contexto desde respuestas IA (`lib/extraerContexto.js`)
- Ejecutarse como demo técnica directa desde `index.html`

> Parte clave del ecosistema IA modular, junto con [`motor-ia-backend`](https://github.com/MauricioBelforte/motor-ia-backend)

---

### 🛠️ Estructura del proyecto

```
/
├── index.html              # Interfaz principal con layout independiente
├── styles.css              # Estilos visuales tipo chat
├── chatbotVisual.js        # Renderizado y conexión con backend
├── lib/
│   ├── armarPrompts.js     # Construcción de prompts IA
│   ├── extraerContexto.js  # Procesamiento de respuestas IA
├── LICENSE                 # Licencia MIT
├── README.md               # Este archivo 📘
```

---

### 📦 Cómo usar

1. Cloná el repo:

```bash
git clone https://github.com/MauricioBelforte/chatbot-frontend-funcional.git
```

2. Configurá el endpoint en `chatbotVisual.js`:

```js
const API_ENDPOINT = 'https://motor-ia-backend.vercel.app/api/chatbotApi';
```

3. Abrí `index.html` directamente o desplegalo como demo estática en GitHub Pages / Netlify.

---

### 🎯 ¿Por qué es funcional?

Este módulo no sólo visualiza: incorpora lógica IA propia. Desde cómo se arma el prompt hasta cómo se filtra y presenta la respuesta, este frontend representa fielmente el comportamiento del sistema en producción.

---

### 📚 Este módulo en el ecosistema

| Repositorio                   | Rol dentro del sistema                      | Estado       |
|-------------------------------|---------------------------------------------|--------------|
| `chatbot-frontend-funcional` | Frontend funcional del chatbot IA personal  | Renombrado ✅ |

---

### 🧠 ¿Por qué no tiene backend propio?

Este módulo **no incluye carpeta `api/` ni backend directo en Vercel** porque está diseñado como *frontend desacoplado*, conectado a un motor IA ya desplegado:

- Se evita duplicar lógica backend en cada repo, manteniendo el sistema modular y con responsabilidad clara por bloque.
- El backend principal vive en [`motor-ia-backend`](https://github.com/MauricioBelforte/motor-ia-backend), que **sí expone el endpoint `/api/chatbotApi`** vía Vercel usando la carpeta `api/`.
- Este enfoque permite escalar, versionar o reemplazar el motor IA sin tocar la interfaz.

> Así, cada módulo cumple su rol específico: este front visualiza e interpreta, el backend procesa y responde.

---
