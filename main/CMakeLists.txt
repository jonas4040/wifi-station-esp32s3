idf_component_register(SRCS "wifi-station-esp32s3.c"
                    INCLUDE_DIRS "."
                    REQUIRES esp_wifi
                    nvs_flash
                    wifi-station
                    )
