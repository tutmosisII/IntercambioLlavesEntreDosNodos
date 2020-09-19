# IntercambioLlavesEntreDosNodos

Este repositorio describe el proceso de intercambio de llaves entre dos nodos (usando Vagrant) y entre la misma máquina de manera circular. Como se describe en el siguiente diagrama.

Que necesitamos para el ejemplo:

1) Vagrant Instalado
2) Hyper-V corriendo y habilitado en Windows10
3) Un switch creado en Hyper-V para ser usado en las instancias.

**Nota**: Puedes encontar infromación de como crear los switch en: [Minikube con Hyper-V en Windows10](https://medium.com/@alejandroleon09/minikube-con-hyper-v-en-windows10-2f3fae956c3b)

![Diagrama Despliegue](media/despliegueDiagrama.png)

## Instancia de Dos Nodos con [Vagrant](https://www.vagrantup.com/).

Acorde con el diagrama de trabajo necesitamos crear dos instacias lo cual se hace el archivo [Vagrantfile](Vagrantfile).

El projecto hace ulto de la configuración [multimáquina](https://www.vagrantup.com/docs/multi-machine)

Para levantar las dos máquinas virtuales necesitas enjecutar en una linea de comandos de administrador lo siguiente:

```powershell
vagrant up
```

La descarga inicial de la imagen [**bento/ubuntu-20.04**](https://app.vagrantup.com/boxes/search?provider=hyperv&q=20.04&sort=downloads&utf8=%E2%9C%93) tomará algún tiempo antes de iniciar los nodos virtuales. Más información de esta imagen la puedes enctra en la nuve de vagrant al filtrar por 20.04 y hyperv.

![SearchBox](media/VagranUbuntu2004_hyperv.png)

## Plugins usados en VSCode.

[![Drawio Integration](media/drawio_integration.png)](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)

ext install hediet.vscode-drawio
