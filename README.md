
## 🧩 chatbot-frontend-embed

**Frontend estático y embebible para IA conversacional**, desacoplado del backend, listo para integrarse en landings, portfolios o demos que consumen respuestas desde APIs externas.

---

### 🚀 ¿Qué es esto?

Este repositorio contiene una interfaz HTML + JS minimalista que permite:

- Enviar prompts a un motor IA externo vía `fetch`
- Renderizar respuestas en pantalla tipo chat
- Ser embebida fácilmente en cualquier página estática

> Ideal para demos de motores IA custom, portfolios técnicos o pruebas con backends desacoplados como [`chatbot-backend-vercel`](https://github.com/MauricioBelforte/chatbot-backend-vercel)

---

### 🛠️ Estructura del proyecto

```
/
├── index.html          # Interfaz principal
├── style.css           # Estilos embebibles
├── script.js           # Lógica básica: prompts + fetch + render
├── README.md           # Este archivo :)
```

---

### 📦 Cómo usar

1. Cloná el repo:

```bash
git clone https://github.com/MauricioBelforte/chatbot-frontend-embed.git
```

2. Configurá el endpoint en `script.js`:

```js
const API_ENDPOINT = 'https://mi-backend.vercel.app/api/chat';
```

3. Abrí `index.html` directamente o hostealo en GitHub Pages / Netlify / cualquier proveedor estático.

---

### 🎯 Integración con backend desacoplado

Podés conectar este frontend con motores como `chatbot-backend-vercel`, que aceptan prompts y devuelven respuestas IA vía HTTP.

> No requiere lógica interna de generación. Solo envía y renderiza.

---

### 🔐 Seguridad y buenas prácticas

- Este repo no maneja claves ni lógica confidencial.
- No incluye `.env`: el endpoint se define directamente en `script.js`.
- Podés agregar soporte para `.env` si lo usás en proyectos con bundlers o frameworks.

---

### 👥 Colaboración y adaptación

Este proyecto está pensado para:

- Ser clonado y adaptado a cualquier caso de uso IA embebido
- Servir como template para desarrolladores que quieren mostrar motores custom
- Usarse como módulo frontend desacoplado dentro de ecosistemas más amplios

---

### 📄 Licencia

Este proyecto está bajo la licencia MIT.  
Podés usarlo, modificarlo y distribuirlo libremente, siempre que incluyas el aviso de copyright correspondiente.

> Consultá el archivo [`LICENSE`](./LICENSE) para más detalles.

---

