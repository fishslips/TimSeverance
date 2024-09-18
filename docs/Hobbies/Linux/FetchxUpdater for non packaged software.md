I created this bash script for fetching and updating software, this example is for vscode
```bash
#!/bin/bash

########################
#      Constants       #
########################

DOWNLOAD_URL="https://code.visualstudio.com/sha/download?build=stable&os=linux-x64"
TEMP_TAR="/tmp/vscode_latest.tar.gz"
INSTALL_DIR="/opt/vscode/"

########################
#       Execute        #
########################

echo "Downloading latest version of VSCode"

wget -O $TEMP_TAR $DOWNLOAD_URL

echo "Extracting package"
sudo mkdir -p $INSTALL_DIR
sudo tar -xvzf $TEMP_TAR -C $INSTALL_DIR --strip-components=1

echo "Cleaning up..."
rm $TEMP_TAR

echo "Creating symlink"

sudo ln -sf $INSTALL_DIR/bin/code /usr/bin/code

echo "VSCode updated successfully."
```

You need to chmod it

```bash
$ chmod +x "update.sh" 
```

Also, #!/bin/bash  makes the script executable