# Flutter Weather App - Clean Architecture & TDD

A professional weather application built with **Flutter**, focusing on architectural scalability and reliability through **Uncle Bob's Clean Architecture** and **Test-Driven Development (TDD)**.

---

## 🏗️ Architecture
The project is divided into three main layers to ensure a separation of concerns and independent testability.

### 1. Domain Layer (Core)
* **Entities**: Pure business objects (e.g., `WeatherEntity`).
* **Use Cases**: Application-specific business rules.
* **Repositories**: Abstract interfaces defining data requirements.

### 2. Data Layer
* **Models**: Data Transfer Objects (DTOs) with JSON serialization.
* **Repositories**: Concrete implementations of domain interfaces.
* **Data Sources**: Remote (API) and Local (Persistence) logic.

### 3. Presentation Layer
* **State Management**: Implemented using **BLoC** for predictable state transitions.
* **UI**: Modular widgets and screens.

---

## 🧪 Testing Strategy
This project follows a strict **TDD (Red-Green-Refactor)** approach:

* **Unit Tests**: Focused on Use Cases and Repository implementations.
* **Mocking**: Utilizes `mockito` to isolate dependencies during testing.
* **Coverage**: Ensures models correctly map from API responses and handle exceptions.

---

## 🛠️ Tech Stack & Tools
* [cite_start]**Framework**: Flutter[cite: 6].
* **State Management**: BLoC.
* **External API**: OpenWeatherMap.
* **Functional Programming**: `dartz` for functional error handling (Either type).
* **HTTP Client**: `http` or `dio` for network requests.

---

## 🚀 Getting Started

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/KamalSaiVoodika/Flutter-Clean-Architecture-TDD-Weather-App.git](https://github.com/KamalSaiVoodika/Flutter-Clean-Architecture-TDD-Weather-App.git)
    ```
2.  **Install Dependencies:**
    ```bash
    flutter pub get
    ```
3.  **Run Tests:**
    ```bash
    flutter test
    ```
4.  **Launch the App:**
    ```bash
    flutter run
    ```

---

## 📝 Assumptions & Notes
* Requires a valid **OpenWeatherMap API Key**.
* Includes a `NetworkInfo` service to handle offline scenarios gracefully.
