__This does not work__

## Deploy

    dnu publish --runtime dnx-coreclr-linux-x64.1.0.0-rc1-update1
    cd bin/output/
    copy ../../manifest.yml     
    cf target https://api.eu-gb.bluemix.net
    cf login
    cf push chaliy-play-with-bluemix-dotnet -b https://github.com/cloudfoundry-community/asp.net5-buildpack.git
