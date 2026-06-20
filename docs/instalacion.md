# Instalación de Metasploit Framework

En esta sección se explica cómo instalar Metasploit Framework en los sistemas operativos más comunes.

## Requisitos del sistema

| Requisito         | Mínimo recomendado          |
|--------------------|------------------------------|
| Sistema operativo  | Linux (Kali, Ubuntu, Parrot) o Windows 10/11 |
| RAM                | 4 GB (8 GB recomendado)      |
| Espacio en disco   | 5 GB libres                  |
| Ruby               | Versión 3.0 o superior       |
| PostgreSQL         | Versión 12 o superior        |

!!! note "Nota"
    Kali Linux y Parrot ya incluye Metasploit Framework preinstalado, por lo que no es necesario seguir estos pasos si usas esa distribución.

## Pasos de instalación

A continuación, los comandos de instalación según tu sistema operativo:

=== "Linux (Debian/Ubuntu)"

```bash
    curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall
    chmod 755 msfinstall
    sudo ./msfinstall
```

=== "Windows (PowerShell)"

```powershell
    # Descargar el instalador desde el sitio oficial de Rapid7
    # https://windows.metasploit.com/metasploitframework-latest.msi

    # Ejecutar el instalador descargado
    .\metasploitframework-latest.msi
```

=== "macOS"

```bash
    brew install metasploit
```

!!! tip "Verificación de la instalación"
    Una vez instalado, verifica que todo funcione correctamente ejecutando el comando `msfconsole` en tu terminal. Si la instalación fue exitosa, se mostrará el banner de bienvenida de Metasploit junto con la versión instalada.

## Siguiente paso

Una vez instalado Metasploit, continúa con la sección de **Uso básico** para aprender los comandos esenciales de la consola.