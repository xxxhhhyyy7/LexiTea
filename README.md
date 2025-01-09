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

## TODO

1. Project Planning & Design | 项目规划与设计
  - [x] Project name and scope definition | 项目名称与范围定义
  - [x] Basic README creation | 基础 README 创建
  - [ ] System architecture design | 系统架构设计
  - [ ] Interface design (TUI layouts) | 界面设计（TUI 布局）
  - [ ] Core data structures design | 核心数据结构设计
  - [ ] Define key interfaces | 定义关键接口

2. Development Environment Setup | 开发环境搭建
  - [ ] Repository initialization | 仓库初始化
  - [ ] Go mod initialization | Go mod 初始化
  - [ ] Dev dependencies setup | 开发依赖设置
  - [ ] Basic project structure setup | 基础项目结构搭建
  - [ ] Create development guidelines | 创建开发指南

3. Core Domain Implementation | 核心域实现
  - [ ] Word entity implementation | 单词实体实现
  - [ ] Review scheduler implementation | 复习调度器实现
  - [ ] Ebbinghaus algorithm implementation | 艾宾浩斯算法实现
  - [ ] Unit tests for core logic | 核心逻辑单元测试

4. Infrastructure Layer | 基础设施层
  - [ ] Data persistence interface | 数据持久化接口
  - [ ] JSON storage implementation | JSON 存储实现
  - [ ] Configuration management | 配置管理
  - [ ] Error handling strategy | 错误处理策略

5. TUI Implementation | TUI 实现
  - [ ] Base application model | 基础应用模型
  - [ ] Main menu view | 主菜单视图
  - [ ] Learning session view | 学习会话视图
  - [ ] Review session view | 复习会话视图
  - [ ] Statistics view | 统计视图
  - [ ] Keybinding setup | 按键绑定设置

6. Testing & Documentation | 测试与文档
  - [ ] Integration tests | 集成测试
  - [ ] User documentation | 用户文档
  - [ ] Code documentation | 代码文档
  - [ ] Example configurations | 示例配置

7. Release Preparation | 发布准备
  - [ ] Performance optimization | 性能优化
  - [ ] Error handling review | 错误处理审查
  - [ ] Documentation review | 文档审查
  - [ ] Release workflow setup | 发布工作流设置


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