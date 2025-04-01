In this directory are patches for [snircd](https://github.com/quakenet/snircd).<br>
Following patches are available:<br>
webirc-tls.diff - Fixed MAXCONNECTIONS issue, adds the WEBIRC function, CAPs (e.g. SASL auth over iauthd) and an experimental TLS support.<br>
<br>
To install this patch, you need a not modified fresh installation of [snircd](https://github.com/quakenet/snircd) and do following steps:<br>
Go into your snircd directory and enter "wget https://raw.githubusercontent.com/WarPigs1602/snircd-patches/refs/heads/main/webirc-tls.diff"<br>
Then enter "git apply webirc-tls.diff", "./configure", "make" and "make install"<br>
<br>
And the ircd will work.<br>
<br>
Have fun with the patches.<br>

