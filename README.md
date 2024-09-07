
---

# Sportan: Cricket Data Analytics Project

**Sportan** is a data analytics project aimed at creating the best 11 cricket team based on player performance records. The primary goal is to select a team that can score an average of at least 180 runs and defend 150 runs effectively.

## Project Goals

1. **Batting Performance**:
   - The selected team should be capable of scoring **at least 180 runs** on average.
2. **Bowling Performance**:
   - The team should be able to **defend 150 runs** on average.

## Team Composition Criteria

### 1. Openers:
- **Batting Average**: >30
- **Strike Rate**: >140
- **Innings Batted**: >3
- **Boundary Percentage**: >50%
- **Batting Position**: <4

### 2. Anchors/Middle Order:
- **Batting Average**: >40
- **Strike Rate**: >125
- **Innings Batted**: >3
- **Average Balls Faced**: >20
- **Boundary Percentage**: >25%
- **Batting Position**: >2

### 3. Finisher/Anchors:
- **Batting Average**: >25
- **Strike Rate**: >130
- **Innings Batted**: >3
- **Average Balls Faced**: >12
- **Batting Position**: >4
- **Innings Bowled**: >1

## Tech Stack

### Frontend:
- **HTML5**: For structuring the web interface.
- **CSS3**: For styling the frontend.
- **JavaScript**: To manage user interactions and dynamic elements.

### Backend:
- **Python**: The core programming language used for data processing, analysis, and team selection.
- **Flask/Django**: A backend web framework to handle API requests, route user inputs, and display results.
- **Pandas**: For data manipulation and analysis of player records.
- **NumPy**: To handle numerical operations and calculations for data analytics.
- **SQL (MySQL/PostgreSQL)**: For storing player records and query handling to fetch data based on criteria.

### Data Visualization:
- **Matplotlib/Seaborn**: To create graphs and visualize player statistics.
- **Plotly/Dash**: For interactive and real-time data visualization in web interfaces.

### Machine Learning (Optional Enhancements):
- **Scikit-learn**: To implement machine learning models for predicting team performance.
- **XGBoost/LightGBM**: For advanced predictive analytics on player performance.

### Deployment & Scalability:
- **Docker**: To containerize the project and ensure it runs consistently across different environments.
- **Cloud Services (AWS/GCP)**: To handle scalability and deployment for web access.

## Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/sportan.git
   cd sportan
   ```

2. **Set up the Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Setup Database**:
   - Use the `db_setup.sql` script to initialize the player records database.
   ```bash
   mysql -u <username> -p < db_setup.sql
   ```

5. **Run the Application**:
   ```bash
   python app.py
   ```

6. **Access the Web Application**:
   - Go to `http://localhost:5000` to access the Sportan web interface.

## Data Requirements

- Player data should include:
  - Batting statistics: average, strike rate, innings, boundaries, batting position.
  - Bowling statistics: innings bowled, runs conceded, economy rate.
  - Match statistics: team totals, match outcomes.

## How It Works

1. **Data Collection**: The system fetches player records from a database containing their performance statistics.
2. **Filtering & Team Selection**: Using the criteria provided for openers, middle-order, and finishers, the program filters out the best players.
3. **Team Formation**: The selected players are then placed into a "best 11" team.
4. **Analytics & Visualization**: Key metrics and graphs show how the selected team would perform based on historical data.

## Future Enhancements

- **Machine Learning Integration**: Use machine learning models to predict player performance and automate team selection.
- **Interactive Dashboards**: Enhance data visualization using Plotly/Dash for real-time updates.
- **User Customization**: Allow users to modify team selection criteria via the UI.

## Contributing

Feel free to open issues or pull requests if you want to contribute to this project.

---
