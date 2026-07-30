# RunaShared Releases

![RunaShared Tkinter GUI](https://raw.githubusercontent.com/Jirolk/RunaShared-Releases/master/screenshots/gui.png)
![RunaShared Web Login](https://raw.githubusercontent.com/Jirolk/RunaShared-Releases/master/screenshots/web-gui-login.png)
![RunaShared Web UI](https://raw.githubusercontent.com/Jirolk/RunaShared-Releases/master/screenshots/web-gui.png)

Binarios públicos de **RunaShared** para descarga directa.

---

## ¿Qué es RunaShared?

**RunaShared** convierte cualquier carpeta local en un servidor de archivos accesible desde **cualquier dispositivo en la red local** (Wi-Fi / LAN). Ideal para compartir archivos entre PC, móvil, tablet, Smart TV, etc., sin subir nada a la nube.

### Características principales

| Función                      | Descripción                                                                                                   |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Acceso Web (HTTP)**        | Panel responsive en el navegador: sube, descarga, renombra, elimina, crea carpetas, vista previa de imágenes. |
| **Acceso SMB (Red Windows)** | La carpeta aparece como unidad de red (`\\IP\RunaShared`) en el Explorador de archivos — copiar/pegar nativo. |
| **Autenticación**            | Usuario/contraseña (por defecto `admin` / `admin`, configurable).                                             |
| **Código QR**                | Escanea con el móvil y abre el panel web al instante.                                                         |
| **Puerto por defecto**       | `8000` (HTTP). SMB usa el puerto `445`.                                                                       |
| **Multiplataforma**          | Windows y Linux (binario único, sin dependencias externas).                                                   |
| **Firewall automático**      | En Windows abre el puerto 8000 al iniciar.                                                                    |

### Casos de uso típicos

- Pasar fotos/vídeos del móvil al PC sin cables.
- Compartir documentos entre portátiles en la misma Wi-Fi.
- Acceder a archivos del PC desde la TV (navegador o SMB).
- Servidor ligero temporal para transferencias puntuales.

---

## Descargas

### Windows

- [latest](https://github.com/Jirolk/RunaShared-Releases/releases/latest/download/RunaShared.exe) – `RunaShared.exe` (ejecutable portable, ~15 MB)

### Linux

- [latest](https://github.com/Jirolk/RunaShared-Releases/releases/latest/download/RunaShared) – `RunaShared` (binario ELF, ~18 MB)

Todas las versiones en: [Releases](https://github.com/Jirolk/RunaShared-Releases/releases)

---

## Instalación rápida

### Windows

1. Descarga `RunaShared.exe` de la versión deseada.
2. Doble clic → se abre la consola y la GUI.
3. En la pestaña **Inicio** verás las URLs HTTP y la ruta SMB.
4. Usuario: `admin` / Contraseña: `admin` (cambiar en pestaña **Config**).

### Linux

```bash
wget https://github.com/Jirolk/RunaShared-Releases/releases/latest/download/RunaShared
chmod +x RunaShared
./RunaShared
```

- Abre `http://<IP>:8000` en el navegador.
- SMB: `smb://<IP>/RunaShared` (GNOME/KDE) o `\\<IP>\RunaShared` (Windows).

---

## Requisitos de red

- Ambos dispositivos en la **misma red local** (misma Wi-Fi / mismo router).
- Perfil de red en **Privada** (Windows) para que SMB funcione.
- Puerto **8000** TCP libre (HTTP) y **445** TCP (SMB).

---

## Licencia y Modelo

**Binarios:** Gratis para uso personal y comercial. Ver [LICENSE-BINARY.txt](LICENSE-BINARY.txt)

**Código fuente:** Privado. No es open source.

**Futuro:** Las versiones 2.0+ podrán incluir publicidad opcional en la interfaz web para sostener el desarrollo. La versión 1.x permanecerá sin publicidad.

¿Soporte comercial / licencia sin ads / personalización? Contacto: [tu-email@dominio.com]
