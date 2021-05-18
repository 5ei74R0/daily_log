# 2021/5/6
|←|→|
|:---|---:|
go to the [previous page](./5th.md) | go to the [next page](./7th.md)

## Univ.
### courses
- **Visual computing**
    - frequency of an image
    - spatial filtering, PSF(Point Spread Function), convolution
    - 2D-DFT & 2D-iDFT
    - frequency filtering
    - sampling theory
        - maximum frequency < Nyquist frequency
          -> avoid aliasing
    - re-sampling

- **Human Interface**

- **Data Modeling**
    - modeling the Entity Relationship Diagram
    - modeling the RDB from Entity Relationship Diagram

- **Network Engineering**
    - Transport Layer protocols
    - TCP (Transmission Control Protocol) : connection-oriented
    - UDP (User Datagram Protocol) : connection-less
    - how to achieve the reliable data transfer above the unreliable data transfer?
        - rdt1.0 ~ rdt3.0
        - deal with error & packet loss
        - stop and wait
        - checksum
        - ARQ (ACK, ~~NAK(~rdt2.1)~~)
        - sequence number
        - time out
    - rdt3.0 is too slow -> next: Protocol pipelining

### homework
- [x] **Visual Computing**
    - Question.  
      why should we use the low pass filter in down sampling?  
      -> Nyquist frequency becomes smaller than maximum frequency because of down sampling.  
      -> then aliasing occurs & the image transforms by mistake.  
      -> we should erase the high frequency in the original image before down sampling.  
      -> we can do this by using the low pass filter.

## Competitive Programming
- [x] solved the problems of competitive programming with Rust
    - [problem](https://atcoder.jp/contests/abc186/tasks/abc186_d)
        - [archived code](https://github.com/OtsuKotsu/training_rust/blob/main/archive/ABC/ABC186/d.rs)
- no contents

## Reading papers, articles, books
- read **The Rust Programming Language**
    - Next : [8.1](https://doc.rust-jp.rs/book-ja/ch08-01-vectors.html)
- read [**paper of Swin Transformer**](https://arxiv.org/pdf/2103.14030v1.pdf)
    - Next : p3 "Self-attention/Transformers to complement CNNs"

## Else
- took a walk
