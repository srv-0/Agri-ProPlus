# Agri ProPlus 
**Agri ProPlus** is an extensive agriculture assistance tool designed to empower farmers with data-driven insights. It bridges the gap between modern technology and traditional farming by integrating real-time news, government scheme data, and AI-based crop recommendations.

---

##  Key Features

* **AI-Powered Crop Recommendation:** Implemented an LSTM-based Artificial Neural Network (ANN) model that predicts optimal crops based on soil and weather parameters with **98.48% accuracy**.
* **Information Hub:** Aggregates real-time farming news and educational content using **YouTube and News APIs**.
* **Government Schemes Tracker:** Features a custom **Python scraper** that extracts and updates the latest agricultural schemes data, serving it through a Node.js backend
* **Secure Authentication:** Robust user login and profile management powered by **Firebase**
* **Modern UI/UX:** A responsive frontend built with **React** and **Chakra UI** for an accessible user experience

---

##  Tech Stack

### Frontend
* ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) **React.js**
* ![Chakra UI](https://img.shields.io/badge/Chakra%20UI-319795?style=flat&logo=chakraui&logoColor=white) **Chakra UI**
* **Context API** (State Management)

### Backend & Database
* ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white) **Node.js & Express.js**
* ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white) **MongoDB**
* ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black) **Firebase Auth**

### AI & Data Science
* ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) **Python**
* **TensorFlow/Keras** (LSTM Model)
* **BeautifulSoup/Selenium** (Web Scraping)

---

##  Architecture

The application follows a decoupled architecture:
1.  **Data Ingestion:** Python scripts scrape government websites and fetch API data.
2.  **Processing:** Data is cleaned and stored in MongoDB. The ML model runs as a microservice/script to process inputs.
3.  **API Layer:** Node.js/Express serves this data to the frontend.
4.  **Client:** React consumes these APIs and presents actionable insights to the user.

---

##  Installation & Setup

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/saurav-singh-srv16/Agri-ProPlus.git](https://github.com/saurav-singh-srv16/Agri-ProPlus.git)
    cd Agri-ProPlus
    ```

2.  **Install Frontend Dependencies**
    ```bash
    cd client
    npm install
    ```

3.  **Install Backend Dependencies**
    ```bash
    cd server
    npm install
    ```

4.  **Set up Environment Variables**
    Create a `.env` file in the root directory and add:
    ```env
    MONGO_URI=your_mongodb_connection_string
    FIREBASE_API_KEY=your_firebase_key
    NEWS_API_KEY=your_news_api_key
    ```

5.  **Run the Application**
    ```bash
    # Run Backend
    cd server
    npm start

    # Run Frontend (in a new terminal)
    cd client
    npm start
    ```

---

##  Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

##  Author

**Saurav Singh**

* **LinkedIn:** [saurav-singh-srv16](https://linkedin.com/in/saurav-singh-srv16)
* **GitHub:** [saurav-singh-srv16](https://github.com/saurav-singh-srv16)
