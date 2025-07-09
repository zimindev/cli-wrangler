# 🎯 Wrangler — Cloudflare Workers CLI

**Wrangler** is the official command-line tool for developing, building, and deploying Cloudflare Workers. It simplifies managing Workers projects locally and publishing them to Cloudflare’s global network.

---

## ✅ Features

* Develop and test Workers locally with a dev server
* Build and bundle your Worker code easily
* Deploy your Worker to Cloudflare with one command
* Manage project configuration via `wrangler.toml`
* Authenticate and interact with your Cloudflare account
* Support for JavaScript, TypeScript, and WebAssembly Workers

---

## 📦 Installation

### Prerequisite: Install Node.js and npm

Make sure you have **Node.js** (version 12 or later) and **npm** installed.

---

### Install Wrangler globally

```bash
npm install -g wrangler
```

### Verify installation

```bash
wrangler --version
```

---

## 🚀 Basic Usage

### Authenticate with Cloudflare

```bash
wrangler login
```

This opens a browser to authorize Wrangler with your Cloudflare account.

---

### Initialize a new Worker project

```bash
wrangler init my-worker
cd my-worker
```

This creates a new Worker project with a `wrangler.toml` config file.

---

### Develop locally

```bash
wrangler dev
```

Runs your Worker in a local development server with live reload.

---

### Build the project

```bash
wrangler build
```

Bundles and prepares your Worker code for deployment.

---

### Publish to Cloudflare

```bash
wrangler publish
```

Deploys your Worker to Cloudflare's edge network.

---

## ⚙️ Common `wrangler.toml` example

```toml
name = "my-worker"
main = "index.js"
type = "javascript"
account_id = "your-account-id"
workers_dev = true
route = ""       # leave empty for workers.dev subdomain
zone_id = ""     # required if deploying to a custom domain route
```

---

## 🧩 Tips

* Use `wrangler whoami` to check current authenticated user
* Combine Wrangler with `npm` scripts for smoother development
* For advanced setups, use Webpack or ESBuild via Wrangler config
* Read Cloudflare docs for Workers API and advanced CLI commands

---

## 📚 More Info

* Official docs: [https://developers.cloudflare.com/workers/cli-wrangler/](https://developers.cloudflare.com/workers/cli-wrangler/)
* GitHub repo: [https://github.com/cloudflare/wrangler](https://github.com/cloudflare/wrangler)
* Cloudflare Workers examples: [https://developers.cloudflare.com/workers/examples/](https://developers.cloudflare.com/workers/examples/)
