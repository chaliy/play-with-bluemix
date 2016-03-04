## Prerequisits

Details https://console.ng.bluemix.net/docs/containers/container_cli_ov.html#container_cli_ov

    cf install-plugin https://static-ice.ug-gb.bluemix.net/ibm-containers-windows_x64.exe


## First time

    cf ic namespace set chaliy_play_with_bluemix
    cf ic login # Follow instructions to setup your shell

    docker ps # to check
    docker-machine start default # On windows
    docker-machine env default | iex # On windows
    cf ic images # To check it works    

    cf ic build -t play-with-bluemix .
    cf ic run registry.eu-gb.bluemix.net/chaliy_play_bluemix/play-with-bluemix

## Build

    cf ic build -t play-with-bluemix .
    cf ic run -p 3000:3000 registry.eu-gb.bluemix.net/chaliy_play_bluemix/play-with-bluemix
    cf ic ps # To check if running...
