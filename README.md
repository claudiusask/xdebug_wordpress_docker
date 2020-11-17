# Wordpress Docker xDebug WSL Boilerplate -- 

This boilerplate is to debug Wordpress websites using Docker and VSCode

This works on windows and also WSL2, but with wsl2 there is a problem of IP address changing everytime windows 10 restarts.

## Usage

> Make sure Docker is running and the [PHP Debug](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug) extension for VSCode is installed

> Install PHP and Xdebug on WSL2 main machine.
> Make sure to use WSL2 ip address of main Ubuntu (main machine which docker is using), and update it in docker-compose.yml. This IP address is changed everytime 
> the windows 10 restarts.
> also update the .vscode/launch.json whith the volume used for wordpress.


1. Run the docker instance
```sh
$ docker-compose up
```

2. Open http://localhost:8000

3. Open the debugger tab on the sidebar and run `Listen for XDebug`

4. Set anywhere in your PHP files a breakpoint
