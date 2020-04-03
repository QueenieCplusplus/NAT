# NAT

    ---------------------------------------------------------
    |                                                       |
    |      Inside Network    inside_Host2  inside_Router2   |
    |                                                       |
    |       inside_Host1                                    |
    |                                                       |
    |       inside_Router1                   Nat Router
    |
    ---------------------------------         
                                                Outside Network
                                                
                                                
                                                Outside_RouterN
                                                
                                                
                                          Outside_HostN       Outside_HostN-1
                                                
# NAT Table and its Entries

a router performing NAT maintains a NAT Table, and there are 5 fields:

* Protocol

* Inside Local IP Addr

* Inside Global IP Addr

* Outside Local IP Addr

* Outside Global IP Addr
