# wazuh-unifi-decoder
Trying to get Unifi Dream Machine Pro syslogs sent to Wazuh Manager node processed, i came up with these decoder and rule sets.

NOTE that the UDMPRO name is the host name you set for your UDM hardware, it shows up in the wazuh logging as the hostname. Wazuh can figure out the date stamp at the beginning and pulls the hostname next, but i couldnt get information properly after that..

I set up some filter rules specifically for LAN_IN initially, but see that there is a lot of different types of log lines i might get from the UDM, so i have a generic one as well. That way i can periodically review the wazuh events (using discover) and see if i need to add new decoders or rules.

Online i see a lot of comments about people trying to get this to work but no one seems to ever actually post their decoders or rules..

I suspect i could make this work better with a parent-child type setup.. but i'm still new to this.
