# UNED_Maple_Demo

Pequeña demo del proyecto UNED para Maple con versión Tutor 15.2.0

## Descarga:

git clone https://github.com/srPepo/UNED_Maple_Demo.git \
  "$(tutor config printroot)/env/build/openedx/themes/UNED_maple_demo"



## Montaje: 

### 1 (Opcional) Reiniciar la plataforma --(todos los parámetros son configurados automáticamente en función de cómo se cubran las respuestas):

`tutor local launch`


### 2 Reiniciar la imagen de openedx y compilar el tema:

`tutor images build poenedx`


### 3 Iniciar los parámetros configurados con el launch de Tutor:

`tutor local start -d`


### 4 Establecer el tema 

`tutor local do settheme UNED_maple_demo` -> para local

`tutor dev do settheme UNED_maple_demo` -> para dev


### 5 Iniciar el lms y cms:

`tutor local start` -> para local

`tutor dev start` -> para dev

`tutor dev start lms` -> solamente iniciando lms

`tutor dev start cms` -> solamente iniciando cms


### 6 Abrir en el navegador la dirección indicada en el montaje de tutor (paso 1), por defecto será:

`http://local.overhang.io/` -> para local

`http://local.overhang.io:8000/` -> para dev





