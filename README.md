# Cronjobs
Thing that need to know for cronjobs

#Check list of Cronjobs :

crontab -l

#Edit cronjob :

crontab -e

#Remove cronjobs :

crontab -r

#Set cronjob in ubuntu :

0 * * * * /usr/bin/php /var/www/html/check_status.php // Provide absolute path
//It's for once per hour

#Set cronjob in linux :

0 * * * *  wget -q https://www.nileshpatil.xyz/test_cron  -O /home/ec2-user/test_cron

#Set cronjob by adding timeout limit :

0 * * * * wget --read-timeout=3600 -o https://www.nileshpatil.xyz/test_cron  -O /home/ec2-user/test_cron //-o indicate generate cron output in server log
