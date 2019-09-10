# bitcoin_stratum_controller_client
Stratum client running in micro controller. 
### Difference between linux and RTOS
1. No pthread.
2. No linux libc
3. No select or epoll

## Todo
0. Run a controller project with(FreeRTOS, Lwip, SSL)
1. Copy cgminer stratum code
2. Use [jsmn](https://github.com/zserge/jsmn) as json parse lib so we don't need malloc
3. Use FreeRTOS task to replace cgminer thread.
4. 
