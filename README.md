# build
docker build -t gismo141/gnucash-docker-novnc .

## How to
### Run
Start the container via
```bash
docker run -td \
	-v </your/local/volume>:/var/gnucash \
	-p 6080:6080 \
	-e LOCALE=<your_LOCALE> \
	-e FILE=<your_gnucash_file> \
	-e VNC_PASS=<your_password> \
	gismo141/gnucash-docker-novnc:<tag>
```
Then access via http://localhost:6080.
Default Password is gnucash

### Locales
The following locales are preinstalled
* de_DE
