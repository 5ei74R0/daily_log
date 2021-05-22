FROM rust:latest

# RUN cargo install mdbook --no-default-features --features output --version "^0.4.5"

RUN mkdir mdbook
RUN curl -Lf https://github.com/rust-lang/mdBook/releases/download/v0.4.5/mdbook-v0.4.5-x86_64-unknown-linux-gnu.tar.gz | tar -xz --directory=./mdbook
RUN echo `pwd`/mdbook >> $GITHUB_PATH

CMD ["mdbook", "build"]
