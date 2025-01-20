# Makimo: Wrapper Logger Using Channels, Goroutines, and Zap

**Makimo** is a lightweight logging wrapper built in Go that integrates **Zap** for structured and high-performance logging. It utilizes **channels** and **goroutines** to ensure efficient and concurrent logging without blocking the main application flow, while also taking full advantage of Zap’s fast logging features.

## Features:
- **Asynchronous Logging**: Makimo uses **goroutines** to handle log messages concurrently, improving performance in high-traffic applications.
- **Thread-Safe**: With the help of **channels**, Makimo ensures thread-safe logging and avoids the need for explicit synchronization (mutexes).
- **Structured Logging**: Built on top of **Zap**, Makimo allows you to leverage structured logging, making it easier to track and query logs.
- **High Performance**: Zap’s optimizations ensure that Makimo maintains low-latency and high throughput in log processing.

## Installation:

To install **Makimo** with Zap as the logger, run the following commands:

```bash
go get github.com/tresnadery/makimo