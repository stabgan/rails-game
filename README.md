# Rails Learning Project

A basic Ruby on Rails web application created as a learning exercise to explore web development fundamentals and the Rails framework.

## 📖 About

This project was built as an educational exploration of Ruby on Rails, focusing on understanding MVC architecture, database migrations, and web application structure. While initially planned as a JavaScript game platform, it currently serves as a foundational Rails application demonstrating basic setup and configuration.

## 🎯 Learning Objectives

- **Ruby Language**: Syntax, conventions, and Ruby-specific features
- **Rails Framework**: MVC architecture, routing, and Rails conventions  
- **Database Integration**: ActiveRecord, migrations, and model relationships
- **Web Development**: HTTP request/response cycle and web application structure
- **Dependency Management**: Bundler, gem management, and Rails ecosystem

## 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| 💎 **Ruby 2.4.1** | Backend programming language |
| 🚂 **Rails 5.2.3** | Web application framework |
| 🐘 **PostgreSQL** | Database system |
| 🎨 **SCSS/Sass** | Stylesheet preprocessing |
| ☕ **CoffeeScript** | JavaScript preprocessing |
| 🔧 **Puma** | Web server |

## 🚀 Getting Started

### Prerequisites

- Ruby 2.4.1
- PostgreSQL
- Bundler gem

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/stabgan/rails-game.git
   cd rails-game
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Setup database**
   ```bash
   rails db:create
   rails db:migrate
   rails db:seed
   ```

4. **Start the server**
   ```bash
   rails server
   ```

5. **Visit the application**
   ```
   http://localhost:3000
   ```

## 📁 Project Structure

```
├── app/
│   ├── controllers/     # Request handling logic
│   ├── models/         # Data models and business logic
│   ├── views/          # HTML templates and layouts
│   └── assets/         # CSS, JavaScript, and images
├── config/             # Application configuration
├── db/                 # Database migrations and schema
└── test/               # Test suite
```

## ⚠️ Known Issues

- **Security Vulnerabilities**: Several gems have known security issues (see Dependabot alerts)
- **Outdated Dependencies**: Rails 5.2.3 and Ruby 2.4.1 are no longer supported
- **Minimal Functionality**: Currently displays only a basic "Hello World" page
- **Missing Game Logic**: Despite the name, no JavaScript game is implemented

## 🔄 Recommended Updates

For production use or continued development:

1. **Upgrade Ruby** to version 3.0+ 
2. **Upgrade Rails** to version 7.0+
3. **Update gems** to address security vulnerabilities
4. **Add comprehensive tests**
5. **Implement the planned game functionality**

## 📚 Learning Outcomes

This project provided hands-on experience with:
- Rails application structure and conventions
- MVC pattern implementation
- Database integration with ActiveRecord
- Asset pipeline and preprocessing
- Ruby ecosystem and tooling

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Created as a learning exercise to explore Ruby on Rails web development.*