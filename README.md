# victron-bland-exporter-requirements
1. android app apk
2. android app connects to victron mppt over bluetooth
3. android app reads the data from victron mppt over bluetooth
4. android app had a cloudflared inside it
5. there is a /metrics server inside the android app
6. android app has a form for the user to enter cloudflared token
7. android app has a status page for cloudflared logs and status at a glance
8. the /metrics endpoint should expose the data of victron mppt example voltages, currents , wattage
9. the /metrics endpoint must be readable by prometheus and compatible with prometheus server.
10. the app must run constantly even if the screen is off, the app needs to guide user to help user make the app stay alive , keep cpu alive , aquire wakelock, use persistent notification if needed
11. give user option to disable cloudflared and allow user to access the /metrics endpoint over local ip (wifi) and port  example http://192.168.1.70:5338/metrics where 192.168.1.70 is the wifi ip address of the android device when it is connected to wifi.
12. easu to build - with docker compose , make build command must use docker compose to build and output the apk file
