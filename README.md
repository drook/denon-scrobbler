# denon-scrobbler


This is a simple perl application to scrobble from Denon networked receivers in a DLNA mode.
Tested and used on a Denon AVR-X1100W/FreeBSD 10.2-STABLE.

This scrobbler requres perl. And some obvious modules.

Change the following lines in the script:

my $denonaddress = "YOUR DENON UNIT IP ADDRESS";

my $username = "YOUR USERNAME";

my $password = "YOUR LAST.FM PASSWORD MD5 HASH HERE";


Usage: play some music on a Denon device, using it "Media Server" DLNA client,
for example I use foobar2000 player as a DLNA server. In the same time launch this
script on a machine that has a network connectivity with both Denon unit and a last.fm site.
You are supposed to see scrobbled tracks after some time (10 seconds).

The main reason for writing this was the fact that DLNA streaming gives more quality comparing 
to the LPCM playback. Obviously, no separate scrobbler is needed when playing directly from a
software player via HDMI/SOLINK.
