This caputures screenshots of webpages using Chrome. You place your list of URLs in the array at the top of the script and then load the ChromeShot.html file into a Chrome browser with remote debugging enabled. The commands below show you how to start Chrome with remote debugging enabled. Don't click around on the tabs while it is working because it can only screenshot the page that is in the forefront. You will be left with a single tab at the end showing the report. You can save this report with the Chrome save option. When you have your report you should shut this browser to end the debugger and also to stop using a browser with web-security disabled.

# Windows

## Windows 10

### 64 Bit

```"%PROGRAMFILES(X86)%\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins file:///C:/Full/Path/To/ChromeShot.html``

### 32 Bit

```"%PROGRAMFILES%\Google\Chrome\Application\chrome.exe"  --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins file:///C:/Full/Path/To/ChromeShot.html```

## Windows 7

```"%localAppData%\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222 --disable-web-security --user-data-dir="%localAppData%/Google/Chrome/User Data" --disable-plugins file:///C:/Full/Path/To/ChromeShot.html```

# OS X

```"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"  --remote-debugging-port=9222 --disable-web-security --user-data-dir="$HOME/Library/Application Support/Google/Chrome" --disable-plugins https://www.google.com/```

# Linux

```google-chrome --remote-debugging-port=9222 --disable-web-security --user-data-dir="~/.config/google-chrome/default" --disable-plugins https://www.google.com```
