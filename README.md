# Dns Leak Test
The test shows DNS leaks and your external IP. If you use the same ASN for DNS and connection - you have no leak, otherwise here might be a problem.

## How to install & use Bash Version   

Please, before use make sure you have `curl`, `ping` and `jq` installed.

### Linux

1. Download dnsleaktest.sh
```
wget https://raw.githubusercontent.com/macvk/dnsleaktest/master/dnsleaktest.sh
```

```
chmod +x dnsleaktest.sh
```

2. Run dnsleaktest.sh
```
./dnsleaktest.sh
```

### macOS

1. Download dnsleaktest.sh

```
curl https://raw.githubusercontent.com/macvk/dnsleaktest/master/dnsleaktest.sh -o dnsleaktest.sh
```

```
chmod +x dnsleaktest.sh
```

2. Run dnsleaktest.sh
```
./dnsleaktest.sh
```


-----------------------------------------------------

## How to install & use Python Version                                                                                  

### Linux & Windows Python way

1. Download dnsleaktest.py
```
wget https://raw.githubusercontent.com/macvk/dnsleaktest/master/dnsleaktest.py
```

```
chmod +x dnsleaktest.py
```

2. Run dnsleaktest.py
```
./dnsleaktest.py
```

### Windows CMD way

1. Download dnsleaktest.bat

```
powershell -command "& { (New-Object Net.WebClient).DownloadFile('https://raw.githubusercontent.com/macvk/dnsleaktest/master/dnsleaktest.bat', 'dnsleaktest.bat') }"
```

2. Run dnsleaktest.bat
```
dnsleaktest.bat
```

### macOS

1. Download dnsleaktest.py

```
curl https://raw.githubusercontent.com/macvk/dnsleaktest/master/dnsleaktest.py -o dnsleaktest.py
```

```
chmod +x dnsleaktest.py
```

2. Run dnsleaktest.py
```
./dnsleaktest.py
```


-----------------------------------------------------

## How to build & use Golang Version                                                                                  

You can use prebuilt executable binary for Linux, MacOs or Windows [created by travis-ci.org](https://github.com/macvk/dnsleaktest/releases/):

### Linux

1. Download [dnsleaktest v1.2](https://github.com/macvk/dnsleaktest/releases/download/v1.2/dnsleaktest)

```
chmod +x dnsleaktest
```

2. Run dnsleaktest
```
./dnsleaktest
```

### Windows

1. Download [dnsleaktest.exe v1.2](https://github.com/macvk/dnsleaktest/releases/download/v1.2/dnsleaktest.exe)

2. Run dnsleaktest.exe, 
open cmd then navigate to the exe file
```
dnsleaktest.exe
```

### macOS

1. Download [dnsleaktest v1.2](https://github.com/macvk/dnsleaktest/releases/download/v1.2/dnsleaktest)

```
chmod +x dnsleaktest
```

2. Run dnsleaktest
```
./dnsleaktest
```

### Or build binaries in your machine 

1. Linux 
```
GOOS=linux GOARCH=386 go build -o dnsleaktest dnsleaktest.go

```
2. MacOS

```
GOOS=linux GOARCH=386 go build -o dnsleaktest dnsleaktest.go
```
3. Windows

```
GOOS=windows GOARCH=386 go build -o dnsleaktest.exe dnsleaktest.go

```
