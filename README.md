# Hospital Food Management System

## Overview
The Hospital Food Management System is a comprehensive application designed to streamline and manage the dietary requirements and food delivery services within a hospital. It provides distinct functionalities for hospital food managers, pantry staff, and delivery personnel, ensuring efficient meal preparation, dietary customization, and timely delivery to patients.

---

## Key Features

### 1. Hospital Food Manager Functionality
- **Role**: Hospital Food Management Admin.
- **Patient Management**:
  - Add, edit, and delete patient details.
  - Patient attributes include:
    - Name
    - Diseases and medical conditions
    - Allergies
    - Room Number, Bed Number, and Floor Number
    - Age and Gender
    - Contact Information
    - Emergency Contact
    - Additional details as required.
- **Diet Chart Management**:
  - Create and assign meal plans for Morning, Evening, and Night.
  - Specify meal ingredients and instructions (e.g., "no salt," "low sugar," etc.).
  - Update or modify diet plans as needed.
- **Pantry Management**:
  - Maintain pantry details including:
    - Staff names
    - Contact information
    - Pantry locations.
  - Assign food preparation and delivery tasks to pantry staff.
- **Meal Tracking**:
  - Monitor the preparation status of each meal.
  - Track delivery statuses for Morning, Evening, and Night meals.
  - Receive alerts for delays or preparation issues.

### 2. Inner Pantry Functionality
- **Task Management**:
  - View assigned meal preparation tasks from the Hospital Food Manager.
  - Update preparation statuses for individual meals.
- **Delivery Personnel Management**:
  - Add and maintain details for delivery personnel (e.g., Name, Contact Info).
  - Assign specific meal boxes for delivery.
- **Meal Delivery Tracking**:
  - Include details of each meal box:
    - Patient information
    - Room number
    - Diet chart details.
  - Update delivery statuses in real-time, visible to both the Hospital Food Manager and Pantry Staff.

### 3. Delivery Personnel Functionality
- **Delivery Management**:
  - Login to the portal to view assigned meal boxes with patient and delivery details.
  - Mark deliveries as "Done" upon successful delivery to patient rooms.
  - Add timestamps and optional delivery notes for record-keeping.

### 4. Dashboards
- **Hospital Food Manager Dashboard**:
  - Track all food deliveries in real-time.
  - View comprehensive patient details and diet charts.
  - Monitor pantry performance and meal delivery statuses.
  - Receive notifications for delays, preparation issues, or missed deliveries.
- **Inner Pantry Dashboard**:
  - View and manage all meal preparation and delivery tasks.
  - Monitor delivery personnel and assigned meal boxes.
  - Update delivery statuses and track progress in real-time.

---

## Technologies Used

### Backend:
- **Preferred**: NestJS, Prisma, PostgreSQL/MongoDB for scalable and efficient backend services.
- **Other Options**: Node.js, Express.js.

### Frontend:
- **Preferred**: React.js, Next.js, or Vite.js for a dynamic, responsive user interface.
- **Styling**: Tailwind CSS, Material UI for clean and consistent design.

### Deployment:
- **Backend**: Render, Railway for reliable and free hosting with database support.
- **Frontend**: Vercel for seamless static hosting and fast deployment.

---

## API Endpoints
### Authentication
- `POST /auth/login`: User login.
- `POST /auth/register`: User registration.

### Patient Management
- `GET /patients`: Fetch all patients.
- `POST /patients`: Add a new patient.
- `PUT /patients/:id`: Update patient details.
- `DELETE /patients/:id`: Remove a patient.

### Diet Charts
- `GET /diet-charts`: Fetch all diet charts.
- `POST /diet-charts`: Create a new diet chart.
- `PUT /diet-charts/:id`: Update an existing diet chart.
- `DELETE /diet-charts/:id`: Delete a diet chart.

### Delivery Management
- `GET /deliveries`: View all deliveries.
- `POST /deliveries`: Assign a delivery.
- `PUT /deliveries/:id`: Update delivery status.

---

## Database Schema
- **Users**:
  - Stores user credentials and roles (Admin, Pantry Staff, Delivery Personnel).
- **Patients**:
  - Stores patient details such as name, age, medical conditions, allergies, and contact info.
- **DietCharts**:
  - Stores meal plan details including ingredients and specific instructions.
- **PantryStaff**:
  - Stores details of pantry staff and their assigned tasks.
- **Deliveries**:
  - Tracks delivery statuses, timestamps, and personnel assignments.

---

## Installation

### Prerequisites
- Node.js
- PostgreSQL/MongoDB
- Git

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-link>
   cd hospital-food-management
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add database and authentication secrets.
     ```
     DATABASE_URL=your_database_url
     JWT_SECRET=your_jwt_secret
     ```

4. Run the application:
   - **Backend**:
     ```bash
     npm run start:backend
     ```
   - **Frontend**:
     ```bash
     npm run start:frontend
     ```

5. Access the application:
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`

---

## Deployment
- **Backend**: Deploy on Render or Railway for reliable backend hosting with built-in database support.
- **Frontend**: Deploy on Vercel for fast, efficient, and free static hosting.

---

## Contributing
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Create a pull request.

---

## License
This project is licensed under the MIT License.

---

## Contact
For any queries or issues, please contact:
- **Email**: support@example.com
- **GitHub**: [Your GitHub Profile](https://github.com/your-profile)

---

## Links
- **GitHub Repository**: [Repository Link](#)
- **Deployed App**: [App Link](#)
