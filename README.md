<p align="center"> 
               <img src="./images/Icon.svg" alt="Pacman Logo" width="80px" height="80px">
</p>
                            
                                                        EnergyX Fitness Application


                                              EPAM educational internship program (Spring 2025) 




![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### 📚 Table of Contents

- [📌 About the Project](#about-the-project)  
- [📁 Files Description](#files-description)  
- [🚀 Demo](#demo)  
- [🧰 Prerequisites](#prerequisites)  
- [🧪 Usage](#usage)  
- [🌟 Main Features](#main-features)  
- [🛠️ Installation](#installation)  
- [💻 Technologies Used](#technologies-used)  
- [🔌 API Integration](#api-integration)  
- [📜 License](#license)  
- [🙌 Acknowledgments](#acknowledgments)


![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### About the Project

**EnergyX** is a fitness application designed to bridge the gap between users and coaches. The app allows users to:
- Browse available workouts  
- Book sessions with coaches  
- Track workout progress  

Coaches can manage their workouts and monitor users’ activity. Whether you're a user looking for workouts or a coach overseeing clients, EnergyX provides an intuitive and powerful platform for your fitness goals.

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Files Description

##### Component Files
- **App.jsx** – Root component for routing and rendering main structure  
- **Coach.jsx** – Displays details of an individual coach  
- **Available.jsx** – Lists available workout slots for booking  
- **Content.jsx** – Handles workout date/time selection and coach filter  
- **Header.jsx** – Navigation bar and user profile  
- **SubHeader.jsx** – Secondary navigation or page titles  
- **ConfirmBookingModal.jsx** – Modal to confirm workout bookings  
- **LoginRequiredModal.jsx** – Modal to prompt login before restricted actions  
- **WorkoutCard.jsx** – Visual cards displaying workout info  

##### Page Files
- **Coaches.jsx** – List of all available coaches  
- **Home.jsx** – Application landing page  
- **Login.jsx** – User login form  
- **SignUp.jsx** – User registration form  
- **Workouts.jsx** – List of workouts with booking options  

##### Helper / Utility Files
- **auth-store.js** – Zustand store managing user auth state  
- **utils.js** – Utility functions (e.g., date formatting)  
- **Layout.jsx** – Page wrapper for consistent layout (e.g., header/footer)

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Demo

🔗 **Live Demo Link (if available)** – _Coming Soon_

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Prerequisites

Before running this project, make sure you have:

- IDE: VS Code / WebStorm / IntelliJ / Atom  
- Node.js (version 20+)  
- NPM  
- Git  

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Installation

```bash
1. Clone the repository:
   git clone https://git.epam.com/epm-edai/project-runs/run-6/team-3/serverless/fitness-app.git

2. Navigate to the project folder:
   cd gym-app

3. Install dependencies:
   npm install

4. Start the development server:
   npm run dev
```

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Usage

- **Home Page** – Acts as the landing page, introducing the app and guiding users to explore workouts and coaches  
  > _Scenario_: A new visitor opens the app and is welcomed with a clean homepage. From here, they can decide whether to explore workouts, view available coaches, or sign up to start booking sessions.

![alt text](images/Home.jpg)




- **Available Workouts** – Displays a list of workout slots filtered by date, time, and coach; users can book sessions here  
  > _Scenario_: After logging in, a user goes to the "Available Workouts" section, selects a preferred date and time, and books a cardio session with Coach Jane.

![alt text](images/Available.jpg)




- **Coaches Page** – Lists all registered coaches with brief bios; users can view profiles and select a preferred coach  
  > _Scenario_: A user who prefers strength training browses the "Coaches" page, filters by specialization, and clicks on Coach Mike's profile to see more details and book a session.

![alt text](images/Coaches.jpg)





- **Workouts Page** – Displays workout cards with booking options and statuses (pending, completed, feedback, etc.)  
  > _Scenario_: A logged-in user visits the "Workouts" page to track progress. They see one upcoming workout, one awaiting feedback, and one already completed.

![alt text](images/Workouts.jpg)





- **Coach Profile Page** – Each coach's profile includes personal info, available workouts, and downloadable certificates  
  > _Scenario_: On the "Coaches" page, a user selects a coach to view their profile, checks available dates, downloads a certificate, and proceeds to book a session.

![alt text](images/Coaches%20-%20Coach%20profile.jpg)



⚠️ *Note: The app currently does not support responsive design.*

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Main Features

- User Registration & Login – Create, sign in, and manage accounts  
- Workout Booking – Book sessions with coaches  
- Coach Profiles – Coaches manage their assigned workouts  
- Workout Tracking – Monitor user progress and assign new workouts  
- Workout Cards – Workouts grouped by status (scheduled, finished, waiting for feedback, cancelled)  
- Giving feedback and Grade for Trainer – Write, grade the session passed with coach  

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### Technologies Used

- React 6 – Component-based UI building  
- SCSS – Styling for clean and consistent design  
- NPM – Dependency management  
- Vite – Fast build and dev environment  
- Zustand – Lightweight state management  
- React Router – Page navigation  
- React Hooks – Functional component logic  
- Git – Version control  

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### API Integration

The EnergyX app communicates with a backend serverless API to handle:

#### Endpoints

**User Authentication**  
- `POST /auth/signup` – Register new users  
- `POST /auth/login` – Authenticate and receive token  
- `POST /auth/logout` – Clear session and logout  

**Workouts**  
- `GET /workouts` – Fetch available workouts  
- `POST /workouts/book` – Book a workout with a coach  

**Coaches**  
- `GET /coaches` – Retrieve all coaches  
- `GET /coach` – Get individual coach data  

**Feedbacks**  
- `GET /feedbacks` – Retrieve feedback  
- `POST /feedbacks` – Submit new feedback  

### Authentication

EnergyX uses **JWT (JSON Web Tokens)** for secure communication. Tokens are stored in the browser and attached to all protected requests.

### API Documentation

📘 *For full API documentation, check the [API Docs link (if available)]*.

![Rainbow Gradient Line](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### License

This project is licensed under the **MIT License** – see the LICENSE file for details.

### Acknowledgments

- React – For efficient and modular UI building  
- Zustand – For simple state management  
- Vite – For ultra-fast development  
- Ant Design – For elegant UI components  
