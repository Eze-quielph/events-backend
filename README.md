# Events-EventoX

# Pasos para levantar proyecto:

1. Clonar Repositorio.
2. Instalar dependencias con el comando: `npm install`.
3. Crear variables de entorno de desarrollo en un archivo `.env.development` usando el archivo `.env.template` por referencia
4. Crear variables de entorno de produccion en un archivo `.env.production` usando el archivo `.env.template` por referencia
5. Si vas a ejecutar en desarrollo, ve al archivo `server.ts` y comenta el middleware https que es el siguiente: ```this.app.use((req: Request, res: Response, next: NextFunction) => {
  res.setHeader('Strict-Transport-Security', 'max-age=31536000');
  next();
});```
6. Para correr en Desarrollo usar el comando: `npm run start:dev`
7. Si vas a correr en Produccion, ejecutar el build: `npm run build`
8. Para correr en Produccion usar el comando: `npm run start:prod`
9. Puedes ver la documentacion de Swagger en: `http://localhost:port/docs`

# Arquitectura de la aplicacion

- Clean Architecture con DDD

# Requisitos de coolaboracion

1. Usar esLint para formateo de codigo.
2. Respetar Arquitectura y el uso de no dependencias ocultas.
3. Nunca pushear en Produccion o Desarrollo.
4. Siempre ejecuta el comando ```npm run precommit``` antes de subir tus cambios.
5. Utilizar logger para la captura de errores

# Recomendaciones

1. Siempre sanitizar el codigo con el adapter `ValidatorAdapters`.
2. Si no hay un metodo sanitizador para tu entrada, revisar documentacion de la libreria `validator` y crea un metodo que adapte lo que necesitas.

# Colaboradores:

1. Ezequiel Benitez:
   - Github: [https://github.com/Eze-quielph]
   - Linkedin: [https://www.linkedin.com/in/ezequiel-benitez2203/]
   - Portafolio: [https://ezequiel-benitez.vercel.app/]
   - Contacto: ezequiel_developer@outlook.com
