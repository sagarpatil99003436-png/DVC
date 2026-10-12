DVC (Data Version Control) Learning Project
This project demonstrates how to use Git and DVC (Data Version Control) together to version control datasets used in Machine Learning projects.

📌 Project Objectives
Learn Git version control
Learn DVC data versioning
Track datasets separately from source code
Switch between different dataset versions
Integrate Git and DVC workflows
Push project to GitHub
🛠️ Technologies Used
Python
Git
GitHub
DVC
Virtual Environment (uv / venv)
📂 Project Structure
DVC/
│
├── Data/
│   ├── data.txt
│   └── data.txt.dvc
│
├── .dvc/
├── .gitignore
├── .dvcignore
└── README.md
🚀 Setup Instructions
Clone Repository
git clone https://github.com/sagarpatil99003436-png/DVC.git
cd DVC
Create Virtual Environment
Using UV:

uv venv
Activate Environment:

source .venv/Scripts/activate
Install DVC
uv pip install dvc
Verify Installation:

dvc version
📊 Initialize DVC
dvc init
Commit DVC Configuration:

git add .
git commit -m "Initialize DVC"
📁 Add Data to DVC
Create a file:

mkdir Data
echo "Version 1" > Data/data.txt
Track with DVC:

dvc add Data/data.txt
Generated file:

Data/data.txt.dvc
Commit metadata:

git add Data/data.txt.dvc .gitignore
git commit -m "Track data with DVC"
🔄 Version Data
Modify the file:

Version 2
Update DVC:

dvc add Data/data.txt
Commit changes:

git add Data/data.txt.dvc
git commit -m "Update data version"
⏪ Checkout Previous Data Version
Switch Git Commit:

git checkout <commit_id>
Restore data:

dvc checkout
DVC automatically restores the corresponding dataset version.

🌐 Push Project to GitHub
Add Remote:

git remote add origin https://github.com/sagarpatil99003436-png/DVC.git
Push Repository:

git push -u origin master
Future Pushes:

git push
✅ Commands Learned
Git
git init
git add .
git status
git commit -m "message"
git log --oneline
git checkout <commit>
git push
git pull
DVC
dvc init
dvc add Data/data.txt
dvc checkout
dvc status
dvc push
dvc pull
dvc version
🎯 Key Learnings
Git is used for source code versioning.
DVC is used for dataset versioning.
Large files should not be stored directly in Git.
DVC creates .dvc metadata files.
Dataset versions can be restored using dvc checkout.
Git and DVC together form the foundation of MLOps workflows.
📚 Future Learning Path
Git
 ↓
DVC
 ↓
MLflow
 ↓
Docker
 ↓
AWS S3
 ↓
AWS ETL Pipelines
 ↓
Kubeflow
 ↓
CI/CD (GitHub Actions/Jenkins)
 ↓
Kubernetes
 ↓
MLOps Engineer
👨‍💻 Author
Sagar Patil

GitHub: https://github.com/sagarpatil99003436-png
