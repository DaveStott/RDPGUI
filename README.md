Simple Remote Desktop Connection Client in PyQt4<br>
<br>
Forked from Gibbio's RDPGUI: https://github.com/Gibbio/RDPGUI<br>
More info can be found at: http://rpitc.blogspot.co.uk/2013/09/freerdprdesktop-gui-client.html<br>
<br>
Package needed:<br>
python-qt4<br>
<br>
edit rdpgui.ini to fit your server environment<br>
<br>
config for FreeRDP > 1.0.1 (new command line release: https://github.com/FreeRDP/FreeRDP/wiki/CommandLineInterface):<br>
[DEFAULT]<br>
RDPBinary = xfreerdp<br>
RDPDomain = defaultdomain<br>
RDPServer = <br>
RDPDomainFlags = /d:<br>
RDPServerFlags = /v:<br>
RDPUserFlags = /u:<br>
RDPPasswordFlags = /p:<br>
RDPDefaulfFlags = /cert-ignore /f<br>
RDPExtraFlags = /sound:sys:pulse /rfx /fonts<br>
<br>
config for FreeRDP < 1.0.1 (old command line release: http://manpages.ubuntu.com/manpages/raring/man1/xfreerdp.1.html):<br>
[DEFAULT]<br>
RDPBinary = xfreerdp<br>
RDPDomain = defaultdomain<br>
RDPServer = <br>
RDPDomainFlags = "-d "<br>
RDPServerFlags = ""<br>
RDPUserFlags = "-u "<br>
RDPPasswordFlags = "-p "<br>
RDPDefaulfFlags = "-x l -f"<br>
RDPExtraFlags = "--plugin rdpsnd -z --rfx"<br>
<br>
config for RDesktop (command line reference: http://manpages.ubuntu.com/manpages/raring/man1/rdesktop.1.html):<br>
[DEFAULT]<br>
RDPBinary = rdesktop<br>
RDPDomain = defaultdomain<br>
RDPServer = <br>
RDPDomainFlags = "-d "<br>
RDPServerFlags = ""<br>
RDPUserFlags = "-u "<br>
RDPPasswordFlags = "-p "<br>
RDPDefaulfFlags = "-x l -f"<br>
RDPExtraFlags = "-r sound:local:alsa -z"<br>
