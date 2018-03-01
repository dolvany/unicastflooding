# unicastflooding
A tcpdump bpf filter for detection of unicast flooding. Just replace the mac address with the address of the host that you are capturing from and you should be left with flooded unicast.

tcpdump -n 'ether[0]&1=0 and not ether host 00:11:22:33:44:55'
