# bitcoin_stratum_controller_client
Stratum client running in microcontroller like arm cortex-m4, cortex-m7 with LAN interface. CGminer is good enough for linux on openwrt or linux.

### Difference between linux and RTOS
1. No pthread.
2. No linux libc
3. No select or epoll


What cgminer has done?

config: stratum pool, account, password
api:    provide status for external 

init tcp, udp socket

with each pool:
  send command to server by network
  listen data from server by network
  
  pool can be deactive at any time.

with rig

send data to rig by i2c/spi/uart
    command
    mining data
    
receive data from rig i2c/spi/uart
    found nounce
    status
    
## Todo
0. Run a controller project with(FreeRTOS, Lwip, SSL(optional)).
1. Understand Cgminer function.
2. Write test data for stratum protocol.
3. 
