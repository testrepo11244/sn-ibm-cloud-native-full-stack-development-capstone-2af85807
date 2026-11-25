# Car Dealership Full-Stack Application

## Repository Name
`car-dealership-fullstack`

## Project Name
**CarDealership** — Django + React Car Dealership Review Application

## Project Overview
CarDealership is a full-stack web application for browsing car dealerships, viewing dealer details and reviews, and submitting reviews for dealerships. The application uses a Django REST backend with a React frontend and includes user registration, login, logout, dealer filtering by state, car make/model lookup, sentiment analysis of review text, and role-based admin functionality.

## Key Features
- View all dealerships on the home page
- Filter dealerships by state
- View dealer details and dealer reviews
- Register a new user account
- Log in and log out
- Post a review for a dealership
- View sentiment analysis for review text
- Browse car makes and models
- Admin login and logout
- CI/CD pipeline using GitHub Actions
- Deployed Django application

## Technology Stack
- **Backend:** Django, Django REST Framework
- **Frontend:** React, JavaScript, HTML5, CSS3
- **Database:** SQLite for local development, PostgreSQL for deployment
- **Authentication:** Django session authentication
- **CI/CD:** GitHub Actions
- **Deployment:** IBM Cloud / Kubernetes-compatible deployment

## Repository Structure
```text
car-dealership-fullstack/
├── README.md
├── django_server
├── loginuser
├── logoutuser
├── getdealerreviews
├── getalldealers
├── getdealerbyid
├── getdealersbyState
├── getallcarmakes
├── analyzereview
├── CICD
├── deploymentURL
├── admin_login.png
├── admin_logout.png
├── get_dealers.png
├── get_dealers_loggedin.png
├── dealersbystate.png
├── dealer_id_reviews.png
├── dealership_review_submission.png
├── added_review.png
├── deployed_landingpage.png
├── deployed_loggedin.png
├── deployed_dealer_detail.png
├── deployed_add_review.png
└── server/
    ├── frontend/
    │   ├── static/
    │   │   ├── About.html
    │   │   └── Contact.html
    │   └── src/
    │       └── components/
    │           └── Register/
    │               └── Register.jsx
    └── djangoapp/
        ├── models.py
        ├── views.py
        ├── serializers.py
        └── urls.py
```

## Local Setup

### Backend
```bash
cd server
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

### Frontend
```bash
cd server/frontend
npm install
npm start
```

## API Endpoints
- `GET /djangoapp/get_dealers/` — Retrieve all dealers
- `GET /djangoapp/get_dealer/<dealer_id>/` — Retrieve dealer by ID
- `GET /djangoapp/get_dealers/<state>/` — Retrieve dealers by state
- `GET /djangoapp/reviews/dealer/<dealer_id>/` — Retrieve reviews for a dealer
- `GET /djangoapp/get_cars/` — Retrieve car makes and models
- `POST /djangoapp/register` — Register a new user
- `POST /djangoapp/login` — Log in a user
- `GET /djangoapp/logout` — Log out the current user
- `POST /djangoapp/add_review` — Add a dealer review
- `GET /djangoapp/analyze_review/<review_text>` — Analyze review sentiment

## Deployment
The deployed application URL is stored in the `deploymentURL` file.

## Author
IBM Full Stack Application Development Capstone Project