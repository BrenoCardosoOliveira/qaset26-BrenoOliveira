# qaset26-BrenoOliveira

**Project:** Test Documentation Organization with Git  
**Author:** Breno Oliveira  
**Repository:** [https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira](https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira)  
**Screenshot:**[https://docs.google.com/document/d/1wZCein4vBYPWrOa-RVb9VGOpIgdgogSQ3Y2YpgXo_H8/edit?usp=sharing]
---

## 📋 Project Description

This task consists of organizing and versioning the project's test documentation (test cases for the *Sign Up* and *Sign In* features) using Git and GitHub.

---

## 🚀 Steps Executed

### Step 1 & 2: Git Installation & GitHub Account Creation
- Local environment setup with Git tool installation.
- Account registration and validation on GitHub.

> ![Step 1 and 2 - Git and GitHub]
---

### Step 3: Remote Repository Creation
- **Repository Name:** `qaset26-BrenoOliveira`
- **Visibility:** Public

> 
> ![Step 3 - GitHub Repository]
### Step 4 & 5: SSH Key Configuration & Git Identity
Configuring SSH key authentication on GitHub and establishing local credentials in the terminal:

```bash
git config --global user.name "Breno Oliveira"
git config --global user.email "YOUR_EMAIL_HERE"
```


> ![Step 4 and 5 - SSH Setup and Git Config]
---

### Step 6 & 7: Clone Repository Locally
Navigating to the home directory and cloning the remote repository via SSH:

```bash
cd ~
git clone git@github.com:BrenoCardosoOliveira/qaset26-BrenoOliveira.git
cd qaset26-BrenoOliveira
```


> ![Step 6 and 7 - Git Clone]
---

### Step 8: Creation of `sign_up.md` File
Creating and populating the registration test case criteria:

```bash
cat << 'EOF' > sign_up.md
1. O registro de um novo usuário permite três campos obrigatórios
2. O nome de usuário não deve estar vazio
3. A tecla “@” é obrigatória para entrar
4. A senha exclusiva é escolhida para o novo registro
5. Redirecionamento para a página de login
EOF
```


> ![Step 8 - Creating sign_up.md]

---

### Step 9: Creation of `sign_in.md` File
Creating and populating the login test case criteria:

```bash
cat << 'EOF' > sign_in.md
1. O usuário faz login no sistema com os dados inseridos durante o registro
2. Validação do e-mail que já está retido no banco de dados
3. A senha corresponde aos dados inseridos durante o registro
4. Redirecionamento para a página de registro
EOF
```

> ![Step 9 - Creating sign_in.md]

---

### Step 10: Initial Status Check (`git status`)
Running the repository status check:

```bash
git status
```

* **Current branch:** `main`
* **Untracked files (available for indexing):** `sign_up.md` and `sign_in.md`

> 
> ![Step 10 - Initial Git Status]
---

### Step 11 & 12: Adding Files to Index (Staging)
Adding all files to the staging area and confirming status:

```bash
git add .
git status
```

* **Result:** The files `sign_up.md` and `sign_in.md` moved to the staging area, displayed in green text.


> ![Step 11 and 12 - Git Add and Status]

---

### Step 13: Recording the Commit
Committing staged changes to local history:

```bash
git commit -m "Add sign_in and sign_up tests"
```


> ![Step 13 - Git Commit]

---

### Step 14: Pushing Changes to Remote Repository
Publishing commits from the local `main` branch to the GitHub repository:

```bash
git push origin main
```


> ![Step 14 - Git Push]

---

### Step 15: Confirmation on GitHub
Accessing the public repository via browser to validate updated files on the `main` branch:
- Link: [https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira](https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira)

