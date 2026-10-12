# Acortador de URL — Node.js, Express y MongoDB

Aplicación web renderizada del lado del servidor para administrar enlaces cortos. Permite guardar una URL original, generar un código breve y redirigir a la dirección de destino.

## Funcionalidades

- Listar enlaces guardados.
- Crear enlaces cortos mediante códigos generados con Nano ID.
- Editar y eliminar enlaces.
- Redirigir desde el código corto hacia la URL original.
- Validar los formularios mediante middleware.

## Tecnologías

- Node.js
- Express
- Express Handlebars
- MongoDB y Mongoose
- Nano ID
- dotenv

## Organización del proyecto

- `routes/`: rutas de la aplicación.
- `controllers/`: lógica para gestionar los enlaces.
- `models/`: modelo de datos.
- `database/`: conexión con MongoDB.
- `middlewares/`: validación de solicitudes.
- `views/`: plantillas Handlebars.
- `public/`: recursos estáticos.

## Ejecutar localmente

Requiere Node.js, npm y una instancia de MongoDB accesible.

```bash
git clone https://github.com/cgldev/hbs-express-mongoDB.git
cd hbs-express-mongoDB
npm install
```

Creá un archivo `.env` en la raíz y configurá la cadena de conexión:

```env
URI=mongodb://127.0.0.1:27017/acortador
PORT=5000
```

Luego iniciá la aplicación:

```bash
npm start
```

El script `npm run dev` también está disponible en versiones de Node.js que soporten `--watch`.

## Estado del proyecto

Proyecto de aprendizaje. Antes de utilizarlo en producción, sería necesario reforzar el control de acceso, la seguridad de las rutas que modifican datos, la validación de URL y el manejo de errores.

## Autor

César Gimenez Lascano — [@cgldev](https://github.com/cgldev)
