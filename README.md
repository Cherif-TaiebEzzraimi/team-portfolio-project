# 🧑‍💻 Team Portfolio Project

## 👥 Contributing Team Members

| Name | Role | Profile Page |
|------|------|--------------|
| **Cherif Taieb Ezzraimi** | Developer | [View Profile](profiles/cherif-taieb-ezzraimi.html) |
| **Ahmed Idris Brahmi** | Developer | [View Profile](profiles/ahmed-idris-brahmi.html) |
| **Aya Elatra Hezam** | Developer | [View Profile](profiles/aya-elatra-hezam.html) |
| **Dounia Saighi** | Developer | [View Profile](profiles/dounia-saighi.html) |
| **Rania Mir** | Developer | [View Profile](profiles/rania-mir.html) |

---

## 🌐 Deployed Website

🔗 **GitHub Pages Deployment:**  
[👉 Click here to visit the live website]()


---

## 🧠 Team Retrospective Analysis

### 🔹 Technical Challenge Analysis
During the collaborative development process, our team faced the most significant technical challenge in managing **merge conflicts across multiple feature branches**. Since each member worked on an individual profile page but also contributed to shared files like `index.html` and the `assets/` folder, Git often encountered overlapping changes that required manual conflict resolution. The difficulty primarily stemmed from simultaneous updates to the same lines of code, particularly when multiple team members added profile links in the same section of the index file.  
To address this, we established a **branching convention** (main → develop → feature/implement-name-profile) and enforced a **pre-merge verification** procedure. Each developer ensured they pulled the latest version of the `develop` branch before pushing changes. This improved synchronization and reduced redundant conflicts.

### 🔹 Merge Conflict Resolution Example
A notable merge conflict occurred in the `index.html` file when integrating multiple feature branches into `develop`. Each team member had added their own navigation link to their personal profile page, which caused overlapping modifications in the same section of the HTML file.  

To resolve this:  
1. We ran `git status` to locate the conflicted file (`index.html`).  
2. The conflict markers (`<<<<<<< HEAD`, `=======`, `>>>>>>>`) highlighted the different link versions contributed by each member.  
3. We manually reviewed and edited the file to include **all members’ profile links** in the navigation section, ensuring consistent formatting and correct paths.  
4. After confirming that all profile links worked properly in the browser, we finalized the resolution using:  
   ```bash
   git add index.html
   git commit -m "fix(index): resolve navigation link merge conflict and include all members"
   git push origin develop
