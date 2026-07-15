# Claude Coding Courses

> Tài liệu học tập tiếng Việt về **Claude Code**, **AI**, **Backend**, **Web3**, **Mobile**, **Machine Learning** và nhiều chủ đề khác — xây dựng trên [Mintlify](https://mintlify.com).

Đây là repo chứa source code cho site docs **Claude Coding Courses** — bộ tài liệu song ngữ (chủ yếu tiếng Việt) hướng dẫn cách dùng [Claude Code](https://claude.com/product/claude-code) để build sản phẩm nhanh hơn 5–10 lần, cùng các khóa học nền tảng về lập trình và AI.

🔗 **Site:** _(sẽ được cập nhật sau khi deploy)_

---

## 📚 Các khóa học

Repo gồm **10 modules** chính, mỗi module là một nhóm tài liệu MDX độc lập:

| # | Module | Mô tả ngắn |
|---|--------|-----------|
| 01 | **[Claude Code](docs/claude-code/overview.mdx)** | Dùng Claude Code để build app Next.js + Firebase, kiến trúc, prompt rules, thực chiến |
| 02 | **[Agentic AI](docs/agentic-ai/overview.mdx)** | Xây dựng AI agent với Claude Agent SDK, LangChain, multi-agent patterns |
| 03 | **[Backend](docs/backend/overview.mdx)** | Backend development — Node.js, Python, database, auth, microservices |
| 04 | **[API](docs/api/overview.mdx)** | Thiết kế & xây dựng REST/GraphQL API với Express, FastAPI, NestJS |
| 05 | **[Web3](docs/web3/overview.mdx)** | Web3 cơ bản, ví, smart contract, dApp, DeFi, NFT |
| 06 | **[Blockchain](docs/blockchain/overview.mdx)** | Solidity, Hardhat, OpenZeppelin, bảo mật smart contract |
| 07 | **[RWA](docs/rwa/overview.mdx)** | Token hóa tài sản thực — bất động sản, trái phiếu, ERC-3643 |
| 08 | **[Machine Learning](docs/machine-learning/overview.mdx)** | ML cơ bản đến nâng cao — supervised, unsupervised, deep learning, MLOps |
| 09 | **[Python Data](docs/python-data/overview.mdx)** | Phân tích dữ liệu với Python — Pandas, NumPy, Matplotlib, thu thập data |
| 10 | **[Mobile](docs/mobile/overview.mdx)** | React Native (Expo) & Flutter — cross-platform mobile development |

Mỗi module có file `overview.mdx` tổng quan + các bài học chi tiết (xem [docs/](docs/)).

---

## 🚀 Bắt đầu nhanh

### Yêu cầu

- **Node.js 18+** (cho Mintlify CLI)
- **Git** để clone repo

### Chạy local

```bash
# 1. Clone repo
git clone https://github.com/<your-org>/claude-coding-courses.git
cd claude-coding-courses

# 2. Cài Mintlify CLI (lần đầu tiên)
npm i -g mint

# 3. Chạy dev server
mint dev
```

Sau đó mở trình duyệt tại **http://localhost:3000** để xem docs.

### Cập nhật CLI nếu gặp lỗi

```bash
mint update
```

---

## 🛠️ Cấu trúc repo

```
claude-coding-courses/
├── README.md                # File này
├── docs/                    # Toàn bộ nội dung tài liệu (MDX)
│   ├── index.mdx            # Trang chủ docs
│   ├── quickstart.mdx       # Quickstart page
│   ├── docs.json            # Cấu hình navigation, theme, branding
│   ├── CLAUDE.md            # Hướng dẫn cho Claude Code khi edit repo
│   ├── favicon.svg
│   ├── logo/                # Logo dark/light
│   ├── claude-code/         # Module 01
│   ├── agentic-ai/          # Module 02
│   ├── backend/             # Module 03
│   ├── api/                 # Module 04
│   ├── web3/                # Module 05
│   ├── blockchain/          # Module 06
│   ├── rwa/                 # Module 07
│   ├── machine-learning/    # Module 08
│   ├── python-data/         # Module 09
│   └── mobile/              # Module 10
└── .gitignore
```

> **Lưu ý:** Nội dung docs nằm trong thư mục con `docs/`, không phải ở root — đây là convention của Mintlify.

---

## ✍️ Cách đóng góp

### Thêm/sửa một trang

1. Tạo hoặc chỉnh sửa file `.mdx` trong thư mục module tương ứng.
2. Mỗi trang MDX cần **YAML frontmatter** ở đầu file:

   ```yaml
   ---
   title: "Tiêu đề trang"
   description: "Mô tả ngắn gọn cho SEO"
   icon: "book-open"   # icon từ Font Awesome / Heroicons
   ---
   ```

3. Nếu tạo trang mới, đăng ký nó trong [docs/docs.json](docs/docs.json) để nó xuất hiện trên navigation.

### Quy tắc viết

Được mô tả chi tiết trong [docs/CLAUDE.md](docs/CLAUDE.md). Tóm tắt:

- Dùng **giọng chủ động**, ngôi **bạn** (second person)
- Câu ngắn gọn — **một ý một câu**
- **Sentence case** cho heading (chỉ viết hoa chữ đầu)
- **Bold** cho UI elements: Click **Settings**
- `code` cho tên file, command, đường dẫn, code reference
- Dùng Mintlify components: `<Card>`, `<CardGroup>`, `<Tabs>`, `<Tab>`, `<Steps>`, `<Step>`, `<Callout>`, `<Tip>`, `<Warning>`, `<Check>`, `<Note>`

### Commit convention

Dùng conventional commits cho dễ theo dõi:

```bash
git commit -m "feat(claude-code): thêm bài học về MCP servers"
git commit -m "fix(backend): sửa lỗi typo trong auth.mdx"
git commit -m "docs: cập nhật README"
```

---

## 🎨 Theme & Branding

Site dùng **Mintlify theme `maple`** với bảng màu cam:

| Token | Value |
|-------|-------|
| Primary | `#FF6B35` |
| Light | `#FFB088` |
| Dark | `#C1390B` |

Thay đổi trong [docs/docs.json](docs/docs.json) → mục `colors`.

---

## 🔧 MCP Servers

Repo này có thể được edit qua **Mintlify MCP servers**:

- **Mintlify MCP:** `https://mcp.mintlify.com` — chỉnh sửa content & settings
- **Mintlify Docs MCP:** `https://www.mintlify.com/docs/mcp` — tra cứu cách dùng Mintlify

Cấu hình MCP trong `.mcp.json` của Claude Code để dùng.

---

## 📖 Tài liệu tham khảo

- [Mintlify Documentation](https://mintlify.com/docs)
- [MDX Syntax](https://mdxjs.com/)
- [Claude Code](https://claude.com/product/claude-code)
- [Claude Agent SDK](https://docs.anthropic.com/en/docs/agents-and-tools/claude-agent-sdk/overview)

---

## 📄 License

Nội dung docs được chia sẻ cho cộng đồng học tập. Vui lòng ghi nguồn khi sử dụng lại.

---

## 💬 Liên hệ & đóng góp

- Mở **Issue** nếu phát hiện lỗi nội dung hoặc muốn đề xuất bài học mới
- Tạo **Pull Request** để đóng góp trực tiếp
- Xem [CONTRIBUTING.md](docs/CLAUDE.md) (trong `docs/CLAUDE.md`) để biết style guide

---

**Happy learning & happy coding with Claude! 🚀**
