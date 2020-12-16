FROM rustlang/rust:nightly

# libmysqlclient needed for diesel_cli
RUN apt-get install libmariadb-dev-compat libmariadb-dev

RUN cargo install diesel_cli --no-default-features --features mysql

RUN cargo install cargo-watch

WORKDIR /usr/src/app

EXPOSE 3001

VOLUME ["/usr/local/cargo"]
