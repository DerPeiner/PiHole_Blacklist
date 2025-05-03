###############################################################################
#.         I created that list because of a lot of NOT IN OTHER Lists
#.         Use the List as you like
#.
#.        First Creation:  2024-06-09
#.        Last Update:    2024-06-23
###############################################################################

#. Links to the Blacklists i use

#. My personal Blacklist with Domains my Firewall had dedected
linkadvdirect.com
yy.puffexles.com
holahupa.com
disclosestockingsprestigious.com
a.adforcast.com
citadelpathstatue.com
filter.realtime-bid.com
blo.booseed.com
yd.cottoidearldom.com
bid.bidclickmedia.com
allvideometrika.com
rougepromisedtenderly.com
cobalten.com
alphaads.de
hoproutepoint.cc
lorlwithinfamlly.com
thoohlzoogll.xyz
ofleafeona.com
a.adforcast.com
green-resultsbid.com
ak.hetapus.com
giersakr.com
gobck.com
creative.mnaspm.com
chaturbate.com
merkurbets.de
play-lustgoddess.com
etoro.com
ey43.com





#. List of different Blacklists i use



#. Welche Einträge findet man hier?
#.
#. Auf der RegEx-Seite finden sich nur die Sperr-Einträge, welche über die normale Blocklist nur schwer zu blockieren wären.
#. Es ist einfacher alle Domains der TLD .porn über RegEx zu sperren, als die 14.000 einzelnen Domains zu sperren. 
#. Das gleiche für die hier aufgeführten ccTLDs.
#.
#. Ein weiterer Anwendungsfall:
#. Wenn Nutzer - aus Gründen des Jugendschutzes - den Zugang zu Facebook oder anderen sozialen Netzwerk verhindern wollen, 
#. ist es einfacher die Hauptdomain über RegEx zu sperren.
#.
#. Alle anderen Sperrungen werden (zumindest in Pihole 4) über die klassische Blocklist realisiert.
#.

#. "WPAD-Lücke": WPAD Protokoll im Netzwerk verbieten:
^wpad\.
#. Kann aber Probleme mit VPN-Sofware verursachen, z.B.: Cisco AnyConnect Secure Mobility Client.

#. Einträge für Spam- und Malware-Schutz:

#. Sperrt alle Domains aus China, Russland, Sowjetunion, Kolumbien, Vietnam sowie die .top-TLD, aus der scheinbar nur Spammails kommen:
(\.cn$|\.ru$|\.su$|\.co$|\.vn$|\.top$)

#. Sperrt alle Domains aus China, Russland, Sowjetunion, Vietnam sowie die .top-TLD, aus der scheinbar nur Spammails kommen:
(\.cn$|\.ru$|\.su$|\.vn$|\.top$)
#. Gleiche Zeile wie oben, nur ohne "Kolumbien", da der Twitter-Linkverkürzer und Spotify einige .co Domains nutzen.

#. Sperrt alle Domains der TLD .link: (Linkverkürzer)
\.link$

#. Sperrt alle Domains der TLD .zip:
\.zip$

#. Sperrt Suchmaschinen-Schrott Domains:
(softonic\.com$|uptodown\.com$|malavida\.com$)

#. Sperrt alle URLs zu "sendgrid.net"
sendgrid\.net$

#. Sperrt alle Punycode-Domains:
.*(xn--).*

#. Sperrt alle URLS zu "duckdns.org"
duckdns\.org$

#. Einträge für Jugendschutz:

#. Sperrt alle Domains verschiedener TLDs (Jugendschutz):
#(\.porn$|\.sex$|\.xxx$|\.sexy$|\.webcam$|\.cam$|\.tube$|\.adult$|\.gay$)

#. Sperrt alle Domains verschiedener TLDs (Jugendschutz):
(\.casino$|\.bet$|\.poker$)

#. Sperrt alle Domains in Zusammenhang mit Instagram:
instagram

#. Sperrt alle Domains in Zusammenhang mit Facebook:
facebook

#. Sperrt Telemetrie-Endpunkte für Windows:
watson\..*\.microsoft\.com
