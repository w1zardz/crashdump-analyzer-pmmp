# PocketMine-MP Crashdump Analyzer

**Free online tool to instantly decode PocketMine-MP server crashdumps into human-readable diagnostics.**

[**Use the Analyzer →**](https://w1zardz.github.io/crashdump-analyzer-pmmp/)

## What it does

When your PocketMine-MP server crashes, it generates a crashdump file containing a wall of technical data. This tool parses that data and tells you:

- **Which plugin** caused the crash (if any)
- **What error** occurred and on which line
- **Human-readable explanation** of the error
- **How to fix it** — actionable suggestions for each error type

## Features

- Supports **PocketMine-MP 3.x, 4.x, and 5.x** crashdump formats
- Parses both **text-based** and **JSON/base64-encoded** crashdumps
- Detects **10+ error types**: null method calls, class not found, type errors, out of memory, timeouts, segfaults, permission errors, and more
- **Drag & drop** or paste crashdump content
- **100% client-side** — no data is ever sent to any server
- **Mobile-optimized** — works perfectly on phones and tablets
- Works **offline** once the page has loaded

## Supported error types

| Error Type | Description |
|---|---|
| Null method call | Method called on null object |
| Class not found | Missing class/dependency |
| Type error | Wrong argument type passed |
| Out of memory | Server RAM exceeded |
| Timeout | Infinite loop or heavy operation |
| Undefined offset | Missing array key |
| Undefined property | Missing object property |
| Redeclaration | Duplicate class/function conflict |
| Segmentation fault | Low-level PHP crash |
| Permission denied | File access issues |

## How to use

1. Open [the analyzer](https://w1zardz.github.io/crashdump-analyzer-pmmp/)
2. Paste your crashdump content **or** drag & drop a `.crash` / `.log` file
3. Click **Analyze**
4. Read the diagnosis and follow the suggestions

## Privacy

All analysis happens locally in your browser using JavaScript. Your crashdump content is **never uploaded, stored, or transmitted** anywhere.

## Contributing

Found a crashdump format that isn't parsed correctly? [Open an issue](https://github.com/w1zardz/crashdump-analyzer-pmmp/issues) with a sample (redact any sensitive info) and we'll add support for it.

## License

MIT
