# Auto GitHub Push & Repository Creation 🚀🔧📂

This project automates the process of committing, pushing changes to an existing GitHub repository, and creating a new repository using Python. 🖥️⚙️✅

## Prerequisites 🛠️📌🔍
Before using this script, ensure you have the following installed on your system:

- Python (>=3.6)
- Git
- `gitpython` and `PyGithub` Python packages
- A GitHub personal access token with repository permissions

## Setup 🔧⚙️📂
### 1. Clone the Repository (Optional) 🌍📥🖥️
If you haven't cloned the repository yet, you can do so using:

```sh
git clone https://github.com/AwaisSabit/Auto_Github1.git
```
### 2. Install Dependencies 📦⚡💡
Install the required Python packages using:

```python
pip install gitpython PyGithub
```

### 3. Set Up Environment Variables 🔐📌🖥️
To authenticate with GitHub, set up your personal access token as an environment variable:

On Windows (Command Prompt): 🖥️🔑📜

```sh 
set AUTO_PUSH_GITHUB_TOKEN=your_github_token
```

On macOS/Linux (Terminal): 🏗️🔑📜

```sh
export AUTO_PUSH_GITHUB_TOKEN=your_github_token
```

## Usage 🚀💾📜

### 1. Automate Git Commit and Push 📤📂✅
This function checks for changes, commits them, and pushes them to the GitHub repository. Run the script with:

```python
python script.py
```

## 2. Create a New GitHub Repository 🌐📁⚙️
To create a new repository, modify and uncomment the relevant section in the script:

```python
new_repo_url = create_github_repo('New_Repo_Name')
print(f"New repo URL: {new_repo_url}")
```
Then, run the script:

```python
python script.py
```

## Explanation of the Script 📜🖥️🔍

`push_to_github()` 🔄📥📤

- Checks if the repository is initialized, if not, it clones it.
- Pulls the latest changes from the remote repository.
- Adds and commits any changes if detected.
- Pushes the committed changes to GitHub.

`create_github_repo(repo_name)` 🔧🌍📦

- Authenticates using the GitHub token.
- Creates a new private repository on GitHub.
- Returns the repository clone URL.

## Troubleshooting 🛑⚠️🔍
- **Authentication Failed:** Ensure that your GitHub token has the correct permissions.
- **Repository Not Found:** Double-check your repository URL.
- **No Changes to Push:** Make sure there are actual file modifications in your repository before running the script.

## License 📜📝✔️
This project is open-source and available under the MIT License.

## Author ✍️👨‍💻📌
**Awais Sabit**


