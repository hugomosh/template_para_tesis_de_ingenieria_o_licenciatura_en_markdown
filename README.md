# Template para tesis de ingenieria o licenciatura en markdown

Tesis para ingeniería o licenciatura usando Markdown, es una herramienta para aquellos que buscan crear una tesis para licenciatura, maestría o incluso doctorado y quieran concentrarse en el contenido primero, antes que otra cosa. Es una alternativa efectiva para softwares de _what you see, what you get_ WYSWYG como Word que hacen complicado el uso de fórmulas y diagramas. Markdwon es tan flexible pero‹ mucho más práctico y directo que las opciones de _Latex_. Este proyecto tiene las ventajas de ambos mundos ya que permite concentrase en la escritura con Markdown pero gracias a _pandoc_ obtienes un documento en Word, HTML y/o PDF_Latex.

+ [Template para tesis de ingenieria o licenciatura en markdown](#template-para-tesis-de-ingenieria-o-licenciatura-en-markdown)
  + [Organización del template](#organización-del-template)
  + [Guía de uso](#guía-de-uso)
    + [Requerimientos](#requerimientos)
    + [Primeros pasos](#primeros-pasos)
  + [¿Problemas? Troubleshooting](#problemas-troubleshooting)
    + [Make Error 43](#make-error-43)
  + [Cosas que deberías saber](#cosas-que-deberías-saber)
  + [Agradecimientos](#agradecimientos)
  + [PH (Por hacer) y contribuciones](#ph-por-hacer-y-contribuciones)

## Organización del template
| Archivo o Carpeta   | Descripción                                                  |
| ------------------- | ------------------------------------------------------------ |
| README.md           | Instrucciones                                                |
| License.md          | MIT License                                                  |
| Makefile            | instrucciones para producir los archivos                     |
| `source/`           |                                                              |
| `source/resources/` | En donde van las figuras, imágnes o recursos a insertar      |
| `output/`           | Archivos de salida (documentos finales en .pdf, docx, .html) |

## Guía de uso

### Requerimientos

- **Editor de textos** Sublime, VSCode, etc. Recomiendo VSCode y las extensiones de Markdown All in One así como Spanish Code Spell Checker
- Un **distribución de Latex**. Por ejemplo [MacTex]
- [Pandoc]() para conevertir los textos Markdown a un archivo con la extensión de tu preferencia (.docx, pdf, .html, .tex, etc.)
- Git para el control de versiones

### Primeros pasos

1. Asegurate de tener todos los requerimientos
2. Crea un fork de este repositorio (puede ser privado)
3. Clona el repositorio en tu computadora (o descarga el archivo ZIP)
4. Ingresa a la carpeta del proyecto
5. Ejecuta make html para revisar que todo en orden
6. Ejecuta make pdf para asegurar que tienes todo instalado
7. Si no hay problemas, puedes comenzar por revisar los capítulos de ejemplo y empezar a escribr
8. Si tienes algún problema revisa primerlo la sección de [**_Troubleshooting_**](#problemas-troubleshooting))

## ¿Problemas? Troubleshooting

### Make Error 43

En caso de error (por ejemplo `make: *** [pdf] Error 43`) ejecuta en la terminal (dentro del folder) los siguientes comandos:

```
sudo tlmgr install truncate
sudo tlmgr install tocloft
sudo tlmgr install wallpaper
sudo tlmgr install morefloats
sudo tlmgr install sectsty
sudo tlmgr install siunitx
sudo tlmgr install threeparttable
sudo tlmgr update l3packages
sudo tlmgr update l3kernel
sudo tlmgr update l3experimental
```

## Cosas que deberías saber

Tips o consejos que debes saber:

- Cada capítulo debe terminar con almenos una linea vacia (un enter). De lo contrarío el título del siguiente capítulo puede que no se dibuje bien.
- Añade dos espacios al final de una linea para forzar el salto de párrafo.
- Este tempalte de Markdown utiliza [Pandoc](http://pandoc.org/MANUAL.html) por lo que te recomiendo ver el manual de uso.

## Agradecimientos

El template está inspirado y se debe en gran parte a los siguientes proyectos:

[Dr Mathew Lipson](https://www.theurbanist.com.au) y su template de [_phd_thesis_markdown_](https://github.com/matlipson/phd_thesis_markdown).
## PH (Por hacer) y contribuciones

- []


Para contribuir _fork_ y edita el proyecto, luego mando un _pull request_.