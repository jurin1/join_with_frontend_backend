# Project Management Suite

This repository serves as a meta-project that integrates both the frontend and backend of the project management tool. The frontend (JavaScript) and backend (Python/Django) are managed as separate repositories and are included here as Git submodules.

## Cloning the Repository

To clone this repository along with its submodules, use the following command:

```sh
git clone --recurse-submodules https://github.com/your-username/project-management-suite.git
```

If you have already cloned the repository without submodules, initialize and update them with:

```sh
git submodule update --init --recursive
```

## Repository Structure

```
project-management-suite/
│── frontend/   # JavaScript frontend (submodule)
│── backend/    # Python/Django backend (submodule)
│── README.md   # Documentation
```

## Updating Submodules

To pull the latest changes from both submodules, run:

```sh
git submodule update --remote --merge
```

## Installation & Setup

Follow these steps to set up and run the application:

### Backend Setup (Python/Django)

1. Navigate to the backend directory:
   ```sh
   cd backend
   ```
2. Create a virtual environment and install dependencies:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Run migrations and start the Django server:
   ```sh
   python manage.py migrate
   python manage.py runserver
   ```

### Frontend Setup (JavaScript)

1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Start with Live Server from VSCode with Port 5500
   ```

## Additional Information

- Make sure both the frontend and backend are running for full functionality.
- Adjust API endpoints in the frontend if necessary.
- Contributions and improvements are welcome!



