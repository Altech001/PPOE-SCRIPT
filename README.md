# PPOE-SCRIPT
MERITE

================= PPOE SCRIPT .RSC =============================
Upload and run via Winbox:

Go to Files → upload the .rsc file
Open Terminal and run:

bash/import altech-mikrotik-setup.rsc
Or paste directly into terminal — copy the whole file and paste it line by line.

One important note: The PPPoE client on ether1-ISP is set with user=altech / password=altech — but that's your internal user. If your real ISP gives you different credentials for ether1 upstream, edit line 8 of the script with those real ISP credentials before running it. Right now your ether1 is getting IP 192.168.1.2 via DHCP from the ISP, so you may not even need the pppoe-out1 client at all.
