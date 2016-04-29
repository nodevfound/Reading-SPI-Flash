# Reading-SPI-Flash
Reference: http://hardware371.rssing.com/chan-9066388/latest.php

<h3>The Setup</h3>
<img src="https://ao2.it/sites/default/files/blog/2012/09/23/tumpa/tumpa-mx25l8005.png"> <br>
<img src="https://ao2.it/sites/default/files/imagecache/scaled-250px/blog/2012/09/23/tumpa/tumpa-mx25l8005-photo.jpg">

<h3>Results</h3>
$ sudo flashrom -p ft2232_spi:type=tumpa,port=B -r flash.bin<br>
<p>
<i>flashrom v0.9.6.1-r1563 on Linux 3.6.0-rc5-ao2 (x86_64)<br>
flashrom is free software, get the source code at http://www.flashrom.org<br>
Calibrating delay loop... OK.<br>
Found Macronix flash chip "MX25L8005" (1024 kB, SPI) on ft2232_spi.<br>
Reading flash... done.<br>
</i>
</P>

<b>Note: Must connect to SPI2 of the TIAO USB board because the command use "port=B"<br>
\#WP and \#HOLD pins are not connected to dump the SPI flash (WindBond Chip Series: W25X20)
</b>

