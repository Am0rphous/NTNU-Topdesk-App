# NTNU Topdesk App

So I was annoyed I had to open the service management plattform a lot because I had so many new updates on cases. I decided to see if I could make a local "app" running on my computer, which saved me a lot of time.
I found the now archived project Nativefier which "make any web page a desktop application" which was perfect. Remember, to make it portable read the `#portable` at [this](https://github.com/nativefier/nativefier/blob/master/API.md#portable) link. 

A longer description of Nativefier is as follows: _"Nativefier is a command-line tool to easily create a “desktop app” for any web site with minimal fuss. Apps are wrapped by Electron (which uses Chromium under the hood) in an OS executable (.app, .exe, etc) usable on Windows, macOS and Linux."_


To build yourself:
1. Install `nativefier`
````
brew install nativefier    #for macOS
````
2. I found these parameters to fulfill my needs. 
````
nativefier --name "hjelp" "https://hjelp.ntnu.no/" --tray --portable
````
3. Expected output may look like this:
````
    Hi! Nativefier is minimally maintained these days, and needs more hands.
    If you have the time & motivation, help with bugfixes and maintenance is VERY welcome.
    Please go to https://github.com/nativefier/nativefier and help how you can. Thanks.

Processing options...
Building app as portable. SECURITY WARNING: all data accumulated in the app folder after running it (including login information, cache, cookies) will be saved in the app folder. If this app is then shared with others, THEY WILL HAVE THAT ACCUMULATED DATA, POTENTIALLY INCLUDING ACCESS TO ANY ACCOUNTS YOU LOGGED INTO.

Preparing Electron app...

Converting icons...

Packaging... This will take a few seconds, maybe minutes if the requested Electron isn't cached yet...

Finalizing build...
App built to /Users/Username/Downloads/myWebApp/hjelp-darwin-x64, move to wherever it makes sense for you and run the app bundle.
````
4. In my case I opened the executable located in folder `myWebApp/hjelp-darwin-x64/` which was named `hjelp`. Cheers!
