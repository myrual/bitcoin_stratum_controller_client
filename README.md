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

send command to server

listen data from server



## Todo
0. Run a controller project with(FreeRTOS, Lwip, SSL(optional)).
1. Understand Cgminer function.
2. Write test data for stratum protocol.
3. 
