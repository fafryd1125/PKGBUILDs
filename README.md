Installation
-----------

```
Current release

                                                     [*] --- mesa-glvnd

                                                   /
  GLVND [1]/[2] --->--- nvidia --->--- GLVND [1]/[2]
                                               \
                                                --- nvidia-libgl

[1]  libglvnd-git
[2]  libglvnd-mesa-git
[*]  bumblebee

-----------------------------------------------------------------------

Legacy releases for GeForce 8 and 9 series GPUs


 [*] nvidia-340xx --->--- nvidia-340xx-libgl
        \
         \
          ---- mesa --->--- mesa-libgl


[*] GLVND isn't supported

```