[![N|Solid](http://koladas.com.ve/wp-content/uploads/2015/03/Koladas_separador.png)](http://koladas.com.ve/)
# Pruebas de Concepto Ionic LlamaVan

Para desarrollar este readme use un editor de MarkDown online:
https://dillinger.io/


[![N|Solid](http://koladas.com.ve/wp-content/uploads/2015/03/Koladas_separador.png)](http://koladas.com.ve/)

#### Paso 1
Como primer paso y buena practica asociar via ssh el github. Como generar el ssh key y asociarlo:
- https://help.github.com/articles/connecting-to-github-with-ssh/
- https://www.youtube.com/watch?v=TCcWwUgQe8s
  
#### Paso 2
Hacer el git clone del repo en un directorio con nombre  projectLlamaVan

> ejemplo: TuRutaPreferidaWorspace/projectLlamaVan

```sh
$ cd projectLlamaVan
$ git clone git@github.com:pitajuan/ionicPoc.git
$ cd ionicPoc
```

#### Paso 3 Installs

#### Node
Descagar e instalar la ultima version de node
- https://nodejs.org/es/

#### Ionic cordova
Ejecutar el siguiente comando para la instalacion
para la instalacion te puedes guiar del siguiente link
- https://ionicframework.com/getting-started/

```sh
npm install -g cordova ionic
```

#### Crear un proyecto dentro del repocon tu nombre

```sh
$ cd ~/.turuta/projectLlamaVan/ionicPoc
$ ionic start nombreApellido blank
```
preguntas y respuestas durante la instalacion:

- Would you like to integrate your new app with Cordova to target native iOS and Android? (y/N) y

- Install the free Ionic Pro SDK and connect your app? (Y/n) N


| Instalar | README |
| ------ | ------ |
| JAVA | [instalacion/java/README.md][PlDb] |
| PATH | [instalacion/path/README.md][PlGh] |
| Ionic pro | [instalacion/ionic/README.md][PlGh] |
| Android Studio | [instalacion/android/README.md][PlOd] |
| Xcode | [instalacion/xcode/README.md][PlMe] |
| Otras dependencias | [instalacion/dependencias/README.md][PlGa] |