Claro, aquí tienes el contenido reformulado y con la tabla de subred completa incluida:  

---

# 🖧 NetTraining  

## 🌟 Introducción  
NetTraining es una herramienta interactiva diseñada para que practiques y entiendas conceptos esenciales de redes informáticas. A través de 10 niveles progresivos, podrás mejorar tus habilidades configurando IPs, subredes y otros elementos clave de redes.  

## 📌 ¿Cómo funciona?  
1. Completa los campos necesarios en cada nivel.  
2. Haz clic en `Comprobar configuración` para verificar si es correcta.  
3. Si completas un nivel con éxito, descarga tu configuración usando el botón `Obtener configuración`.  
4. Avanza al siguiente nivel con el botón `Siguiente nivel`.  
5. Accede a la herramienta [aquí](https://ricardoreves.github.io/42-net-practice/).  

## 🌍 Conceptos básicos de redes  

### 📋 Dirección IP  
Una dirección IP identifica de forma única un dispositivo en una red. En el caso de IPv4, consiste en 32 bits divididos en cuatro octetos (por ejemplo, `192.168.0.1`).  
- **Red:** Determina a qué segmento de red pertenece la dirección.  
- **Host:** Especifica el dispositivo dentro de esa red.  

> **Analogía:** Es como una dirección postal, donde la red es el nombre de la calle y el host, el número de casa.  

### 🧩 Máscara de subred  
La máscara de subred es un número de 32 bits que separa los bits dedicados a la red de los asignados a los hosts dentro de ella.  
- Las direcciones terminadas en `255` se utilizan para broadcasts.  
- Las direcciones terminadas en `0` identifican la red.  

#### Ejemplo práctico:  
```
Dirección:  192.168.1.10  
Máscara:    255.255.255.0  
Red:        192.168.1.0  
Broadcast:  192.168.1.255  
Rango útil: 192.168.1.1 - 192.168.1.254  
```  

### 🗂️ Tabla de máscaras de subred  
Esta tabla te será útil para calcular redes y subredes.  

| Máscara de subred | CIDR | Notación binaria                  | Bits de red | Bits de host | Direcciones disponibles |  
|-------------------|------|-----------------------------------|-------------|--------------|--------------------------|  
| 255.255.255.255   | /32  | 11111111.11111111.11111111.11111111 | 32          | 0            | 1                        |  
| 255.255.255.254   | /31  | 11111111.11111111.11111111.11111110 | 31          | 1            | 2                        |  
| 255.255.255.252   | /30  | 11111111.11111111.11111111.11111100 | 30          | 2            | 4                        |  
| 255.255.255.248   | /29  | 11111111.11111111.11111111.11111000 | 29          | 3            | 8                        |  
| 255.255.255.240   | /28  | 11111111.11111111.11111111.11110000 | 28          | 4            | 16                       |  
| 255.255.255.224   | /27  | 11111111.11111111.11111111.11100000 | 27          | 5            | 32                       |  
| 255.255.255.192   | /26  | 11111111.11111111.11111111.11000000 | 26          | 6            | 64                       |  
| 255.255.255.128   | /25  | 11111111.11111111.11111111.10000000 | 25          | 7            | 128                      |  
| 255.255.255.0     | /24  | 11111111.11111111.11111111.00000000 | 24          | 8            | 256                      |  
| 255.255.254.0     | /23  | 11111111.11111111.11111110.00000000 | 23          | 9            | 512                      |  
| 255.255.252.0     | /22  | 11111111.11111111.11111100.00000000 | 22          | 10           | 1024                     |  
| 255.255.248.0     | /21  | 11111111.11111111.11111000.00000000 | 21          | 11           | 2048                     |  
| 255.255.240.0     | /20  | 11111111.11111111.11110000.00000000 | 20          | 12           | 4096                     |  
| 255.255.224.0     | /19  | 11111111.11111111.11100000.00000000 | 19          | 13           | 8192                     |  
| 255.255.192.0     | /18  | 11111111.11111111.11000000.00000000 | 18          | 14           | 16384                    |  
| 255.255.128.0     | /17  | 11111111.11111111.10000000.00000000 | 17          | 15           | 32768                    |  
| 255.255.0.0       | /16  | 11111111.11111111.00000000.00000000 | 16          | 16           | 65536                    |  
| 255.254.0.0       | /15  | 11111111.11111110.00000000.00000000 | 15          | 17           | 131072                   |  
| 255.252.0.0       | /14  | 11111111.11111100.00000000.00000000 | 14          | 18           | 262144                   |  
| 255.248.0.0       | /13  | 11111111.11111000.00000000.00000000 | 13          | 19           | 524288                   |  
| 255.240.0.0       | /12  | 11111111.11110000.00000000.00000000 | 12          | 20           | 1048576                  |  
| 255.224.0.0       | /11  | 11111111.11100000.00000000.00000000 | 11          | 21           | 2097152                  |  
| 255.192.0.0       | /10  | 11111111.11000000.00000000.00000000 | 10          | 22           | 4194304                  |  
| 255.128.0.0       | /9   | 11111111.10000000.00000000.00000000 | 9           | 23           | 8388608                  |  
| 255.0.0.0         | /8   | 11111111.00000000.00000000.00000000 | 8           | 24           | 16777216                 |  

### 🔧 Herramientas recomendadas  
- [IP Calculator](https://jodies.de/ipcalc): Herramienta para calcular rangos de hosts, máscaras y configuraciones relacionadas con redes.  

## 📖 Recursos adicionales  
- [Guía de subredes para principiantes](https://www.packetcoders.io/a-beginners-guide-to-subnetting/)  
- [Máscaras de subred explicadas](https://avinetworks.com/glossary/subnet-mask/)  
- [Subnetting avanzado](https://softwaretestinghelp.com/subnet-mask-and-network-classes/)  

---
