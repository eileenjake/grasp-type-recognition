<p align="center">
  <img src="https://example.com/uatservice.svg" alt="uatservice" width="200" height="200" />
</p>

<h1 align="center">uatservice</h1>

<h4 align="center">
  <a href="https://github.com/uatservice">Repository</a> |
  <a href="https://docs.run">Documentation</a> |
  <a href="https://discord.run">Discord</a> |
  <a href="https://roadmap.run">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/uatservice/actions"><img src="https://github.com/uatservice/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/uatservice"><img src="https://badge.fury.io/rb/uatservice.svg" alt="Version"></a>
  <a href="https://github.com/uatservice/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ developer toolkit for everyday tasks 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install uatservice
```

In your `Gemfile`:
```ruby
gem 'uatservice'
```

### Run uatservice

```bash
uatservice --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/uatservice.rb`:

```ruby
uatservice::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = uatservice::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'connectors' },
  { id: 2, title: 'kubernetes' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [connectors] and [kubernetes].

