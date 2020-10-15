# PyconAR 2020 

## Como desarrollar un switch de capa 2 sobre un controlador SDN con Ryu framework
![Python](https://img.shields.io/badge/OpenFlow-v1.3-orange)
![Python](https://img.shields.io/badge/mininet-v2.2.2-orange)
![Python](https://img.shields.io/badge/ovs-v2.13.0-orange)
![Python](https://img.shields.io/badge/ryuframework-4.34-blue)
![Python](https://img.shields.io/badge/python-v3.6-blue)
![Python](https://img.shields.io/badge/platform-linux--64-lightgrey)

**Abstract:**
Las redes definidas por software (SDN) vienen a cambiar la forma en la que pensamos como las aplicaciones se vinculan con las redes sobre las que funcionan. En esta charla intentaré dar una breve introducción a la arquitectura y protocolos propuestos por SDN y como desarrollar nuevas funcionalidades de red usando un framework/controlador hecho en Python.

**Descripción:**
El objetivo de la charla es abordar los conceptos básicos de las redes definidas por software utilizando openflow como southbound interface y Open Virtual Switch (ovs) como elemento de red programable. Como ejemplo práctico, utilzaremos un framework para el desarrollo de aplicaciones SDN hecho en Python (Ryu) y veremos como desarrollar aplicaciones que implementen funcionalidades nuevas sobre nuestra red.

**Tabla de contenido**

- [Empezando](#empezando)
- [Ejemplos](#ejemplos)
    - [Switch L2](#switch-l2)
    - [Calidad de servicio](#calidad-de-servicio)
- [Referencias](#referencias)

### Requerimientos
Además de los requerimientos del repositorio, será necesario contar mininet.

### Comenzando
Clonar repositorio y (opcional) crear un virtualenv+virtualenvwrapper python para el manejo de dependencias

```bash
$ git clone https://github.com/joagonzalez/pyconar-2020
$ mkproject pyconar-2020
$ workon pyconar-2020
$ pip install -r requirements.txt
```

**Instalar Ryu**
```baskh
git clone https://github.com/faucetsdn/ryu.git
cd ryu; pip install .
```

**Instalar Mininet**
```bash
git clone git://github.com/mininet/mininet
cd mininet
git tag  # list available versions
git checkout -b 2.2.2
cd ..
mininet/util/install.sh [options]
```

### Ejemplos

#### Switch L2
Inicializar controlador
Inicializar Mininet/GNS3

#### Calidad de servicio
Inicializar controlador
Inicializar script
![Figura 2](doc/pyconar-qos.png)

### Referencias
- http://mininet.org/
- https://ryu-sdn.org/
- https://github.com/faucetsdn/ryu
- https://www.opennetworking.org/
- https://iperf.fr/ 


