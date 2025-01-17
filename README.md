In this directory are patches for [snircd](https://github.com/quakenet/snircd).<br>
Following patches are available:<br>
Updates-snircd-to-midircd.diff - Fixes IAuth crashes, fixes sethost issues (e.g. G-Line setted by server), added G-line for authed users, fixed MAXCONNECTIONS issue, adds the WEBIRC function from ircu to snircd and updates snircd to midircd<br>
<br>
To install this patch, you need a not modified fresh installation of snircd and do following steps:<br>
Go into your snircd directory and enter "wget https://raw.githubusercontent.com/WarPigs1602/snircd-patches/refs/heads/main/Updates-snircd-to-midircd.diff"<br>
Then enter "git apply Updates-snircd-to-midircd.diff", "./configure", "make" and "make install"<br>
<br>
And the ircd will work.<br>
<br>
Have fun with the patches.<br>

