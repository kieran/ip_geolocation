IP Geolocation
==============

Modifies the IPAddr class to provide a _dead simple_ geolocation method.

To do this, it relies on a free web service at http://geoip.wtanaka.com 
provided by Wesley Tanaka. He deserves your thanks.

Usage
-----

    IPAddr.new('1.2.3.4').geolocate #=> {:code=>'ca',:name=>'Canada'}
    
Bad IP's will raise `IPAddrInvalidError`, 
and you will get a `IPAddrTimeoutError` if the service times out


I forked Carsten
----------------

[You may prefer geoquery](http://github.com/heycarsten/geoquery/tree/master)
