# subjs (Fetches javascript file from a list of URLS or subdomains)

https://github.com/lc/subjs


Usage:

Examples:

$ cat urls.txt | subjs 

$ subjs -i urls.txt

$ cat hosts.txt | gau | subjs


To display the help for the tool use the -h flag:

$ subjs -h

Flag 	Description 	Example
-c 	Number of concurrent workers 	subjs -c 40
-i 	Input file containing URLS 	subjs -i urls.txt
-t 	Timeout (in seconds) for http client (default 15) 	subjs -t 20
-ua 	User-Agent to send in requests 	subjs -ua "Chrome..."
-version 	Show version number 	subjs -version"
Installation
From Source:

$ GO111MODULE=on go get -u -v github.com/lc/subjs


From Binary

You can download the pre-built binaries from the releases page and then move them into your $PATH.

$ tar xvf subjs_1.0.0_linux_amd64.tar.gz

$ mv subjs /usr/bin/subjs

