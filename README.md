## Rate Repository App

This is a mobile application built with react native and expo and is used for rating GitHub repositories. Users can view reviewed repositories, sign up and sign in to create their own reviews. The application uses GraphQL as its backend.

### How to use the App

Just scan the QR code below with expo Go on your mobile phone

<img width="350" height="255" alt="QR code" src="https://github.com/user-attachments/assets/cd96f751-b280-4226-a9b3-3445b5c2967d" />

## 🚀 Key Features

- **Cursor-Based Infinite Scrolling:** Implemented paginated GraphQL queries with Apollo Client (`relayStylePagination`) to seamlessly load reviewed repositories and user reviews.
- **Search & Sorting:** Integrated real-time keyword filtering.
- **JWT Authentication Flow:** Built secure sign-in and sign-up workflows, persisting access tokens natively via `AsyncStorage`.
- **Validated Form Architecture:** Engineered declarative forms with **Formik** and **Yup** schema validation for user authentication and review submissions.

---

## 🛠️ Tech Stack

- **Mobile Core:** React Native, Expo, React Router Native
- **Data Layer:** GraphQL, Apollo Client
- **Forms & Validation:** Formik, Yup
- **Storage & Testing:** AsyncStorage, Jest, React Native Testing Library

---

## 📦 Local Setup (Frontend Client)

### Prerequisites

- [Node.js](https://nodejs.org) (LTS Version)
- [Expo Go](https://expo.dev) installed on your mobile device (or a local iOS/Android emulator)

### 1. Clone and Install

```bash
git clone https://github.com/chunogreg/rate-repository-app
cd rate-repository-app
npm install
```

### 2. Environment Configuration

Create a `.env` file in the root directory and configure your GraphQL endpoint:

```env
APOLLO_URI=http://your-server-ip:4000/graphql
```

### 3. Run the App

```bash
npx expo start
```

Scan the terminal QR code with **Expo Go**, or press `a` / `i` to open an emulator.

---

## 🧪 Running Tests

Run the Jest component and form validation test suite:

```bash
npm test
```
