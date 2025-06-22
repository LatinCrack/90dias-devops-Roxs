# 📅 Semana 01 - Linux, Vagrant y Ansible

## 🎯 Objetivo de la Semana
Familiarizarte con el sistema operativo Linux, automatizar tareas básicas con scripts Bash, levantar entornos virtuales con Vagrant y aplicar tus primeros playbooks con Ansible.

---

## 📘 Teoría

### 🐧 Fundamentos de Linux
- **¿Qué es Linux? ¿Por qué es esencial en DevOps?**
  - 🎥 [Linux para principiantes - freeCodeCamp (min 0:00 - 10:00)](https://www.youtube.com/watch?v=IVquJh3DXUA)
  - ✅ *Práctica:* Explica en una nota qué es un sistema operativo y qué ventajas ofrece Linux en entornos DevOps.

- **Estructura de directorios: `/home`, `/etc`, `/var`, `/usr`, `/bin`**
  - 🎥 [Linux Directory Structure Explained - LearnLinuxTV](https://www.youtube.com/watch?v=42iQKuQodW4)
  - ✅ *Práctica:* Usa `tree /` o `ls -l /` y haz una tabla explicando 5 directorios con su propósito.

- **Permisos y propietarios (`chmod`, `chown`, `ls -l`)**
  - 🎥 [Permisos de Archivos y chmod en Linux - Fazt](https://www.youtube.com/watch?v=6tNS--WetLI)
  - ✅ *Práctica:* Crea un archivo, cambia sus permisos y dueño, luego explica cada cambio.

- **Comandos básicos: `cd`, `ls`, `pwd`, `mkdir`, `cp`, `mv`, `rm`, `cat`, `nano`, `top`, `ps`**
  - 🎥 [Comandos básicos en Linux - Píldoras Informáticas](https://www.youtube.com/watch?v=k3j3LQzDRNE)
  - ✅ *Práctica:* Crea un “diario de comandos” donde uses al menos 10 comandos para organizar archivos en tu terminal.

- **Variables de entorno (`$PATH`, `$HOME`)**
  - 🎥 [Variables de entorno en Linux - Sysadmin Academy](https://www.youtube.com/watch?v=9swdaJqEMVA)
  - ✅ *Práctica:* Imprime tus variables con `echo $PATH` y crea una variable temporal personalizada.

- **Pipes y redirecciones (`|`, `>`, `>>`, `<`)**
  - 🎥 [Redirección y pipes en Linux - Victor Robles](https://www.youtube.com/watch?v=kB_hsL6i5Ao)
  - ✅ *Práctica:* Combina comandos con pipes y guarda el resultado en un archivo. Ej: `ps aux | grep ssh > procesos.txt`

### 💻 Bash Scripting Básico
- **`#!/bin/bash`, variables, condicionales (`if`, `else`), bucles (`for`, `while`)**
  - 🎥 [Curso de Bash Shell Script desde cero (Fazt)](https://www.youtube.com/watch?v=3Kq1MIfTWCE)
  - ✅ *Práctica:* Crea un script que recorra una lista de nombres y los imprima con un saludo personalizado.

- **Crear scripts ejecutables (`chmod +x script.sh`)**
  - 📄 Explicado también en [linuxcommand.org](https://linuxcommand.org/lc3_lts0050.php)
  - ✅ *Práctica:* Haz un script que cree 5 carpetas y escriba un archivo `.txt` dentro de cada una.

### 📦 Vagrant
- **¿Qué es Vagrant?**
  - 🎥 [Curso completo de Vagrant (HolaMundo)](https://www.youtube.com/watch?v=iG5A8Erg9Zc)
  - ✅ *Práctica:* Explica en tus palabras qué problema resuelve Vagrant en equipos DevOps.

- **Inicializar VM: `vagrant init ubuntu/bionic64`**
- **Levantar VM: `vagrant up`**
- **Acceder: `vagrant ssh`**
- **Destruir VM: `vagrant destroy`**
  - ✅ *Práctica:* Crea una VM, accede por SSH, instala `htop`, y luego destrúyela.

### 🤖 Ansible
- **¿Qué es Ansible y por qué se usa?**
  - 🎥 [Ansible para principiantes (Bitácora de Codelandia)](https://www.youtube.com/watch?v=XIV-lT7zJZ4)
  - ✅ *Práctica:* Resume los beneficios de usar Ansible en comparación con scripts manuales.

- **Inventario, módulos, YAML y Playbooks**
- **Ejecutar un comando remoto: `ansible all -i inventario -m ping`**
- **Estructura de un playbook básico**
  - ✅ *Práctica:* Crea un playbook que instale `htop` en una máquina remota y verifícalo con `ansible -m shell -a "htop --version"`

---

## 🧪 Ejercicios

1. Instalar una distro Linux (Ubuntu recomendado, VM o WSL si estás en Windows).
2. Crear una estructura de carpetas y archivos, luego automatizarlo con un script.
3. Instalar Vagrant y VirtualBox.
4. Levantar una máquina virtual Ubuntu con Vagrant.
5. Acceder a la VM y cambiar el hostname.
6. Crear un archivo de inventario para Ansible.
7. Ejecutar un playbook que instale `nginx` y cree un archivo de bienvenida en `/var/www/html`.

---

## 🛠 Proyecto: "Castillo DevOps".

**Objetivo:** Levantar dos máquinas virtuales usando Vagrant, y configurarlas automáticamente con Ansible.

### Estructura esperada:
```
castillo-devops/
├── Vagrantfile
├── inventario
├── playbook.yml
└── roles/
    └── webserver/
        ├── tasks/main.yml
        └── files/index.html
```
### Requisitos del proyecto:
- 2 VMs: una llamada `torre` y otra `muralla`
- En ambas instalar `nginx` con Ansible
- Crear una página HTML personalizada para cada una

---

## 🎯 Mini-Quiz (respuestas al final del archivo)

1. ¿Qué comando muestra los procesos en ejecución en Linux?  
   a) `ps`  
   b) `ls`  
   c) `top`  

2. ¿Qué hace `chmod +x script.sh`?  
   a) Borra el archivo  
   b) Lo hace ejecutable  
   c) Lo copia a otra carpeta  

3. ¿Cuál es la función principal de Vagrant?  
   a) Crear contenedores Docker  
   b) Automatizar flujos CI/CD  
   c) Gestionar máquinas virtuales  

4. ¿Qué extensión tienen los archivos de playbooks en Ansible?  
   a) `.json`  
   b) `.xml`  
   c) `.yml`  

5. ¿Qué comando usas para iniciar una VM con Vagrant?  
   a) `vagrant ssh`  
   b) `vagrant destroy`  
   c) `vagrant up`  

---

## 📺 Recursos Gratuitos

### Videos
- [Linux para principiantes (freeCodeCamp)](https://www.youtube.com/watch?v=IVquJh3DXUA)
- [Curso de Bash Shell Script desde cero (Fazt)](https://www.youtube.com/watch?v=3Kq1MIfTWCE)
- [Curso de Vagrant (HolaMundo)](https://www.youtube.com/watch?v=iG5A8Erg9Zc)
- [Ansible para principiantes (Bitácora de Codelandia)](https://www.youtube.com/watch?v=XIV-lT7zJZ4)

### Documentación
- https://linuxcommand.org/
- https://developer.hashicorp.com/vagrant/docs
- https://docs.ansible.com/

---

## ✅ Respuestas del Mini-Quiz
1. ✅ c) `top`  
2. ✅ b) Lo hace ejecutable  
3. ✅ c) Gestionar máquinas virtuales  
4. ✅ c) `.yml`  
5. ✅ c) `vagrant up`

