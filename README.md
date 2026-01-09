# timek - Time Library Extension

⏰ Custom Konsultin time library with Indonesian/English locale and carbon wrapper.

## Installation

```bash
go get github.com/konsultin/timek
```

## Quick Start

```go
import "github.com/konsultin/timek"

// Get current time (defaults to ID locale)
now := timek.Now()

// Format as "DD/MM/YY" (e.g., 15/12/24)
fmt.Println(now.ToDate())

// Format as "DD MMMM YYYY" (e.g., 15 Desember 2024)
fmt.Println(now.ToDateFull())

// Human readable (e.g., "beberapa detik yang lalu")
fmt.Println(now.ToReadable())

// Standard datetime format
fmt.Println(now.ToDateTimeStandard()) // 2024-12-15 14:30:00
```

## Features

- **Multi-language** - Built-in Indonesian (ID) and English (EN) support
- **Custom Formats** - Comprehensive date/time layout constants
- **Human Readable** - Relative time strings ("2 jam yang lalu")
- **Database Compatible** - Implements `Scanner` and `Valuer` interfaces
- **JSON Support** - Proper JSON marshaling/unmarshaling

## License

MIT License - see [LICENSE](LICENSE)
