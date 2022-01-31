# Scipt to regenerate Directadmin DNS records

`rm -f fix_db.sh && rm -f fix.sh && wget https://raw.githubusercontent.com/yatosha/directadmin_dns/master/fix_db.sh && wget https://raw.githubusercontent.com/yatosha/directadmin_dns/master/fix.sh && chmod 755 fix_db.sh && chmod 755 fix.sh`
 
`sh fix_db.sh && sh fix.sh`
# Sync DNS Zones
`echo "action=rewrite&value=named" >> /usr/local/directadmin/data/task.queue`