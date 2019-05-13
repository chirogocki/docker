# Single Board Computing
![Asus Tinker Board S](../pictures/asus-tinker-logo.png)

New docker swarm with 8 [Asus Tinker Board S](https://www.asus.com/us/Single-Board-Computer/Tinker-Board-S/)  
  
## Hardware
  
### Specification
  
| Type | Values |
|----------|:---------:|
| SBC | Asus Tinker Board S |
| Cpu | Rockchip Quad-Core RK3288 processor |
| Ram | 2Go Dual Channel DDR3 |
| eMMC | 16Go |
| Ethernet | 1x1Gb |
  
### Case
  
Cases printed with [Neva Magis](https://dagoma.fr/neva-magis.html) by Dagoma, original design find on [Thingiverse](https://www.thingiverse.com/thing:3352189)  
  
Some pictures of my project :  

![slim-case](../pictures/SBC/hardware/slim-case.png)
![slim-case-2](../pictures/SBC/hardware/slim-case-2.png)
![stack](../pictures/SBC/hardware/stack.png)
![stack-front](../pictures/SBC/hardware/stack-front.png)
![running-single](../pictures/SBC/hardware/running-single.png)
![running](../pictures/SBC/hardware/running.png)
  
## OS
  
Using [DietPi](https://dietpi.com/) OS cause it's fully optimized according to this hardware.  
  
Considering low storage support for these SBC, mounted shares are used. Here is why I choose NFS :  
  
![benchmark](../pictures/SBC/benchmark.png)