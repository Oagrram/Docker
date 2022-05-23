FROM rust:1.24.0

COPY ./rust_app_hello .

WORKDIR ./rust_app_hello

RUN cargo build 

CMD cargo run

#git clone https://github.com/Oagrram/rust_app_hello.git &&  docker build -t 03 . && docker run -it 03 