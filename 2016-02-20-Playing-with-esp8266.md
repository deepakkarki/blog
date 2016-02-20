#Playing with ESP8266

For those of you who don't know, ESP8266 is a Serial to WiFi module available for under 250 rupees (~$3). I managed to get my hands on a couple of them earlier last week and wanted to try them out. My use case was simple - get the module up and running to execute the following workflow

```
Connect ESP to my WiFi --> assign a static IP --> initiate a server on ESP --> 
connect and send data to ESP via my laptop (client) --> get ESP to send a response.
```

For this experiment I wanted to go about doing stuff manually, so no Arduino. Just a plain old USB to Serial converter (3.3V). I used FOCA for this purpose. All setup and executions were done using **AT commands**. 

> AT commands are commands which are used to control the modems where AT stands for Attention. These commands were derived from Hayes commands which were used by the Hayes smart modems. Every wireless as well as the dial up modems require an AT command to interact with a computer machine.

The AT commands are sent over serial, detailed instructions for ESP8266 can be found [here](https://room-15.github.io/blog/2015/03/26/esp8266-at-command-reference).


The steps are as follows - 

1. Set the chip mode.
2. Enable multiple connections.
3. Connect to the WiFi
4. Set static IP.
5. Start TCP server
6. Set the timeout.

(more to come...)
