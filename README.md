Installation
------------

```
Current release


 nvidia -->-- GLVND [1]->- nvidia-drivers ->- mesa-glvnd -> [2]


[1] libglvnd-git
[2] bumblebee

------------------------------------------------------------------------------

Legacy releases for GeForce 8 and 9 series GPUs


 nvidia-340xx --->--- [*] nvidia-340xx-libgl --> [v2]
    \
     \
      [v1] -->-- GLVND [1] -->-- mesa-glvnd --> [2]


[1]  libglvnd-git
[2]  bumblebee
[*]  GLVND isn't supported

[v1] version: glvnd Mesa
[v2] version: mesa (without mesa-glvnd package)
```

See also
--------

* [Andy Ritger - libglvnd Status Update](https://www.youtube.com/watch?v=4PflCyiULO4&feature=youtu.be&t=10156)
* [glvnd Status Report](https://www.x.org/wiki/Events/XDC2016/Program/xdc-2016-glvnd-status.pdf)
* [Add support for libglvnd](https://bugs.freedesktop.org/show_bug.cgi?id=92877)