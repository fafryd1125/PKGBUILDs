Installation
------------

```
Current release

                                                     [N] ->- mesa-glvnd -> [3]

                                                   /
  GLVND [1]/[2] --->--- nvidia --->--- GLVND [1]/[2]
                                               \
                                                ->- nvidia-libgl

[1] libglvnd-git
[2] libglvnd-mesa-git
[3] bumblebee
[N] not tested

------------------------------------------------------------------------------

Legacy releases for GeForce 8 and 9 series GPUs


 nvidia-340xx --->--- [*] nvidia-340xx-libgl --> [v2]/[N][v3]
    \
     \
      [N][v1] -->-- GLVND [1] -->-- mesa-glvnd --> [2]
       \
        \
         [v2] -->-- mesa --> [2]

[1]  libglvnd-mesa-git
[2]  bumblebee
[*]  GLVND isn't supported
[N]  not tested

[v1] version: glvnd Mesa
[v2] version: mesa (non-GLVND)
[v3] version: mesa-glvnd (without mesa-glvnd-libgl)
```

See also
--------

* [Andy Ritger - libglvnd Status Update](https://www.youtube.com/watch?v=4PflCyiULO4&feature=youtu.be&t=10156)
* [glvnd Status Report](https://www.x.org/wiki/Events/XDC2016/Program/xdc-2016-glvnd-status.pdf)
* [Add support for libglvnd](https://bugs.freedesktop.org/show_bug.cgi?id=92877)