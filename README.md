<a name="readme-top"></a>

<h3 align="center">SysVinit version of <a target="_blank" href="https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html">amazon-ssm-agent</a></h3>


## Installation


### <a href="https://www.devuan.org/" target="_blank">Devuan</a>/<a href="https://www.debian.org/" target="_blank">Debian</a>
1. Download the deb
   ```
   wget -O amazon-ssm-agent-sysvinit.deb https://raw.githubusercontent.com/jkister/amazon-ssm-agent-sysvinit/master/pkg/amazon-ssm-agent-sysvinit.deb
   ```
2. Install the deb
   ```
   sudo dpkg -i ./amazon-ssm-agent-sysvinit.deb
   ```
3. Enjoy

### Others
1. Clone the repo
   ```
   git clone git@github.com:jkister/amazon-ssm-agent-sysvinit.git
   cd amazon-ssm-agent-sysvinit/deb
   ```
2. Copy files around
   ```
   sudo cp -R usr/* /usr/
   sudo cp -R etc/* /etc/
   ```
3. Set up startup (not just for Debian)
   ```
   sudo bash DEBIAN/postinst
   ```
4. Enjoy
