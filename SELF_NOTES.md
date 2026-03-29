Clique layer issue debugging

Seems the issue was that flashing will try to preserve changes made in clique
and in this instance this blocked the Mod layer key, which is needed to put it
in studio/clique mode.

For some reason, flashing the reset file did not clear this.
Instead, had to flash the default image, go to clique, and choose 'restore
default layout', then flash the customized image again.

