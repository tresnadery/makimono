# Makimono: Wrapper Logger Using Channels, Goroutines, and Zap

**Makimono** is a lightweight logging wrapper built in Go that integrates **Zap** for structured and high-performance logging. It utilizes **channels** and **goroutines** to ensure efficient and concurrent logging without blocking the main application flow, while also taking full advantage of Zap’s fast logging features.

## Features:
- **Asynchronous Logging**: Makimono uses **goroutines** to handle log messages concurrently, improving performance in high-traffic applications.
- **Thread-Safe**: With the help of **channels**, Makimono ensures thread-safe logging and avoids the need for explicit synchronization (mutexes).
- **Structured Logging**: Built on top of **Zap**, Makimono allows you to leverage structured logging, making it easier to track and query logs.
- **High Performance**: Zap’s optimizations ensure that Makimono maintains low-latency and high throughput in log processing.

## Installation:

To install **Makimono**, run the following commands:

```bash
go get github.com/tresnadery/makimono