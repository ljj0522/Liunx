apt update
apt-get install ca-certificates curl gnupg lsb-release -y
apt-get install docker.io -y

docker pull selenium/standalone-chrome

docker run -d -p 4440:4444 -p 7900:7900 --shm-size="2g" -e SE_VNC_PASSWORD=JnY8LWWUo0tH -e http_proxy="http://" -e https_proxy="http://" selenium/standalone-chrome:latest

http://192.168.1.1:7900?autoconnect=1&resize=scale&password=JnY8LWWUo0tH

https://chromewebstore.google.com/detail/gradient-sentry-node/caacbgbklghmpodbdafajbgdnegacfmo

https://chromewebstore.google.com/detail/dawn-validator-chrome-ext/fpdkjdnhkakefebpekbdhillbhonfjjp
