# 📌 Portafolio de Deck Maurice

Este es un portafolio profesional desarrollado con **Next.js 15** y **Tailwind CSS**, con un enfoque modular y escalable. Aquí encontrarás instrucciones detalladas para modificar, mejorar y escalar el proyecto.

---

## 🚀 **Cómo funciona este proyecto**

Este portafolio está estructurado en **componentes reutilizables** y **páginas** dentro de la carpeta `app/`. La navegación y el diseño se manejan con **Next.js**, lo que permite una carga rápida y eficiente.

📂 **Estructura del Proyecto**
```
portafolio/
│── app/                 # Páginas principales del sitio
│   ├── layout.js        # Layout global (Navbar, Footer, etc.)
│   ├── page.js          # Página de inicio (index)
│   ├── about/           # Página "Sobre mí"
│   ├── projects/        # Página de proyectos
│   ├── contact/         # Página de contacto
│── components/          # Componentes reutilizables
│   ├── Navbar.js        # Barra de navegación
│   ├── Hero.js          # Sección principal
│   ├── ProjectCard.js   # Tarjetas de proyectos
│   ├── About.js         # Sección "Sobre mí"
│   ├── ContactForm.js   # Formulario de contacto
│   ├── Footer.js        # Pie de página
│── public/              # Imágenes y otros recursos estáticos
│── styles/              # Estilos globales y Tailwind CSS
│── tailwind.config.js   # Configuración de Tailwind CSS
│── package.json         # Dependencias del proyecto
│── README.md            # Documentación del proyecto
```

---

## 🔧 **Instalación y Configuración**

1️⃣ **Clonar el repositorio**  
```sh
git clone https://github.com/tu-usuario/portafolio.git
cd portafolio
```

2️⃣ **Instalar dependencias**  
```sh
npm install
```

3️⃣ **Ejecutar el servidor de desarrollo**  
```sh
npm run dev
```
➡️ El sitio estará disponible en **http://localhost:3000**

---

## ✨ **Cómo agregar componentes**

🔹 **Paso 1:** Crea el archivo del componente en `components/`  
Ejemplo: `components/Button.js`

🔹 **Paso 2:** Define el componente en React con Tailwind
```jsx
export default function Button({ text }) {
  return (
    <button className="bg-blue-500 text-white px-4 py-2 rounded-lg">
      {text}
    </button>
  );
}
```

🔹 **Paso 3:** Importarlo en una página o componente
```jsx
import Button from "@/components/Button";

export default function Home() {
  return (
    <div>
      <Button text="Ver Proyectos" />
    </div>
  );
}
```

---

## 🛠 **Cómo agregar páginas nuevas**

🔹 **Paso 1:** Crea una carpeta dentro de `app/` con el nombre de la página (ejemplo: `services/`).

🔹 **Paso 2:** Crea un archivo `page.js` dentro de la nueva carpeta:
```jsx
export default function Services() {
  return (
    <div className="p-6">
      <h1 className="text-2xl font-bold">Mis Servicios</h1>
      <p>Ofrezco desarrollo web profesional.</p>
    </div>
  );
}
```

🔹 **Paso 3:** Agregar el enlace en `Navbar.js`:
```jsx
<li><a href="/services" className="hover:text-gray-400">Servicios</a></li>
```

➡️ Ahora puedes acceder a **http://localhost:3000/services**

---

## 🚀 **Cómo escalar el proyecto**

1️⃣ **Modularizar el código** → Separa el código en componentes reutilizables.
2️⃣ **Optimizar imágenes** → Usa `next/image` para una mejor performance.
3️⃣ **SEO y Accesibilidad** → Agrega metaetiquetas y asegúrate de que el sitio sea accesible.
4️⃣ **Agregar animaciones** → Usa `framer-motion` para transiciones fluidas.
5️⃣ **Deploy en Vercel** → Despliega tu portafolio con un solo comando:
```sh
vercel
```

---

## 📌 **Conclusión**

Este portafolio está diseñado para ser **rápido, escalable y fácil de mantener**. Usa este README como guía cada vez que necesites modificar o expandir el proyecto. 💪🔥

¿Tienes dudas? ¡Sigue iterando y mejorando! 🚀

