# CarbonEthics Recruitment Business Case: Fullstack Developer

Welcome to CarbonEthics!
CarbonEthics is an organization that aims to restore the climate balance through natural climate solutions with pioneers in blue carbon rehabilitation. When you conserve with CarbonEthics, you are not only creating positive environmental change, but you are also advancing social impact by directly enhancing the livelihoods of local community partners and thriving biodiversity. Starting as a not-for-profit organization, we are expanding to Impact Enterprise to provide more climate solutions through our net zero journey: Tree Planting, Carbon Consultancy, and Nature-based Carbon Projects.

## About this Repository
This repository contains the source code for a comprehensive e-commerce platform for digital products developed as part of the technical challenge for the Fullstack Developer position at CarbonEthics. The platform includes features for product management, user authentication, order processing, and administrative functionalities. The application is built using Django for the backend and React.js for the frontend, and it leverages Redux for state management, JWT for authentication and Amazon Web Service S3 for storage.

## Features of the App
- **Full featured shopping cart**
- **Product reviews and ratings**
- **Product pagination**
- **Top products carousel**
- **Product search feature**
- **User profile with order history**
- **Admin product management**
- **Admin user management**
- **Admin Order details page**
- **Mark orders as delivered option**
- **Checkout process (shipping, payment method, etc.)**
- **PayPal / credit card integration**

## Technology Stack
1. **Backend**: Django
2. **Frontend**: React.js
3. **State Management**: Redux
4. **Authentication**: JWT
5. **API Framework**: Django REST Framework
6. **Database Hosting**: Supabase
7. **Database**: PostgreSQL
8. **Storage:** AWS S3
9. **Cloud Platform:** Heroku

## Installation
### Backend Setup
1. Clone this repo.
    ```bash
    https://github.com/achmadardanip/ecommerce.git
    ```
2. Navigate to the project folder.
    ```bash
    cd ecommerce
    ```
3. Create a virtual environment.
    ```bash
    virtualenv myenv
    ```
4. Run virtual environment
   ```bash
   myenv\scripts\activate
   ```
5. Install the required packages.
    ```bash
    pip install -r requirements.txt
    ```
6. In the project folder, add a `.env` file with the following content:
    ```env
    DB_PASS=YOUR DATABASE PASSWORD
    DB_NAME=YOUR DATABASE NAME
    DB_USER=YOUR DATABASE USERNAME
    DB_HOST=YOUR DATABASE HOST
    DB_PORT=YOUR DATABASE PORT
    AWS_ACCESS_KEY_ID=YOUR AWS ACCESS KEY ID
    AWS_SECRET_ACCESS_KEY=YOUR AWS SECRET ACCESS KEY
    AWS_STORAGE_BUCKET_NAME=YOUR AWS BUCKET NAME
    ```
6. Run the server.
    ```bash
    python manage.py runserver
    ```

### Frontend Setup
1. Navigate to the frontend project folder.
    ```bash
    cd frontend
    ```
2. Install the required packages.
    ```bash
    npm install
    ```
3. In the frontend project folder, add a `.env` file with the following content:
    ```env
    SKIP_PREFLIGHT_CHECK=true
    ```

## API Endpoints
### Products
- `GET /api/products`
- `POST /api/products/create`
- `POST /api/products/upload`
- `POST /api/products/:id/reviews`
- `PUT /api/products/update/:id`
- `DELETE /api/products/delete/:id`

### Users
- `GET /api/users`
- `POST /api/users/login`
- `POST /api/users/register`
- `GET /api/users/profile`
- `PUT /api/users/profile/update`
- `GET /api/users/:id`
- `PUT /api/users/update/:id`
- `DELETE /api/users/delete/:id`

### Orders
- `POST /api/orders/add`
- `GET /api/orders/myorders`
- `PUT /api/orders/:id/deliver`
- `GET /api/orders/:id`
- `PUT /api/orders/:id/pay`

## Live Application
The application is deployed at [https://ecommerce-carbonethics-4fde1ef0b9b7.herokuapp.com/#/](https://ecommerce-carbonethics-4fde1ef0b9b7.herokuapp.com/#/)

Admin Access:
- **Email**: admin@achmadardani.me
- **Password**: admin

Test Case:
Credit Card
- Card Number 4032038847445073
- Expiry Date: 03/2026
- CVC: 576

## Any Assumptions or Decisions Made During Development

### Cloud Platform
- **Heroku**: Chosen for its ease of use, built-in deployment tools, and support for multiple languages. Compared to other options like AWS or Vercel, Heroku simplifies the deployment process and offers a free tier for small projects.

### Database Hosting
- **Supabase**: Selected for its seamless integration with PostgreSQL, real-time capabilities, and ease of setup. Supabase offers an open-source alternative to Firebase, providing similar features with more control over the database.

### State Management
- **Redux**: Used for its predictable state management, ease of debugging, and robust ecosystem. Compared to Context API or MobX, Redux provides a clearer structure for large applications, making state changes more predictable and easier to manage.

### Storage
- **AWS S3**: Chosen for its scalability, reliability, and integration with other AWS services. S3 offers cost-effective storage and high availability, making it a superior choice compared to traditional hosting or other cloud storage providers.

### Payment Integration
- **PayPal**: Selected for its widespread adoption, ease of integration, and secure payment processing. PayPal offers robust developer tools and APIs, making it easier to implement compared to other payment gateways like Stripe or Square.

### Authentication
- **JWT**: Used for its stateless nature, scalability, and ease of implementation. JWT allows for secure transmission of information between parties as a JSON object. Compared to traditional session-based authentication, JWT is more flexible and suitable for modern web applications.

## Known Limitations
- The user's current location on a map is not applied.
- No unit tests are implemented.

## Contact
If you have any trouble setting up the app, please contact me on WhatsApp at +6283877502520.
