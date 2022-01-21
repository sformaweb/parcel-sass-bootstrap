## Notas e consideracións
* Vaise crear un pequeno sitio web empregando o framework de CSS Bootstrap, o preprocesador Sass e o bundle de JS Parcel.

* Debemos instalar primeiro dende a consola o manexador de paquetes npm, Bootstrap e Sass.

* Crearase unha árbore de directorios con distintas carpetas. Será no arquivo style.scss no que deberemos modificar o estilo da nosa web. Nel tamén se deberán importar os módulos que vaiamos a utilizar, aloxados en /node_modules/bootstrap/scss/.

  > **Nota**: A orde dos imports no arquivo style.scss é relevante: 1. functions 2.variables 3.mixins

* Debemos executar o servidor dende a consola utilizando o comando "npm start". Durante o proceso de creación do sitio é necesario resetealo algunha vez para que os cambios se executen ou ben para eliminar a caché de erros.

* No arquivo de configuración package.json debemos engadir Parcel no apartado de scripts co seguinte código: "start":"parcel ./src/index.html

* Os compoñentes do sitio son:

  * un header con menú;

  * un footer

  * e un formulario cos estilos de Bootstrap e cun script que permite a validación.*

    > ***Importante**: Engadir o script da validación antes de pechar a etiqueta de <body> e o index.js no <head>.

* Para o procesamento dos datos creouse un arquivo PHP que recolle a información do formulario e móstraa en pantalla. Debe introducirse na carpeta dist e no arquivo index.html introducir os seguintes atributos no formulario: action="nomearquivo.php" method="POST". Ademáis, debemos engadirlle un atributo name a todos os inputs do formulario que se recollerán da seguinte maneira no arquivo PHP: echo "Frase a mostrar en pantalla: ". $__POST[' name_'].

