emailpoubelle
=============
A Yunohost version of Email Poubelle by David Mercereau. All thanks to David. 
http://www.mercereau.info/sortie-de-la-version-1-0-demailpoubelle-php-email-jetable-auto-hebergeable/
Original packaging done by Matlink, https://github.com/matlink/emailpoubelle_ynh

WARNING
=========
Using this will cause to disable the Yunohost ldap aliases ! Once installed, you won't be able to use the aliasses settings that you can see when you modify your personnal settings in the SSOWAT pannel.
Of course, once uninstalled, everything get back to normal. 

TODO : 
------
[X] move to 2.0

[ ] check nginx conf

[X] insert clean index.php

[ ] insert cron in conf

[ ] insert symlink for langages in /lang

[X] check dependency for lang

[X] remove php-geoip 

[ ] remove new locale on remove

[ ] Implement Admin panel

[ ] Test it ! (and check if that doesn't interfer with postfix and its aliases)

[ ] cron job to remove redirections (0 */2 * * * /usr/bin/wget -q -t 1 -T 7200 -O /dev/null 'https://domain/poubelle/index.php?act=cron' >/dev/null 2>&1) conflict with SSOWAT + non-public app
