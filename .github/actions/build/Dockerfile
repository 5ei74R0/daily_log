FROM rust:latest

RUN cargo install mdbook --no-default-features --features output --vers "^0.4.0"

CMD ["mdbook", "build"]
