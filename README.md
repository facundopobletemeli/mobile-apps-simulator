# mobile-apps-simulator
Apps para correr en el simulador iOS/Android

## iOS

### 1.- Instalar Simuladores

1. Instalar XCode
2. Descargar Simualdores

### 2.- Correr App

#### Listar simuladores
> $ xcrun simctl list

#### Iniciar un simulador
> $ xcrun instruments -w {ID-SIMULADOR ó NOMBRE-SIMULADOR}

#### Instalar App
    By Booted device:
        > $ xcrun simctl install booted ~/Desktop/Applicacion.app

    By Device Name / ID
        > $ xcrun simctl install {ID-SIMULADOR ó NOMBRE-SIMULADOR} ~/Desktop/Applicacion.app
        
### Devs: Generar .app
Iniciar la app desde el XCode y en la consola de debug correr el comando:

> po NSHomeDirectory()

Output:
> /Users/**{USUARIO}**/Library/Developer/CoreSimulator/Devices/C970ECA1-E369-4F8D-BAD7-1171E0FFD744/data/Containers/Data/Application/{ID}

Buscar el .app en la carpeta

> /Users/**{USUARIO}**/Library/Developer/CoreSimulator/Devices/C970ECA1-E369-4F8D-BAD7-1171E0FFD744/data/Containers/Bundle/Application/...
