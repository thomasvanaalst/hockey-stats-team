# Teampagina

Eén bestand: `docs/index.html`. Daar staat de data in als versleutelde tekst.

De pagina vraagt om een wachtwoord, leidt daar met PBKDF2-SHA256 (310.000
iteraties, willekeurig salt) een sleutel uit af en ontsleutelt met AES-GCM-256
via WebCrypto, in je eigen browser. Er gaat niets over het netwerk.

Het wachtwoord staat **niet** in deze repo en komt er ook nooit in. Zonder dat
wachtwoord valt er uit dit bestand niets te halen — het is geen scherm dat iets
verbergt, de data is echt versleuteld.

De bron, de data en de bouwstap staan in een aparte, privé repo.
