# README de nodepop

1.  Base de datos: 
    +   Conectada con localhost/3000 a Nodepop
    +   Tiene dos colecciones: anuncios y usuarios

2.  Filtrados:
    +   Acepta filtro por precio en rangos 10<=precio, 10<=precio<=50, precio<=50. (routes/api/anuncios.js:37) 
    +   Acepta filtro por nombre. (routes/api/anuncios.js:23)
    +   Acepta filtro por venta (venta = true) / búsqueda (venta = false). (routes/api/anuncios.js:24)
    +   Acepta filtro por tags. (routes/api/anuncios.js:25)

3.  Creación:
    +   Acepta los tags work, lifestyle, motor y mobile. (routes/api/anuncios.js:132)
    +   Los usuarios tienen nombre, email y clave. (models/Usuario.js:7)
    +   Los anuncios pueden tener nombre, tipo de venta, precio, foto y tags. (models/Anuncio.js:7)

4.  Autenticación:
    +   Se realiza a través de json web token (lib/jwtAuth.js)
