# fail2ban

	fail2ban
 	sudo apt-get install fail2ban                                                                                      
	nano /etc/fail2ban/jail.d/defaults-debian.conf                                                                     
 	cp /etc/fail2ban/jail.d/defaults-debian.conf /etc/fail2ban/jail.d/ssh.conf                                         
 	nano /etc/fail2ban/jail.d/ssh.conf 
	[sshd]                                                                                                                  
	enabled  = true                                                                                             
        port     = 22124                                                                                                        
	filter   = sshd                                                                                                      
   	logpath  = /var/log/auth.log                                                                  
 	maxretry = 3                                                                                  
 	nano /etc/fail2ban/jail.conf 
	bandtime = -1
