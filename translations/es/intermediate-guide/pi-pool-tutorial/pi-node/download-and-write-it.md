---
description: Flash image
---

# Descargar y Flashear

## Flashea la imagen

Descarga, instala y abre [ Raspberry pi Imager ](https://github.com/raspberrypi/rpi-imager/releases/latest). Conecte su unidad USB de destino.

{% tabs %}
{% tab title="Local Machine (Ubuntu)" %}
```bash
# Ubuntu users can download and install with snapd
sudo apt update
sudo apt install snapd
sudo snap install rpi-imager
```
{% endtab %}
{% endtabs %}

{% hint style="danger" %}
Los modelos más antiguos del Pi4B 8GB necesitan tener su cargador de arranque (boot loader) actualizado para arrancar desde un USB. Si tu imagen no arranca, retire la unidad USB3 y usa rpi-imager para flashear el recovery de arranque Pi 4 EEPROM a una tarjeta SD.

Conecta el Pi a un monitor, inserta la tarjeta SD y enciéndela. Una vez que vea una pantalla verde sería buen momento para arrancar desde tu unidad USB3. Las versiones más recientes vienen con un cargador de arranque compatible con USB. **Feeling lucky?**

**Choose OS -> Misc utility images -> Raspberry Pi 4 EEPROM boot recovery** [https://www.raspberrypi.org/documentation/hardware/raspberrypi/booteeprom.md](https://www.raspberrypi.org/documentation/hardware/raspberrypi/booteeprom.md)
{% endhint %}

![](../../../../.gitbook/assets/otgpoltut (1) (1) (3) (3).png)

{% tabs %}
{% tab title="Pre configured Pi-Node.img.gz" %}
### Obtén el archivo Pi-Pool .img.gz

<<<<<<< HEAD
| [Pi-Node](https://db.adamantium.online/Pi-Node.img.gz) |
| ------------------------------------------------------ |
=======
| [Pi-Node](https://mainnet.adamantium.online/Pi-Node.img.gz) |
|:------------------------------------------------------ |
>>>>>>> master
|                                                        |

### Dentro de Raspberry Pi Imager

**Choose OS -> Use custom**

Localiza el archivo .img.gz que descargaste & y flashealo.

Localiza tu unidad de destino & y grábala al disco.

![](../../../.gitbook/assets/custom_os.png)
{% endtab %}

{% tab title="Fresh Ubuntu 21.04 installation" %}
### Dentro de Raspberry Pi Imager

### Select  Ubuntu Server 21.04 (RPI 3/4/400)

**Choose OS -> Other general purpose OS -> Ubuntu -> Ubuntu Server 21.04 (RPI 3/4/400)**. Opción de servidor de 64 bits.

Localiza tu unidad de destino & y grábala al disco.

![](../../../../.gitbook/assets/21.04-rpi-imager.png)
{% endtab %}
{% endtabs %}
