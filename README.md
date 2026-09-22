# qaset26-BrenoOliveira

# Execution Report: Git Branching and Pull Request Workflow

**Project 1:** QA Test Documentation Management (Settings Test Suite)  
**Author:** Breno Oliveira  
**Repository:** [https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira](https://github.com/BrenoCardosoOliveira/qaset26-BrenoOliveira)  
**Screenshot - sprint 1:** [https://docs.google.com/document/d/1qz92ufSb1jWB4yrTq6HcfvK1_dHzZiW65vTe23O_6ds/edit?usp=sharing]  
**Screenshot - sprint 2:** [https://docs.google.com/document/d/1qz92ufSb1jWB4yrTq6HcfvK1_dHzZiW65vTe23O_6ds/edit?usp=sharing]
---

## 📋 Project Description
**Sprint 1:**

This activity involved extending the project's test case repository by working with Git branches. A new feature branch was created to add test cases for the **Settings** functionality, followed by opening a Pull Request (PR) on GitHub and merging the changes into the `main` branch.

**Sprint 2:**

This activity involved extending the project's test case repository by working with Git branches. A new feature branch was created to add test cases for the **Settings** functionality, followed by opening a Pull Request (PR) on GitHub and merging the changes into the `main` branch.


---

## 🚀 Sprint 1: Steps Executed

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

