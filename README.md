# STM32F4_HAL_ETH_MBEDTLS
STM32F4 HAL mbedTLS library testing (SSL/TLS client)

1. Reference<br>
https://engschool.tistory.com/entry/SSLTLS-embedded-for-IoT-8 <br>
https://cxemotexnika.org/2018/10/primer-zashhishhennogo-https-soedineniya-s-ispolzovaniem-mbed-tls/ <br>
https://github.com/PetroShevchenko/cxemotexnika/tree/master/Examples/NUCLEO_F429ZI/nucleo_f429zi_https_client <br>

2. Tutorial [Written in Korean]
https://blog.naver.com/eziya76/221959527368 <br>
https://blog.naver.com/eziya76/221963225897 <br>

3. Issue<br>
solved<br>
https://github.com/eziya/STM32F4_HAL_LWIP_LAB/issues/1

I found a memory leak issue when "mbedtls_ssl_handshake" is called and haven't solved it yet.
To walk around this issue, I used "mbedtls_memory_buffer_alloc_init" and recreate SSL task whenever memory error happens.

4. Testing video
https://youtu.be/gn9HXI1YNUg

