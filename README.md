# Full Project Setup Guide

This guide provides an overview of setting up, building, and running each component in the correct order, with links to the README files in each repository for detailed instructions.

## Project Overview

### Repositories

1. **Database Repositories**:
   - [Project Resource Database](https://github.com/W4153WASMCoder/ProjectResourceDB) - Includes DDL and dummy data in the `src` directory.
   - [User Database](https://github.com/W4153WASMCoder/UserDB) - Includes DDL and dummy data in the `src` directory.

2. **Service Repositories**:
   - [Project Resource Service](https://github.com/W4153WASMCoder/ProjectResource.git)
   - [User Authentication Service](https://github.com/W4153WASMCoder/user_authen_service.git)
   - [Application Service](https://github.com/W4153WASMCoder/ApplicationService.git)

3. **React Application Repository**:
   - [Application Frontend](https://github.com/W4153WASMCoder/Application)

## Setup Steps

### 1. Clone Repositories

Clone all repositories to your local environment.

```bash
mkdir wasmcoder
cd wasmcoder
# Clone databases
git clone https://github.com/W4153WASMCoder/ProjectResourceDB.git
git clone https://github.com/W4153WASMCoder/UserDB.git

# Clone services
git clone https://github.com/W4153WASMCoder/ProjectResource.git
git clone https://github.com/W4153WASMCoder/user_authen_service.git
git clone https://github.com/W4153WASMCoder/ApplicationService.git

# Clone frontend application
git clone https://github.com/W4153WASMCoder/Application.git
```

### 2. Set Up Databases

Each service requires its own SQL database. Follow the instructions in the respective database repositories to set up and initialize the databases.

- **[Project Resource Database Setup](https://github.com/W4153WASMCoder/ProjectResourceDB)**: See the README in the `ProjectResourceDB` repository for details on loading `create-table.sql` and `dummy-data.sql` into your SQL server.
- **[User Database Setup](https://github.com/W4153WASMCoder/UserDB)**: Refer to the README in the `UserDB` repository to load `create-table.sql` and `dummy-data.sql`.

### 3. Set Up and Run Services

After setting up the databases, refer to the README files in each service repository for detailed setup, environment configuration, and build instructions.

#### A. Project Resource Service

- Repository: [Project Resource Service](https://github.com/W4153WASMCoder/ProjectResource.git)
- Instructions: See the README for environment setup, dependencies, build, and run commands.

#### B. User Authentication Service

- Repository: [User Authentication Service](https://github.com/W4153WASMCoder/user_authen_service.git)
- Instructions: Refer to the README for configuration, building, and running the service.

#### C. Application Service

- Repository: [Application Service](https://github.com/W4153WASMCoder/ApplicationService.git)
- Instructions: Follow the README to configure environment variables, install dependencies, build, and run the service.

### 4. Set Up and Run the React Frontend

Once the backend services are up, you can set up and run the frontend.

- Repository: [Application Frontend](https://github.com/W4153WASMCoder/Application)
- Instructions: Refer to the README in the `Application` repository for environment setup, build, and run instructions.

### 5. Order of Operations

1. **Database Setup**: Set up and initialize both databases following their README instructions.
2. **Run Backend Services**:
   - Start the **Project Resource Service**.
   - Start the **User Authentication Service**.
   - Start the **Application Service** (which depends on both of the above services).
3. **Run Frontend**: Start the React frontend application after all backend services are up.

### 6. Access the Application

- **Frontend**: Visit the React application at `http://localhost:3000`.
- **Backend Services**:
  - Project Resource Service: `http://localhost:8080`
  - User Authentication Service: `http://localhost:8081`
  - Application Service: `http://localhost:8000`

---

Use this guide as an overview to set up the projects in the correct order, and refer to each repository’s README for detailed instructions. This ensures that all components are properly configured and interact seamlessly.
