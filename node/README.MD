## Dependencies

   choco install cloudfoundry-cli
   choco install node # 5.7+

## Deploy

    npm install
    cf target https://api.eu-gb.bluemix.net
    cf login
    cf push
