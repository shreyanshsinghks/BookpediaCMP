# 📚 BookpediaCMP

![Compose Multiplatform](https://img.shields.io/badge/Compose--Multiplatform-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)

---

## 🌟 Overview

<img src="https://github.com/user-attachments/assets/ec2cfcb6-23a1-4ecc-a6b8-b7ee33adff6f" width="300"/>
<img src="https://github.com/user-attachments/assets/28633e19-442e-4400-b25c-2277b633c3d4" width="300"/>
<img src="https://github.com/user-attachments/assets/778e6f8a-7a9d-4875-b207-461832d630a8" width="300"/>

**BookpediaCMP** is a comprehensive book search and discovery application...


**BookpediaCMP** is a comprehensive book search and discovery application that allows users to explore books, view detailed information, and manage their reading preferences across multiple platforms. The app uses the **Open Library API** and follows **clean architecture patterns**.

---

## ✨ Features

### 🔍 **Advanced Book Search & Discovery**
- Real-time search by title, author, or keyword
- Access to millions of books via Open Library
- Smart filters and optimized API performance

### 📖 **Rich Book Information Display**
- Metadata, ratings, publication, and descriptions
- Author profiles and multilingual support
- Community ratings and full synopses

### 💾 **Offline-First Architecture**
- Room DB with smart caching
- Offline sync and favorite management
- Local reading history and saved data

### 🎨 **Modern UI/UX Design**
- Material Design 3 support
- Adaptive responsive layout
- Accessibility and theme switching

---

## 🏗️ Architecture & Technical Excellence

### Clean Architecture
- MVVM Pattern
- Repository + UseCase layers
- Koin for DI

### Tech Stack
- Kotlin Multiplatform
- Compose Multiplatform
- Ktor Client
- Room Database
- StateFlow + Coroutines

---

## 🛠️ Technology Stack

| Category      | Technology              | Purpose                            |
|---------------|--------------------------|-------------------------------------|
| **Core**      | Kotlin Multiplatform     | Shared code across platforms        |
|               | Compose Multiplatform    | Declarative UI                      |
|               | Coroutines & Flow        | Async programming                   |
| **Data**      | Room Database            | Local storage                       |
|               | Ktor Client              | API calls                           |
|               | Open Library API         | Book metadata source                |
| **Architecture** | Koin DI               | Dependency injection                |
|               | Navigation Compose       | Type-safe navigation                |
|               | ViewModel                | UI state handling                   |

---

## 📱 Platform Support

| Platform   | Status            | Features                                             |
|------------|-------------------|------------------------------------------------------|
| Android    | ✅ Fully Supported | Native experience with Material You                 |
| iOS        | ✅ Fully Supported | SwiftUI-friendly integration                        |
| Desktop    | ✅ Fully Supported | JVM-based for Windows, macOS, and Linux             |

---

## 📂 Project Structure

```
BookpediaCMP/
├── 📱 composeApp/
│   ├── src/
│   │   ├── 🌐 commonMain/
│   │   │   └── kotlin/com/plcoding/bookpedia/
│   │   │       ├── 🚀 app/
│   │   │       ├── 📚 book/
│   │   │       │   ├── 💾 data/
│   │   │       │   ├── 🏢 domain/
│   │   │       │   └── 🎨 presentation/
│   │   │       ├── ⚙️ core/
│   │   │       └── 💉 di/
│   │   ├── 🤖 androidMain/
│   │   ├── 🍎 iosMain/
│   │   └── 🖥️ desktopMain/
├── 📱 iosApp/
└── ⚙️ gradle/
```

---

## 🎯 Key Features Breakdown

### Search Experience
- Instant search with suggestions
- Search history
- Advanced filters

### Book Details
- High-res covers
- Author & related books
- Publication info and stats

### User Experience
- Smooth navigation
- Loading animations
- Error/retry handling
- Optimized performance

---

## 🚀 Getting Started

### Prerequisites
- Android Studio or IntelliJ (with KMP support)
- Xcode (for iOS)
- JDK 11+ (for Desktop)

### Quick Setup
```bash
# Clone the repository
git clone https://github.com/shreyanshsinghks/BookpediaCMP.git

# Navigate into the project
cd BookpediaCMP

# Run Android build
./gradlew :composeApp:installDebug

# Run Desktop app
./gradlew :composeApp:run

# iOS build (macOS + Xcode required)
./gradlew :composeApp:iosSimulatorArm64Test
```

---

## 🔧 Configuration

### Open Library API
- **Base URL**: `https://openlibrary.org/`
- `/search.json`
- `/works/{id}.json`
- `/covers/b/id/{id}-{size}.jpg`

### Room DB Schema
- Books metadata
- Favorites
- Cached content
- Search history

---

## 🎨 UI Components

- `BookCard`: Title + Cover + Author
- `SearchBar`: With filters
- `LoadingPulse`: Animated loading
- `EmptyState`: No results placeholder

### Theme System
- Material 3 Tokens
- Dynamic colors
- Scalable typography
- Uniform spacing

---

## 📊 Performance Features

- Lazy loading & pagination
- Image and data caching
- Indexed DB for faster queries
- Network optimizations

---

## 🧪 Testing Strategy

- Unit tests for logic
- Integration tests for API/db
- UI tests via Compose
- Platform-specific test coverage

---

## 🤝 Contributing

We welcome contributions!

### Guidelines
- Follow Kotlin conventions
- Keep code modular and clean
- Include tests
- Update docs

### Workflow
```bash
git checkout -b feature/your-feature
# Make changes
git commit -m "Add feature"
git push origin feature/your-feature
# Open a PR
```

---

## 📄 License

This project is available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- [Open Library](https://openlibrary.org/)
- [JetBrains](https://kotlinlang.org/)
- [Material Design](https://m3.material.io/)
- Contributors ❤️

---

**Built with ❤️ using Kotlin Multiplatform**

![GitHub Stars](https://img.shields.io/github/stars/shreyanshsinghks/BookpediaCMP?style=social)
![GitHub Forks](https://img.shields.io/github/forks/shreyanshsinghks/BookpediaCMP?style=social)
