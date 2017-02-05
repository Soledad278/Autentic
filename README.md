# Autentic
SDK Java - Framework para la explotación de aplicaciones que requieren autenticación de tarjetas

 + [Instalación](#instalacion)
 	+ [Versiones de Java soportadas](#Versionesdejavasoportadas)
 	+ [Generalidades](#general)
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
La versi&oacute;n implementada de la SDK, esta testeada para versiones desde Java 6 en adelante con JAX-WS.

<a name="initconector"></a>
####Inicializar la clase correspondiente al conector (Autentic\Sdk).

Intent intent = new Intent(Activity_Origen.this, Activity_Destino.class);
intent.putExtra("usuario", usr);
startActivity(intent);
