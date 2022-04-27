FROM debian
RUN apt-get update &&  apt-get -y upgrade && \
apt install -y wget lbzip2 && \
wget https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
lbzip2 -d teamspeak3-server_linux_amd64-3.13.6.tar.bz2 && \
tar -xf teamspeak3-server_linux_amd64-3.13.6.tar && \
cd teamspeak3-server_linux_amd64 && \
touch .ts3server_license_accepted
WORKDIR /teamspeak3-server_linux_amd64/
ENTRYPOINT ./ts3server_minimal_runscript.sh start


#docker run -it --name teamspeak -p 9987:9987/udp -p 10011:10011 -p 30033:30033 -e TS3SERVER_LICENSE=accept ex01
