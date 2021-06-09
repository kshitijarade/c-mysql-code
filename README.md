# C MYSQL API Skeleton Project

This is a C program written to connect to mysql database on macOS

## Prerequisite and software Installations
First download and install [mysql-community](https://dev.mysql.com/downloads/mysql/5.7.html) server

Use brew to install packages on mac

```bash
brew install mysql-client
```
Then add following to your system PATH variable
```
export PATH=/usr/local/opt/mysql-client/bin:$PATH
```

## Usage

```bash
gcc -o main $(mysql_config --cflags) Main.c $(mysql_config --libs) -L/usr/local/opt/openssl/lib
```
or
```bash
gcc -o main Main.c `mysql_config --cflags --libs` -L/usr/local/opt/openssl/lib
```

`-L/usr/local/opt/openssl/lib` is required if you get `ld: library not found for -lssl` error

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Video Tutorial on Linux
[YouTube](https://www.youtube.com/watch?v=jACHG6tZakw)

