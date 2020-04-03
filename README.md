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
                                          
                                          
# NAT features

it is a process by a router to replace the original IP addr of both the Source & Destination with different IP addr. 

# NAT can resolve the Problems:

1. to reuse(重複使用) IP addr to resolve the global ip addr space depletion(過度消耗).


2. to solve the overlapping (same) private IP address allocates to 2 companies which of which merge with the other.


3. to be LB for specific service from server, make user to perseive/recognize（感知認知到）they are connecting with a single server, but multi-servers in reality.
                                          
                                                
# NAT Table and its Entries

a router performing NAT maintains a NAT Table, and there are 5 fields:

* Protocol

* Inside Local IP Addr

* Inside Global IP Addr

* Outside Local IP Addr

* Outside Global IP Addr

The NAT table can be populated with entry in 2 ways, the 1st of wich is called "static NAT", and which is set by admin, the 2nd way is called "dynamic NAT", it is created when the Router receives the datagrams, whose character satisfies the rule of NAT set by the admin.
