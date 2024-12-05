# sofa_cell_micromanipulation
This is a simulation scene for robotic cell micromanipulation based on [Sofa](https://github.com/sofa-framework/sofa)
<img src="https://www.sofa-framework.org/wp-content/uploads/2013/01/SOFA_LOGO_ORANGE_2-normal.png" alt="SOFA, Simulation Open-Framework Architecture" width="100" height="auto">


<table align=center>

  <tr align=center>
    <td>
      <img src="./scene/1.gif" alt="First GIF" style="width: 100%;"/>
    </td>
    <td>
      <img src="./scene/2.gif" alt="3 GIF" style="width: 100%;"/>
    </td>
  </tr>


  <tr align=center>
    <td>
      demo1
    </td>
    <td>
      demo2
    </td>
  </tr>

</table>


### 1.build sofa platform
In this link [build sofa](https://sofa-framework.github.io/doc/getting-started/build/linux/), you may find useful steps.
And my environment is V23.12.00 in sofa Ubuntu 22.04.4 LTS

### 2.build geomagic plugin with sofa
In this link [build plugin](https://sofa-framework.github.io/doc/getting-started/build/linux/](https://www.sofa-framework.org/community/doc/plugins/build-a-plugin-from-sources/#in-tree-build)), you may find useful steps.
Make sure that you build plugin by in-tree-build with sofa.

### 3.install Touch Driver and Software
Driver and Software files are in [Driver and Software](https://github.com/nc-yc/sofa_cell_micromanipulation/tree/main/src)

### 4.Run commands

```bash
ls -l /dev/ttyACM*
# if you connect the Touch, it will show like:
# crw-rw---- 1 root dialout 166, 0 12月  4 21:42 /dev/ttyACM0
sudo chmod 777 /dev/ttyACM0
cd ~/sofa/build/bin
sudo ./runSofa
```


