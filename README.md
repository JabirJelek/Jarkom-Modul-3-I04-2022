# Jarkom-Modul-3-I04-2022
<strong> Our Members :
1. Farzana Afifah Razzak 
2. Raihan Farid
3. Muhammad Azka Aysar 
</strong>

## 1. Loid with Franky plan to create the map above with criteria WISE as DNS Server, Westalis as DHCP Server, Berlint as Proxy Server 
 we can enter this code into WISE, to make it as DNS Server
```bash
apt-get update
apt-get install bind9 -y
service bind9 restart
```

And enter this syntax in Berlint to make it as Proxy Server
```
apt-get update
apt-get install squid -y
service squid start
```

Last, we enter this syntax into Westalis to make it as DHCP Server
```
apt-get update
apt-get install isc-dhcp-server -y
service isc-dhcp-server start
```


## 2. and Ostania as DHCP Relay

Enter This syntax in Ostania to make it as DCHP Relay
```bash
apt-get update
apt-get install isc-dhcp-relay -y
service isc-dhcp-relay start
```


## 3.Client that go through Switch1 have the IP range from [prefix IP].1.50 - [prefix IP].1.88 and [prefix IP].1.120 - [prefix IP].1.155 

## 4. Client that go through Switch3 have the IP range from [prefix IP].3.10 - [prefix IP].3.30 dan [prefix IP].3.60 - [prefix IP].3.85

## 5. Client gets the DNS from WISE and client can connect to the internet through the DNS.

## 6. The length of time the DHCP server lends an IP address to client via Switch1 is 5 minutes, while the client via Switch3 is 10 minutes. With a maximum time allocated for borrowing an IP address is 115 minutes.

## 7. Loid and Franky plan to make Eden as a server for exchanging information with a fixed IP address with IP [prefix IP].3.13
