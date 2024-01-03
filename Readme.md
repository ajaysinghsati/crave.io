for Linux
```bash
curl -s https://raw.githubusercontent.com/accupara/crave/master/get_crave.sh | bash -s --
```
install necessary package 
```bash
sudo apt install rsync
```
## Download crave.config from api section in same directory where you download the crave binary
# Connect to your Devspace
```bash
./crave devspace
```
#  Inside Devspace
## Run Crave inside your Devspace, use the command below to check the available command options.
```bash
crave clone --help
# list                List all crave clones
# destroy             Destroy the clone
# create              Create the clone
```
```bash
crave clone list
```
## Clone the available project using Project Id inside a destination dir.
```bash
crave clone create --projectID <Project ID from crave clone list> <destination dir>
```
## Destroy or remove the cloned project using destination dir name.
```bash
crave clone destroy <destination dir>
```
## start the build using check that the you are under repo directory
```bash
crave run --no-patch "put commands that required for build and use && when you put next command"

