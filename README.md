These are my xkb configs that I believe might be useful to other people

Among layouts that are not avalible in standard xkb it has Diktor, Rulemak _(it is in standard xkb but is missing from some evdev.xml configs that are on part of the OS)_ and powerful [Extend](https://dreymar.colemak.org/layers-extend.html) layers for them (and Colemak).

![image](https://github.com/carbon-starlight/xkb-configurations/assets/145182032/6ce7556a-ff93-44c6-8720-bc7a41511a27)

You can install these configurations with the following command:

```
TMP_DIR=$(mktemp -d) && sudo rm -rf /usr/share/X11/xkb && git clone https://github.com/carbon-starlight/xkb-configurations.git $TMP_DIR && sudo mv $TMP_DIR/xkb /usr/share/X11/ && rm -rf $TMP_DIR
```

This line will overwrite the whole xkb cataloge (unless you installed 3-rd party keyboard layouts it shouldn't contain any personal configurations). This installation doesn't touch anything but the `usr/share/X11/xkb` catalouge (folder). If something goes wrong, just replace this catalouge with the default one for your distribution.
