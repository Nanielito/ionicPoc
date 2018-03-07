[![N|Solid](http://koladas.com.ve/wp-content/uploads/2015/03/Koladas_separador.png)](http://koladas.com.ve/)
# Ionic LlamaVan POC

Para desarrollar este readme use un editor de MarkDown online:
https://dillinger.io/

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

### brew
```sh
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

#### Node
Descagar e instalar la ultima version de node
- https://nodejs.org/es/

#### Ionic cuenta
Crear una cuenta para poder hacer uso del framework
https://dashboard.ionicjs.com/signup

#### Ionic install
Ejecutar el comando de instalaccion 
- https://ionicframework.com/getting-started/

```sh
$ npm install -g cordova ionic
```

#### Crear proyecto 

La idea es tener varios proyecticos en este repo para ir armando las pruebas

```sh
$ cd ~/.turuta/projectLlamaVan/ionicPoc
$ ionic start nombreApellido blank
```
preguntas y respuestas durante la instalacion:

- Would you like to integrate your new app with Cordova to target native iOS and Android? (y/N) y

- Install the free Ionic Pro SDK and connect your app? (Y/n) N

#### Instalacion de plataforma android 

Se de correr el siguiente comando para la plataforma android

En tal caso no se tenga el SKD Manager ver el tutorial de Instalacion de Android Studio

```sh
$ ionic cordova platform add android@6.4.0

```

#### build y deploy de la app en el celular android

Conectar el cel y correr el siguiente comando

```sh
$ ionic cordova run android

```
 
#### Listado de posibles errores:


 -CordovaError: Could not find an installed version of Gradle either in Android Studio,
or on your system to install the gradle wrapper. Please include gradle 
in your path, or install Android Studio ( instala gradel pe won)

- https://gradle.org/install/

```sh
$ brew install gradle

```

> You have not accepted the license agreements of the following SDK components:
  [Android SDK Platform 26, Android SDK Build-Tools 26.0.2].
  Before building your project, you need to accept the license agreements and complete the installation of the missing components using the Android Studio SDK Manager.
  Alternatively, to learn how to transfer the license agreements from one workstation to another, go to http://d.android.com/r/studio-ui/export-licenses.html (abre tu android studio y descarga la ultima version del sdk 6)


#### Link para instalar entorno android

- https://cordova.apache.org/docs/en/7.x/guide/platforms/android/


#### Otras instalaciones (en construcción)

| Instalar | README |
| ------ | ------ |
| JAVA | [instalacion/java/README.md][PlDb] |
| PATH | [instalacion/path/README.md][PlGh] |
| Ionic pro | [instalacion/ionic/README.md][PlGh] |
| Android Studio | [instalacion/android/README.md][PlOd] |
| SDK Manager | [instalacion/android/README.md][PlOd] |
| Gradel | [instalacion/android/README.md][PlOd] |
| Xcode | [instalacion/xcode/README.md][PlMe] |
| Otras dependencias | [instalacion/dependencias/README.md][PlGa] |


##### alias de comandos ionic

```sh
alias io="ionic"
alias cdv="cordova"
alias ioc="ionic cordova"
alias iog="ionic generate"
alias iorm="rm -rf node_modules/ && rm -rf plugins/ && rm -rf www/ && rm -rf platforms/ && rm -rf .sourcemaps/"
alias ioi="npm i && ionic cordova build"
alias ior="ionic cordova run"
alias ioan="ionic cordova run android --device"
alias cpl="cordova plugin list"
alias ioap="ionic cordova plugin add"
alias iormp="ionic cordova plugin rm"
```