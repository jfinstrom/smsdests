smsdests
========

##The basic Idea

Currently we have a "pager" field in FreePBX for voicemail. This would hook in and replace that field with

SMS Destination: {Phone Number} {Dropdown of carriers}

This would store in the database something like
14805551212@sms.carrier.com

##Other uses

Any module that wants a field for sending an email to an SMS gateway.

##The class
This will support FreePBX 12+ not to sure on previous versions.
PUT/GET data handled as json

$Smsdest->getCarriers() - Get list of Carriers, domains, descriptions
$Smsdest->addCarrier($json) - add carrier
$Smsdest->delCarrier($id) - delete carrier
$Smsdest->getUser($id)


##Notes
With number porting there is no automagic way to determine carrier

##TODO

Finish class
everything
