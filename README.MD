# ESP32S3 CONNECTED TO A ROUTER

* Instructions to run:

   -criar dentro da pasta main, um arquivo chamado Kconfig.projbuild com o seguinte
   <pre>
        <code>
        menu "Wifi Connection Configuration"

    config ESP_WIFI_SSID
        string "WiFi SSID"
        default "myssid"
        help
            SSID (nome da rede) to connect to.

    config ESP_WIFI_PASSWORD
        string "WiFi Password"
        default "mypassword"
        help
            WiFi password (senha - WPA or WPA2) to use.

    config ESP_MAXIMUM_RETRY
        int "Maximum retry"
        default 5
        help
            Numero maximo de tentativas (to avoid station reconnecting to the AP unlimited when the AP is really inexistent).

endmenu
        </code>
   </pre>