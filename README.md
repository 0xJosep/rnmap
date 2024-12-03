# RNMAP - Rust Network Port Scanner

RNMAP is a fast, multi-threaded port scanner written in Rust. It allows you to scan for open ports on a target IP address with customizable thread counts for optimized performance.

```
░▒▓███████▓▒░░▒▓███████▓▒░░▒▓██████████████▓▒░ ░▒▓██████▓▒░░▒▓███████▓▒░  
░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░ 
░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░ 
░▒▓███████▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓████████▓▒░▒▓███████▓▒░  
░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░        
░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░        
░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░        
                                                v1.0 by @0xJosep
```

## Features

- Multi-threaded scanning for improved performance
- Progress bar visualization of scan progress
- Customizable thread count
- Scans all ports (1-65535)
- Simple and intuitive command-line interface
- Written in Rust for memory safety and performance

## Prerequisites

- Rust (Latest stable version)
- Cargo (Comes with Rust)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/rnmap.git
cd rnmap
```

2. Build the project:
```bash
cargo build --release
```

3. The binary will be available at `target/release/rnmap`

### System-wide Installation

#### Linux/MacOS
```bash
sudo cp target/release/rnmap /usr/local/bin/
```

#### Windows
- Add the binary location to your PATH environment variable
- Or copy the executable to a directory that's already in your PATH

## Usage

Basic syntax:
```bash
rnmap [OPTIONS] IP_ADDRESS
```

Options:
- `-t, --threads <number>`: Specify number of threads (default: 4)
- `-h, --help`: Show help message

Examples:
```bash
# Basic scan with default threads
rnmap 192.168.1.1

# Scan with 1000 threads
rnmap -t 1000 192.168.1.1

# Show help
rnmap -h
```

## Security Notice

This tool is intended for network administrators and security professionals to scan their own networks or networks they have explicit permission to test. Unauthorized port scanning may be illegal in some jurisdictions.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[Your chosen license]

## Author

@0xJosep

## Disclaimer

The creator of this tool is not responsible for any misuse or damage caused by this program. Use at your own risk and only on networks you have permission to scan.