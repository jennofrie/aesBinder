# aesBinder

Bind 2 executables and have them run at the same time.

The script can be encrypted with the -e switch, but if either of your exe's are detected by AV they still will be, because the script just writes out the exe's to a system variable eg. TEMP, then runs them both at the same time.
This only works on windows. flare-dropper.py can be compiled into an exe with pyinstaller or py2exe.

There are two modes of operation: self-contained and URL-drop.


	usage: ./aesBinder.py [options]
	
	optional arguments:
	  -h, --help            show this help message and exit
	  -m MEXE, --mexe MEXE  Malicious exe/bat/vbs to drop, hide and run.
	  -i IEXE, --iexe IEXE  Inert exe/bat/vbs to drop and run.
	  -u URL, --url URL     URL to download and run binary from.
	  -v VAR, --var VAR     System variable to place the files, eg TEMP
	  -e, --encrypt         Encrypt the dropper to evade AV.


![aesBinder](https://user-images.githubusercontent.com/58376175/138593710-c4119098-94b2-4447-b306-cc1150201f93.PNG)
