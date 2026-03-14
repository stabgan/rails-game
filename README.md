# Rails Game

A simple JavaScript game served through a Ruby on Rails application — built as a learning exercise for the Rails MVC framework, DOM manipulation with vanilla JS, and database migrations.

## What It Does

Serves a single-page web app via Rails 5.2 with a `WelcomeController` that renders the game view. The project demonstrates the full Rails request lifecycle: routing → controller → view rendering, backed by PostgreSQL.

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| 💎 Framework | Ruby on Rails 5.2.3 |
| 🐘 Database | PostgreSQL |
| 🖥 Server | Puma 3.x |
| 🎨 Styles | SCSS (via sass-rails) |
| ⚡ JS | Vanilla JavaScript + Turbolinks |
| 🧪 Testing | Minitest + Capybara + Selenium |

## Prerequisites

- Ruby 2.4.1+
- PostgreSQL
- Bundler
- Node.js + Yarn (for asset pipeline)

## Setup

```bash
git clone https://github.com/stabgan/rails-game.git
cd rails-game
bundle install
rails db:create db:migrate
rails server
```

Then open [http://localhost:3000](http://localhost:3000).

## Project Structure

```
app/
├── controllers/   # WelcomeController (root route)
├── views/         # ERB templates + layouts
├── assets/
│   ├── javascripts/  # Application JS + Turbolinks
│   └── stylesheets/  # SCSS styles
config/
├── routes.rb      # root → welcome#index
├── database.yml   # PostgreSQL config
└── puma.rb        # Web server config
```

## ⚠️ Known Issues

- Ruby 2.4.1 is EOL — consider upgrading to Ruby 3.x with Rails 7 for production use
- `Gemfile.lock` may need regeneration after the `chromedriver-helper` → `webdrivers` migration — run `bundle install` to resolve
- CoffeeScript dependency (`coffee-rails`) is still in the Gemfile but no `.coffee` files remain; safe to remove if desired

## License

See [LICENSE](LICENSE) for details.
