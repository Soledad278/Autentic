# Autentic
SDK Java - Framework para la explotación de aplicaciones que requieren autenticación de tarjetas

 + [Instalación](#instalacion)
	+ [Versiones de Java soportadas](#Versionesdejavasoportadas)
	+ [Versiones de Android soportadas](#Versionesdeandroidsoportadas)
  + [Uso](#uso)		
    + [Inicializar la clase correspondiente al conector (Autentic\Sdk)](#initconector)
 
 
 
<a name="instalacion"></a>		
## Instalación
Se debe descargar la última versión del SDK desde el botón Download ZIP del branch master.


Una vez descargado y descomprimido el SDK JAVA actualizado, tenés que realizar el import a tu proyecto:
```xml
dependencies {
    compile fileTree(dir: 'libs', include: ['*.jar'])
    testCompile 'junit:junit:4.12'
    compile project(path: ':autenticapi')
}
```

Una vez descargado se deben hacer los siguiente import.
```java
import com.tesis.autentic.ui.M1CardActivity;
```
<a name="Versionesdejavasoportadas"></a>   
####1. Versiones de Java soportadas
La versi&oacute;n implementada de la SDK, esta testeada para versiones desde Java 7 en adelante con JAX-WS.

<a name="Versionesdeandroidsoportadas"></a>   
####2. Versiones de Android soportadas
     Android 2.0 o superior
 
Todos los buil.gradle deben tener el mismo targetSdk. Versiones utilizadas:

     targetSdk = API 23: Android 6.0 (Marshmallow)
  
     minSdkVersion = 19 Android 4.4 (KitKat).

<a name="uso"></a>		
## Uso	
<a name="initconector"></a>
####Inicializar la clase correspondiente al conector (Autentic\Sdk).

     Intent intent = new Intent(Activity_Origen.this, M1CardActivity.class);

     intent.putExtra("usuario", usr);

     startActivity(intent);

Como parámetro se debe pasar el usuario registrado en autentic.
