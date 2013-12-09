gold\_importer
=============

### Installing Ruby DB2 drivers
- Unpack the tarball found in the 3rdparty directory to a suitable location:
    tar -C /tmp -xzf 3rdparty/ibm\_data\_server\_driver\_package\_linuxx64\_v10.5.tar.gz
- Change to the directory created
    cd /tmp/dsdriver
- If you are not using ksh as your shell,  make the installation script writable:
    chmod +w installDsDriver 
- Open /tmp/dsdriver/installDSDriver and change the first line to point to your shell (e.g. /bin/bash)
- Run the installation script
    ./installDSDriver
- When running bundler for the first time:
    IBM_DB_HOME=/tmp/dsdriver/ bundle
