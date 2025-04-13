## Project Structure
/project-root ├── backend/ # Spring Boot project └── frontend/ # React Native project

---
## Prerequisites

### Backend (Spring Boot)
- Java 17+
- Maven or Gradle

### Frontend (React Native)
- Node.js (v16+)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`) or React Native CLI
- Android emulator
---
## 🛠️ Setup Instructions

### Backend (Spring Boot)
```bash
# 1. Navigate to the backend directory
cd backend

# 2. Run with Maven
./mvnw spring-boot:run

# OR build and run the JAR
mvn clean package
java -jar target/Part1Application.jar
```
In frontend, open GetIP.js file from /frontend/services/GetIP.js and change the IP_ADDRESS variable
with your local IP address.

Then open MongoDB compass and create new connection with this string: mongodb://localhost:27017/CS458Project

After this create CS458 database and create two collections called Survey and User.

In User collection add example test user with add data-->import json or csv file-->choose the file from /frontend/tests/testUser.json or you can add your own test users with your mail and password

### Frontend (React Native)
```bash
# 1. Navigate to the frontend directory
cd frontend

# 2. Install dependencies
npm install

# 3. Start the development server
npx expo start
# or (if using native React Native CLI)
npx expo run:android
```

After these steps, you can run the appium test. Just before running tests, change the email and password input for each test javascript file located in /frontend/tests subfolders with the email and password in your database because our tests using login functionality coming from backend.


