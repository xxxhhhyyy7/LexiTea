# LexiTea

🍵 A delightful TUI vocabulary learning application powered by the Ebbinghaus forgetting curve.

## Overview

LexiTea is a terminal-based vocabulary learning tool that implements the Ebbinghaus forgetting curve to optimize your memorization process. Built with Go and the charming Bubble Tea framework, it provides an elegant and efficient interface for vocabulary acquisition and review.

## Features

- 📚 Scientific-based learning using Ebbinghaus forgetting curve
- 🎯 Intelligent review scheduling
- 📊 Learning progress tracking
- ⌨️ Vim-style keyboard navigation
- 💾 Local progress persistence
- 🎨 Beautiful TUI interface

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/lexitea.git

# Enter the project directory
cd lexitea

# Install dependencies
go mod download

# Build the application
go build

# Run LexiTea
./lexitea
```

## Usage

### Key Bindings

- Global
    - `q`, `Ctrl+C`: Quit
    - `h`: Help
    - `Esc`: Go back

- Navigation
    - `j`, `↓`: Move down
    - `k`, `↑`: Move up
    - `Enter`: Select

- Learning Mode
    - `Space`: Show/Hide answer
    - `Enter`: Confirm
    - `n`: Next word

- Review Mode
    - `y`: Know the word
    - `n`: Don't know the word
    - `s`: Skip current word

## Project Structure

```
.
├── cmd/
│   └── lexitea/
│       └── main.go
├── internal/
│   ├── core/
│   │   ├── word.go
│   │   └── scheduler.go
│   ├── storage/
│   │   └── repository.go
│   └── tui/
│       ├── views/
│       └── state.go
├── pkg/
│   └── utils/
├── go.mod
├── go.sum
└── README.md
```

## Ebbinghaus Review Schedule

LexiTea follows the scientifically proven Ebbinghaus forgetting curve with the following review intervals:

1. First review: 30 minutes after learning
2. Second review: 12 hours after learning
3. Third review: 24 hours after learning
4. Fourth review: 2 days after learning
5. Fifth review: 4 days after learning
6. Sixth review: 7 days after learning
7. Seventh review: 15 days after learning

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Bubble Tea](https://github.com/charmbracelet/bubbletea) - The elegant TUI framework
- [Hermann Ebbinghaus](https://en.wikipedia.org/wiki/Hermann_Ebbinghaus) - For his groundbreaking research on memory

---
Built with ❤️ using Go and Bubble Tea