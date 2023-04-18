# Python virtual environment and git setup guide

## Virtual Environment

### Inintial setup

1. Create a virtual environment from the root of the project folder

    ```sh
    python3 -m venv env
    ```

2. Activate the environment

    ```sh
    source env/bin/activate
    ```

    Typing `deactivate` in the shell will exit the environment

3. Update pip

    ```sh
    pip install --upgrade pip
    ```

4. Install packages need for the project

    ```sh
    pip install <package_name>
    ```

### Saving and Loading requirements

This is only needed if packages needs to be synced with e.g. collaborators or your future self

1. Save a formatted list of packages in a `requirements.txt` file

    ```sh
    pip freeze > requirements.txt
    ```

1. Install requirements from the list

    ```sh
    pip install -r requirements.txt
    ```

## Git

1. Create `.gitignore`

    ```sh
    echo env/ > .gitignore
    ```

2. Create git repo

    ```sh
    git init
    ````

3. Connect to remote repository

   ```sh
   git remote add origin <url_to_remote_git_repo>

## Linting

@todo

## Formatting

@todo
