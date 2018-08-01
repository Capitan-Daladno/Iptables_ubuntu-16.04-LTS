# iptables
# Generataed by iptables-save v1.6.0 on Wed Aug 1 05:22:12 2018
# filter убрать одну звезду 
# :INPUT DROP [5:204]
# :FORWARD DROP [0:0]
# :OUTPUT ACCEPT [123:11877]
# :f2b-ssh - [0:0]
# :f2b-sshd - [0:0]
# -A INPUT -p tcp -m multiport --dports 22 -j f2b-ssh
# -A INPUT -p tcp -m multiport --dports 22 -j f2b-sshd
# -A INPUT -p tcp -m tcp --dort 22 -j ACCEPT
# -A INPUT -p icmp -j ACCEPT
# -A f2b-ssh -j RETURN
# -A f2b-sshd -J RETURN
# COMMIT
# Completed on Wed Aug 1 05:22:12 2018 
