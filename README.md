# sofa_cell_micromanipulation
this is a simulation scene for robotic cell micromanipulation




## 1.build sofa platform
In this link [build sofa](https://sofa-framework.github.io/doc/getting-started/build/linux/), you may find useful steps.
And my environment is V23.12.00 in sofa Ubuntu 22.04.4 LTS

## 2.build geomagic plugin with sofa
In this link [build plugin](https://sofa-framework.github.io/doc/getting-started/build/linux/](https://www.sofa-framework.org/community/doc/plugins/build-a-plugin-from-sources/#in-tree-build)), you may find useful steps.
Make sure that you build plugin by in-tree-build with sofa.

## 3.install Touch Driver and Software
Driver and Software files are in [Driver and Software](https://github.com/nc-yc/sofa_cell_micromanipulation/tree/main/src)

## 4.Run commands

```bash
ls -l /dev/ttyACM*
# if you connect the Touch, it will show like:
# crw-rw---- 1 root dialout 166, 0 12月  4 21:42 /dev/ttyACM0
sudo chmod 777 /dev/ttyACM0
cd ~/sofa/build/bin
sudo ./runSofa
```
