# qaset26-BrenoOliveira

**Project:** Test Documentation Organization with Git  
**Author:** Breno Oliveira  
**Repository:** [https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira](https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira)  
**Screenshot - sprint 1:**[https://docs.google.com/document/d/1wZCein4vBYPWrOa-RVb9VGOpIgdgogSQ3Y2YpgXo_H8/edit?usp=sharing]  
**Screenshot - sprint 2:** [https://docs.google.com/document/d/1qz92ufSb1jWB4yrTq6HcfvK1_dHzZiW65vTe23O_6ds/edit?usp=sharing]
---

## 📋 Project Description

**Sprint 1:**

This task consists of organizing and versioning the project's test documentation (test cases for the *Sign Up* and *Sign In* features) using Git and GitHub.

**Sprint 2:**

This activity involved extending the project's test case repository by working with Git branches. A new feature branch was created to add test cases for the **Settings** functionality, followed by opening a Pull Request (PR) on GitHub and merging the changes into the `main` branch.


---

## 🚀 Sprint 1: Steps Executed

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

  ---

## 🚀 Sprint 2: Steps Executed

### Step 1: Create and Switch to a New Branch
Created and checked out a dedicated feature branch named `add_settings_test_suite`:

```bash
git checkout -b add_settings_test_suite
```

* **Branch Status:** Successfully switched from `main` to `add_settings_test_suite`.


> ![Step 1 - Branch Creation]
---

### Step 2: Create the `settings.md` File
Created the test specification file for settings functionality with the required test criteria:

```bash
cat << 'EOF' > settings.md
1. O link inserido atualiza a imagem do usuário
2. O usuário tem permissão para atualizar o nome
3. É permitido inserir 200 caracteres
4. O novo e-mail não é usado em registros anteriores
5. O comprimento do novo e-mail não deve ser inferior a 8 caracteres
6. Verificar erros gramaticais
7. Os símbolos da senha não devem ter menos de 8 caracteres
8. O usuário é desconectado e redirecionado para a página inicial como convidado
EOF
```


> ![Step 2 - Settings File Creation]

### Step 3: Stage and Commit the File
Added `settings.md` to the Git staging index and committed the changes with a descriptive message:

```bash
git add settings.md
git commit -m "Add settings test suite"
```


> ![Step 3 - Git Add and Commit]
---

### Step 4: Push Branch to Remote Repository
Published the feature branch `add_settings_test_suite` to the remote repository on GitHub:

```bash
git push -u origin add_settings_test_suite
```


> ![Step 4 - Git Push Branch]
---

### Step 5: Create a Pull Request (PR)
Opened a Pull Request on GitHub to request merging `add_settings_test_suite` into `main`:

* **Base Branch:** `main`
* **Compare Branch:** `add_settings_test_suite`
* **Title:** Add settings test suite


> ![Step 5 - Open Pull Request]

### Step 6: Merge Pull Request on GitHub
Approved and merged the Pull Request directly on GitHub's web interface:

1. Clicked **Merge pull request**.
2. Confirmed the merge action.
3. Status changed to **Merged** (purple tag).


> ![Step 6 - Merge Pull Request]
---

### Step 7: Update Local `main` Branch
Switched back to the local `main` branch and pulled the newly merged changes from GitHub:

```bash
git checkout main
git pull origin main
```

* **Verification:** Confirmed that `settings.md` is now present in the `main` branch locally.


> ![Step 7 - Git Checkout and Pull Main]

