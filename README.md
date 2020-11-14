# Curso de tailwind

# Aprendiendo Tailwind y haciendo un clon de Spotify

![img](https://github.com/solisjoaquin/tailwindcss/blob/main/public/images/screen.png)

## iniciar proyecto

```
npm init -y
```

## instalar 

```
npm i tailwindcss autoprefixer postcss-cli
```

## iniciar tailwind

```
 npx tailwindcss init
```

 * crear archivo postcss.config.js que requiera tailwind y prefixer

```
 module.exports = {
    plugins: [
        require('tailwindcss'),
        require('autoprefixer')
    ]
}
```

 * instalar plugins de Tailwind: Tailwind CSS IntelliSense

 * crear carpetas de public / index.html y css /  tailwind.css

 * conectar el css al html  --> link:css

```
 <link rel="stylesheet" href="css/style.css">
```

 Este archivo style todavia no esta creado, y se guardara en una carpeta css pero esta carpeta esta dentro de public. Se creara en el siguiente paso.

 * en el package.json crear el script: 

```
 "build": "postcss css/tailwind.css -o public/css/style.css"
```


 * ejecutar el comando
 
 ```
  npm run build
```

 Si hay problemas con el prefixer puedes instalar una version compatible 

```
 npm install autoprefixer@'9.8.6' 
```

 # Ahora ya tienes Tailwind en tu proyecto


 ## Como obtener el archivo full con todos los colores y variables de tailwind

 ```
 npx tailwindcss init tailwind.config.full.js --full
```
    

