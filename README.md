# Running the website locally (requires internet)

Build and run it locally:
```shell
bundle exec jekyll serve 
```

Build and run it locally while being accessible to a mobile phone:
```shell
# find your computer's IP first
# https://stackoverflow.com/questions/13322485/how-to-get-the-primary-ip-address-of-the-local-machine-on-linux-and-os-x/13322549#13322549
ifconfig | grep -Eo 'inet (addr:)?([0-9]*\.){3}[0-9]*' | grep -Eo '([0-9]*\.){3}[0-9]*' | grep -v '127.0.0.1'

# host it locally
bundle exec jekyll serve --host=0.0.0.0

# enable the firewall settings
#  -> if on OSX, a dialog should appear where it gives you an option to enable ruby to go through the firewall.

# access via your phone by typing in <computer's IP>:4000 into the address bar of a browser.
```

