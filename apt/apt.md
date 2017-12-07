Configure apt-get behind proxy.

Helpful links


https://stackoverflow.com/a/38833454/3629379

https://stackoverflow.com/a/47288908/3629379


* Change user to root

```sh
$ sudo su
```

* create a new empty file apt.conf in /etc/apt/

```sh
$ nano /etc/apt/apt.conf
```

* Add this line to the file if you are using http proxy else https of ftp:

```sh
Acquire::http::Proxy "http://user:pass@proxy_host:port";
```

* Add a new file in root user , ~/.bash.rc to make this command permanent

```sh
$ nano ~/.bash.rc
```

```sh
export http_proxy=http://user:pass@proxy_host:port
```

* Run it in current session.

```sh
$ . .bash.rc
```

* Then run apt-get update.

```sh
$ apt-get update
```