# Scipt to regenerate Directadmin DNS records
This script regenerates all dns records and updates named.conf records. It also syncs dns records

`rm -f fix_db.sh && rm -f fix.sh && wget https://raw.githubusercontent.com/yatosha/directadmin_dns/master/fix_db.sh && wget https://raw.githubusercontent.com/yatosha/directadmin_dns/master/fix.sh && chmod 755 fix_db.sh && chmod 755 fix.sh && sh fix_db.sh && sh fix.sh && echo "action=rewrite&value=named" >> /usr/local/directadmin/data/task.queue && echo done`
