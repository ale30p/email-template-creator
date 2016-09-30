# Foundation for Emails Template

[![devDependency Status](https://david-dm.org/zurb/foundation-emails-template/dev-status.svg)](https://david-dm.org/zurb/foundation-emails-template#info=devDependencies)

**Please open all issues with this template on the main [Foundation for Emails](http://github.com/zurb/foundation-emails/issues) repo.**

This is the official starter project for [Foundation for Emails](http://foundation.zurb.com/emails), a framework for creating responsive HTML devices that work in any email client. It has a Gulp-powered build system with these features:

- Handlebars HTML templates with [Panini](http://github.com/zurb/panini)
- Simplified HTML email syntax with [Inky](http://github.com/zurb/inky)
- Sass compilation
- Image compression
- Built-in BrowserSync server
- Full email inlining process

## Installation

To use this template, your computer needs [Node.js](https://nodejs.org/en/) 0.12 or greater. The template can be installed with the Foundation CLI, or downloaded and set up manually.

Then open the folder in your command line, and install the needed dependencies:

```bash
cd projectname
npm install
```

## Build Commands

Run `npm start` to kick off the build process. A new browser tab will open with a server pointing to your project files.

Run `npm run build` to inline your CSS into your HTML along with the rest of the build process.

Run `npm run litmus` to build as above, then submit to litmus for testing. *AWS S3 Account details required (config.json)*

Run `npm run zip` to build as above, then zip HTML and images for easy deployment to email marketing services.

USO FC.
* En la carpeta layouts esta el base, de cual heredan todas los templates en la carpeta pages.
* En la carpeta pages estan los 4 emails nuestros + index que es el ejemplo que esta roto.
* En la carpeta partials estan los pedazos de template que se usa en las pages.
* Corriendo el comando npm run build, cada cambio que se haga te regenera en la carpeta dist el
html compilado, este para los mails debe ser formateado por alguna herramienta[1] online para que los
emails no se corten.(Me pasaba que un link de una imagen se rompia por un salto de linea que generaba
el navegador)
* copia y pegar el resultado en el template correspondiente y listo.

TODO:
1) El proceso es engorroso, se podria mejorar si no compilara el html en una linea, imagino que se
puede sacar eso de gulp.


[1]
[Formatter](http://www.freeformatter.com/html-formatter.html)