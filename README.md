# FacialRecognitionJs

Aplicación sencilla para probar el uso de [WebGazer]('https://webgazer.cs.brown.edu/')

Una librería pública hecha por estudiantes de la universidad de Brown

Utiliza la camara del browser sin importar el dispositivo y hace seguimiento de la vista, devuelve la posición de la vista calibrandose a sí misma con los clicks del mouse.


Para correr está app es necesario correrla en un servidor https, por lo cual el package.json hace referencia a certificados que deben estar en root del proyecto.

---

## Para hacer los certificados si lo quieres correr con un server básico de js:
* Instalar [OpenSSL]('https://www.openssl.org/source/')
* `openssl genrsa -out key.pem 2048`
* `openssl req -new -key key.pem -out csr.pem`
* `openssl x509 -req -days 9999 -in csr.pem -signkey key.pem -out cert.pem`
* Colocar estos archivos en el root del proyecto.

* Correr la aplicación en Local `npm start`

----
Para poder correr necesita acceso a la camara