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

