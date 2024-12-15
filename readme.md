## Concurrent Key-Value Database 💿

embeddable, persistent key-value database with support for concurrent operations and indexing written in golang

## Features
- In-memory and persistent storage
- ACID-like transaction support
- Concurrent read/write operations
- Range and prefix-based queries
- Simple key-value data model

## Installation
```bash
go get github.com/codrion/gokv
```

## Quick Start
```go
db, err := gokv.Open("path/to/database")
defer db.Close()

// Write operations
db.Set("key", "value")
db.Delete("key")

// Read operations
value, err := db.Get("key")
```

## Performance
- O(1) read and write operations
- Configurable concurrency levels
- Memory-mapped file support

## License
MIT License

## Contributing
Contributions welcome. Please read CONTRIBUTING.md
