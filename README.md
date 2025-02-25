# Asynchronous Programming in Rust

This is the repository for the book: _Asynchronous Programming in Rust_.

Written by Carl Fredrik Samson, published by Packt

## How to use this repository

My clear recommendation is to clone this repository by either clicking on the `<> Code` button and select "Download ZIP" or clone the repository using your preferred git client.

Each chapter has its own folder in this repository. Each example is organized as a standalone crate within that folder.

When encountering examples in the book, you might find it easier to read the code in the repository since you'll be able to open it up in the editor of your choice and have appropriate highlighting and formatting.

Even if you only write the examples directly from the book line by line, you'll need the repository for `delayserver` and `corofy` which is two tools I wrote to help in the learning process.

## Delayserver

Most of the examples will use a program called delayserver that's provided in this repository. Delayserver is a simple local webserver where you can write a HTTP GET request with a configurable delay.

You have two options for running the delayserver:

1. Go to the folder named `/delayserver` and write `cargo run` in a separate terminal window and leave it running there
2. Go to the same folder and install the server by writing `cargo install --force --path .`. By doing so you install the program locally in you PATH so you can run it from any location by simply writing `delayserver` and leave the terminal process running.

How delayserver works is described in the book, but you'll also find the relevant information in its root folder.

## Corofy

Corofy is another tool that we'll use from chapter 7 onwards. I recommend installing this tool locally by entering the folder `ch7/corofy` and installing it on your machine by writing `cargo install --force --path .`

## I'll be going on a plane, how can I use the repository in an offline situation?

You'll need to install both `delayserver` and `corofy` locally on your machine while you're online. The process is described above.

Most of the examples have no external dependencies, but from chapter 6 onwards
we will have some of them. The best way to be able to run these examples while offline is to enter each folder and use [cargo vendor](https://doc.rust-lang.org/cargo/commands/cargo-vendor.html) to vendor the dependencies locally. This way you'll be able to build and experiment with the examples even though you'll be offline.

----

Asynchronous Programming in Rust, published by Packt
