FROM debian

WORKDIR /src/c

RUN apt update && apt -y  upgrade && apt install -y  build-essential && apt install -y vim 

 COPY ./ANSI-color-code-in-c-programming/main.c .

RUN gcc main.c

CMD  ./a.out

# git clone https://github.com/Guleri24/ANSI-color-code-in-c-programming.git && docker build -t 05 . && docker run -it 05