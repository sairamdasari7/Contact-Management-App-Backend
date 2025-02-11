# Contact Management App Backend

This is a simple Contact Management API built using **Node.js** and **Express.js** with **MongoDB** as the database. The API allows users to perform CRUD operations on contacts, including adding, updating, deleting, and fetching contacts.

## Features

- **Create** a new contact
- **Retrieve** all contacts
- **Retrieve** a single contact by ID
- **Update** a contact by ID
- **Delete** a contact by ID
- **Validation** of user input using `express-validator`
- **Error Handling** with proper HTTP status codes
- **Search Contacts** by name or email *(Bonus Feature)*

## Technologies Used

- Node.js
- Express.js
- MongoDB with Mongoose
- Express Validator
- Dotenv
- Cors

## Project Structure

```
contact-management-backend/
│── node_modules/
│── src/
│   ├── config/
│   │   ├── db.js
│   ├── controllers/
│   │   ├── contactController.js
│   ├── middleware/
│   │   ├── errorMiddleware.js
│   ├── models/
│   │   ├── Contact.js
│   ├── routes/
│   │   ├── contactRoutes.js
│   ├── utils/
│   │   ├── validation.js
│── .env
│── .gitignore
│── package.json
│── README.md
│── server.js
```

## Installation & Setup

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community) (or use MongoDB Atlas)

### Clone the Repository

```sh
git clone https://github.com/yourusername/contact-management-backend.git
cd contact-management-backend
```

### Install Dependencies

```sh
npm install
```

### Configure Environment Variables

Create a `.env` file in the root directory and add:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

### Start the Server

For development mode with **nodemon**:

```sh
npm run dev
```

For production mode:

```sh
npm start
```

## API Endpoints

| Method | Endpoint       | Description            |
| ------ | -------------- | ---------------------- |
| GET    | /contacts      | Fetch all contacts     |
| GET    | /contacts/\:id | Fetch a single contact |
| POST   | /contacts      | Create a new contact   |
| PUT    | /contacts/\:id | Update a contact       |
| DELETE | /contacts/\:id | Delete a contact       |

### Example Contact JSON

```json
{
  "name": "John Doe",
  "email": "johndoe@example.com",
  "phone": "1234567890",
  "address": "123 Main St"
}
```

## Running Tests

To run tests (if implemented):

```sh
npm test
```

## Contributing

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push to the branch.
5. Submit a pull request.

## License

This project is licensed under the MIT License.

---

**Author:** Sairam
**GitHub:** https://github.com/sairamdasari7/Contact-Management-App-Backend.git

