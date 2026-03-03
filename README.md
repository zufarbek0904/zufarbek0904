# 👋 Hi there, I'm Zufarbek!

## 💻 About Me

* 🚀 Frontend Developer
* 🌱 Currently learning React & JavaScript
* 📍 From Uzbekistan
* 📫 How to reach me: [your_email@gmail.com](mailto:your_email@gmail.com)

---

## 🛠 Tech Stack

![HTML](https://img.shields.io/badge/HTML5-orange?style=for-the-badge\&logo=html5)
![CSS](https://img.shields.io/badge/CSS3-blue?style=for-the-badge\&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-yellow?style=for-the-badge\&logo=javascript)
![React](https://img.shields.io/badge/React-black?style=for-the-badge\&logo=react)

---

## 📊 GitHub Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=zufarbek0904\&show_icons=true\&theme=radical)

---

## 🐍 My Contributions

![Snake animation](https://raw.githubusercontent.com/zufarbek0904/zufarbek0904/output/github-contribution-grid-snake.svg)

name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: zufarbek0904
          outputs: dist/github-contribution-grid-snake.svg
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
          publish_branch: output
