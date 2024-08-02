# expressPaymentGateway

## Express Payment Gateway Api

### Features

- [x] Auth with JWT and Auth with Role Permission
- [x] Advanced Login And Register
- [x] Refresh Token JWT
- [x] Confirmation Email Activation, Reset Password and more
- [x] Transfer Money To Another Users
- [x] Integration With Docker
- [x] Encryption Password
- [x] Build Automation Using Makefile
- [x] Any More


### Clone Repository

git clone https://github.com/nodeexcel/expressPaymentGateway.git

cd expressPaymentGateway

npm install

npm run dev


### Docker Command Makefile

- Docker Compose Up

  ```sh
  make cpup env=dev or make cpup env=prod
  ```

- Docker Compose Down

  ```sh
  make cpdown
  ```

- Dockerfile Build

  ```sh
  make dbd or make dbp
  ```

- Application Running
  ```sh
  make dev or make prod
  ```

### Express Container Default Environment


- ### Development

  - PG_HOST = db
  - PG_USERNAME = username
  - PG_PASSWORD = password
  - PG_DATABASE = payment
  - PG_PORT = 5432

### Postgres Container Default Environment

- POSTGRES_HOST=db
- POSTGRES_USER=username
- POSTGRES_PASSWORD=password
- POSTGRES_DB=payment

### Rest API Endpoint

| Name              | Endpoint                         | Method |
| ----------------- | -------------------------------- | ------ |
| **User**          |                                  |        |
| Register          | /api/v1/users/register           | POST   |
| Login             | /api/v1/users/login              | POST   |
| Activation        | /api/v1/users/activation/:id     | GET    |
| Resend            | /api/v1/users/resend-activation  | POST   |
| Forgot            | /api/v1/users/forgot-password    | POST   |
| Reset             | /api/v1/users/reset-password/:id | POST   |
| **admin**         |                                  |        |
| Create            | /api/v1/admins                   | POST   |
| Results           | /api/v1/admins                   | GET    |
| Result            | /api/v1/admins/:id               | GET    |
| Delete            | /api/v1/admins/:id               | DELETE |
| Update            | /api/v1/admins/:id               | PUT    |
| **Topup**         |                                  |        |
| Create            | /api/v1/topups                   | POST   |
| Results           | /api/v1/topups                   | GET    |
| Result            | /api/v1/topups/:id               | GET    |
| Delete            | /api/v1/topups/:id               | DELETE |
| Update            | /api/v1/topups/:id               | PUT    |
| **Withdraw**      |                                  |        |
| Create            | /api/v1/withdraw                 | POST   |
| Results           | /api/v1/withdraw                 | GET    |
| Result            | /api/v1/withdraw/:id             | GET    |
| Delete            | /api/v1/withdraw/:id             | DELETE |
| Update            | /api/v1/withdraw/:id             | PUT    |
| **Transfer**      |                                  |        |
| Create            | /api/v1/transfer                 | POST   |
| Results           | /api/v1/transfer                 | GET    |
| Result            | /api/v1/transfer/:id             | GET    |
| Delete            | /api/v1/transfer/:id             | DELETE |
| Update            | /api/v1/transfer/:id             | PUT    |
| **Saldo**         |                                  |        |
| Create            | /api/v1/saldo                    | POST   |
| Results           | /api/v1/saldo                    | GET    |
| Result            | /api/v1/saldo/:id                | GET    |
| Delete            | /api/v1/saldo/:id                | DELETE |
| Update            | /api/v1/saldo/:id                | PUT    |
| **Refresh Token** |                                  |        |
| Refresh           | /api/v1/refresh-token            | POST   |
