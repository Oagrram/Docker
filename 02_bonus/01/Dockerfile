FROM python:2.7.10

WORKDIR /game

COPY ./Astray .

CMD ["python", "-m", "SimpleHTTPServer", "80"]

# git clone https://github.com/wwwtyro/Astray.git && docker build -t 01 . && docker run -it -p 8080:80 --rm 01