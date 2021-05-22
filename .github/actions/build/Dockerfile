FROM rust:latest

RUN cargo install mdbook --no-default-features --features output --version "^0.4.5"

CMD ["mdbook", "build"]
