---
title: Guia Torrents Callampiaos
draft: false
---

Esta guía esta diseñada para que puedan descargar películas y series en torrent de manera fácil y rápida. Se basa en el uso de 2 programas; qBittorrent y VLC.

## Desmitificando los Torrents

He visto que varios tienen miedo de descargar torrents ya que pueden estar descargando un virus. Sin embargo, al descargar películas y series, los riesgos son mínimos, dado que el proceso no requiere ejecutar ningún programa o script. Debes abrir únicamente los siguientes tipos de archivos:

- **Archivos de video:** Los formatos más comunes son `.mp4`, `.avi` y `.mkv`. Otros menos utilizados son `.mov` y `.wmv`.
- **Archivos de subtitulos:** El mas común es `.srt`, rara vez van a ver un `.ass`, pero también es un archivo de subtitulos un poco mas avanzado.

> [!IMPORTANT]
> Los sufijos mencionados representan los caracteres finales después del punto. Es decir un archivo llamado `nombre.mp4.exe` deja de ser un archivo `mp4`.

> [!CAUTION]
> Nunca ejecutar archivos que te pidan permisos de administrador. Ni ejecutables como `.exe` y `.bat`. 

Con esta información, quiero reiterar que descargar torrents de películas o series es generalmente muy seguro, especialmente si utilizas las fuentes confiables que recomendaré más adelante.

## Instalación de programas 

En esta guía, utilizaremos dos programas de código abierto recomendados para el proceso de descarga y visualización de contenidos.

### qBittorrent

Recomiendo usar [qBittorrent](https://www.qbittorrent.org/download), un cliente de torrents de código abierto. Esta guía se basa principalmente en este cliente y su motor de búsqueda integrado.
#### Instalación de qBittorrent 

**Windows:** En este [link](https://www.fosshub.com/qBittorrent.html) seleccionen la opción `qBittorrent Windows x64`. Luego siguen los pasos típicos de instalación de un `.exe`.

**Mac:** Lo mismo que Windows. En este [link](https://www.fosshub.com/qBittorrent.html) seleccionen la opción `qBittorrent Mac OS X`. Instalan como cualquier `.deb`.

**Linux:** No creo que tengan Linux, pero si hay algún valiente con Linux me puede preguntar como instalarlo en su distro, ya que el proceso depende de que distro estén usando de Linux.

#### Instalación de motor de búsqueda 

Para instalar el motor de búsqueda dentro de qBittorrent se van a Tools, Search Engine y siguen los pasos hasta llegar a una ventana que se ve así:

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412130001.png)


Acá deben seleccionar Search plugins, en la esquina de abajo a la derecha.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412130338.png)

Esta lista les va a salir vacía pero si seleccionan `Check for updates`, se les van a instalar los recomendados.

Acá por temas de simpleza, les recomiendo desactivar Jackett y TorLock, haciendo doble click en donde sale enabled yes.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412130350.png)

Ya pueden cerrar esta ventana y van a ver que les aparece `Search` en la esquina superior izquierda. Acá podrán buscar cualquier torrent, las recomendaciones están en la siguiente sección.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412130610.png)
### VLC 
#### Instalación de VLC 

Me da paja escribir mucho acá, pero este es el [link](https://www.videolan.org/)

- **Windows:** Seleccionen `Windows 64bit`, siempre que tengan la opción seleccionen 64 bits, en cualquier programa.
- **Mac:** Selecciones `macOS` si tienen mac basado en intel, `macOS (Apple Silicon)` si tienen un mac con procesador `ARM` ya sea M1, M2 y M3, y todos sus derivados como M3SuperMaxXZ.
- **Linux:** Si tienen una store, desde ahí, si no, me preguntan.

## Proceso de Descarga de Torrents

### Busqueda de Torrent

Acá voy a generalizar mucho, por lo que la información no sera 100% correcta, pero siguiendo un par de guías van a encontrar el bueno pero no el mejor.

Entre mas seeders mas rápido pero no se guíen solo con eso.

**Encodings:** x264, h264, x265, h265 son los comunes, los 265 son mas modernos y sin conplicar el tema mantienen la calidad en menos espacio. un 265 de 2GB se va a ver mejor que un 264 de 2GB

#### Películas 
Recomiendo buscar de la siguiente manera:

`nombre_película + año`

Por ejemplo:

**Arrival 2016**

Busquen películas de mas de 1.5 GB, que no contengan la palabra `HDCAM`, esto en general significa que fue grabado con una cámara en el cine. Las mejores pesan unos 20 GB si son 264.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412132105.png)

Todos los demás son buenos dependiendo de cuanto pesen, `WEBRIP` significa que los sacan plataformas como Netflix, Apple TV, etc. `BlueRay` y `DVD` se entienden de donde vienen.

Un ejemplo de un torrent perfecto es:

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412134522.png)

Lo clave acá son:
- **x265:** codec, considerando que su peso es de 11 GB. Con x264 seria mas o menos el doble.
- **1080p:** resolución.
- **BluRay:** .
- **Japanese**: En este caso la película es japonesa, este flag hace referencia a que el audio es en japones. Mas adelante hablaremos de subtitulos.

#### Series  recomiendo buscar por temporada si la temporada esta lista. Esto ademas de descargar 1 solo link, facilitara también encontrar subtitulos mas fácilmente.

Para esto poner:

`nombre_serie temporada COMPLETE`

Por ejemplo:

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412140335.png)

Los resultados serán distintos al poner Season 1 o S01, busquen en ambos el mejor torrent.

### Descarga de Torrent

Al encontrar el torrent que te guste les dan doble click y les mostrara una ventana así:
![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412140529.png)

A la izquierda pueden seleccionar donde guardar el torrent, y a la derecha lo que están por descargar.
### Proceso del Torrent

#### Estados importantes 

- **Downloading:** Esto significa que el torrent está descargando datos activamente.
- **Seeding:** Una vez que la descarga de un torrent está completa, generalmente cambia al estado de "Seeding". Esto significa que estás subiendo partes del archivo torrent a otros usuarios. Acá recomiendo apretar el torrent y luego apretar el botón pausa. Debería cambiar al estado `Completed`.
- **Completed:** Muestra que el torrent ha terminado de descargar.
- **Stalled:** Indica que el torrent no está descargando ni subiendo activamente debido a la falta de actividad de red. Esto puede suceder si no hay "seeders" o "peers" disponibles.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412154002.png)

#### Pausa 
Como indique previamente es importante pausar el torrent una vez termine, así no gastan bandwidth en subir archivos.

#### Eliminación 
Una vez vean la serie o película completa pueden eliminar el archivo desde qBittorrent, con el botón remove.

![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412152753.png)

Luego es importante darle click a esta opción:
 
![Alt text](/Archives/torrentGuide/Pasted%20image%2020240412152815.png)

Si no solo eliminaran el link al torrent y no los archivos de este.
## Subtitulos 
### Descarga 
Paginas que uso para descargar son:

- [OpenSubtitles.org](https://www.opensubtitles.org/en/search/sublanguageid-spa,spl): En este link ya esta preseleccionado que busque en español, sino lo tienen que seleccionar en lenguaje.
- [SubDL](https://subdl.com/): Acá busco subtitulos de temporadas completas.

Recomiendo descargar subtitulos con el nombre parecidos a tu torrent.

### Usar subtitulos descargados

Generalmente los subtitulos vienen en un zip, recomiendo mover solo el archivo `.srt` o `.ass` al mismo directorio de la película o serie. 

Luego en VLC al medio haces click derecho, subtitulos, add subtitle file y le das click a tu `.srt` descargado.

### Ajustes en VLC

A veces los subtitulos están de-sincronizados, pueden estar adelantados o atrasados. Esto es fácil de solucionar con las teclas `g` y `h`. Generalmente están de-sincronizados por segundos, recomiendo probar con saltos de 1000ms.

Una vez lo sincronizas al principio del video recomiendo ir al final y ver si siguen sincronizados, si no  están sincronizados gg. Vas a tener que probar con otro subtitulo.
