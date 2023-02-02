<img align="right" alt="GIF" color="green" src="https://github.com/abhisheknaiidu/abhisheknaiidu/blob/master/code.gif?raw=true" width="500" height="320" />

##  Full Stack Developer 🚀
- 🔭 I’m currently working on a large and special application.
- 🌱 I’m currently learning 😂
- 👯 I’m looking to collaborate with other Flutter developer 👩‍💻 and mobile app designers 🎨
- 🤔 I’m looking for help with Flutter front-end developer
- 🥅 2021 Goals: Developing an app to be heard in the world 🌎 and learning artificial intelligence 🤖
- ⚡ Fun fact: I love to swim 🏊‍♀️, play chess ♟, play basketball 🏀 and cycling 🚴‍♀️


### 📩 Connect with me:

<p align="center">
  <a href="https://twitter.com/iolardemartini" target="_blank">
    <img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white&color=071A2C" alt="Twitter"/>
  </a>
  <a href="https://www.linkedin.com/in/iolardemartini" target="_blank">
    <img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white&color=071A2C" alt="LinkedIn"/>
  </a>
  <a href="https://instagram.com/iolarjr" target="_blank">
    <img src="https://img.shields.io/badge/instagram-%23E4405F.svg?&style=for-the-badge&logo=instagram&logoColor=white&color=071A2C" alt="Instagram"/>
  </a>
  <a href="https://medium.com/@Demartini" target="_blank">
    <img src="https://img.shields.io/badge/medium-%2312100E.svg?&style=for-the-badge&logo=medium&logoColor=white&color=071A2C" alt="Medium"/>
  </a>
  <a href="https://www.facebook.com/iolardemartini" target="_blank">
    <img src="https://img.shields.io/badge/facebook-%231877F2.svg?&style=for-the-badge&logo=facebook&logoColor=white&color=071A2C" alt="Facebook"/>
  </a>
</p>
<br />



### 🔧 Languages and Tools:

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=java,spring,maven,hibernate,react,javascript,html,bootstrap,css,vscode,idea,visualstudio,github,postgres,mysql,mongodb,docker,aws,nodejs,jquery,githubactions,git,discord,powershell,kubernetes,ps,linux,wordpress,stackoverflow" />
  </a>
</p>
<br />


[vsCode]: https://code.visualstudio.com/
[git]: https://git-scm.com/
[github]: https://github.com/IbrahimTalha0


<br />
<br />

### :fire: My Stats :
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=your-github-username&layout=compact&theme=vision-friendly-dark)](https://github.com/Tekmily)
 [![GitHub Streak](http://github-readme-streak-stats.herokuapp.com?user=your-github-username&theme=dark&background=000000)](https://github.com/Tekmily)
 

### step 2. Create workflow file.

Create a workflow file like the one below.

* `.github/workflows/profile-3d.yml`

The schedule is set to start once a day.
Please correct the startup time to a convenient time.

```yaml:.github/workflows/profile-3d.yml
name: GitHub-Profile-3D-Contrib

on:
  schedule: # 03:00 JST == 18:00 UTC
    - cron: "0 18 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v3
      - uses: yoshi389111/github-profile-3d-contrib@0.7.1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: ${{ github.repository_owner }}
      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          git commit -m "generated"
          git push
```

Note: If you also want to include the private repository, register the "personal access token" in the repository and set it to GITHUB_TOKEN specified in the workflow file.

This will add the action to the repository.

#### Environment variables

* `GITHUB_TOKEN` : (required) access token
* `USERNAME` : (required) target user name (or specify with an argument).
* `MAX_REPOS` : (optional) max repositories, default 100 - since ver. 0.2.0
* `SETTING_JSON` : (optional) settings json file path. See `sample-settings/*.json` and `src/type.ts` in `yoshi389111/github-profile-3d-contrib` repository for details. - since ver. 0.6.0

### step 3. Manually launch the action

Launch the added action.

* `Actions` -> `GitHub-Profile-3D-Contrib` -> `Run workflow`

The profile image is generated with the following paths.

* `profile-3d-contrib/profile-green-animate.svg`
* `profile-3d-contrib/profile-green.svg`
* `profile-3d-contrib/profile-season-animate.svg`
* `profile-3d-contrib/profile-season.svg`
* `profile-3d-contrib/profile-south-season-animate.svg`
* `profile-3d-contrib/profile-south-season.svg`
* `profile-3d-contrib/profile-night-view.svg`
* `profile-3d-contrib/profile-night-green.svg`
* `profile-3d-contrib/profile-night-rainbow.svg`
* `profile-3d-contrib/profile-gitblock.svg`

example: night green version

![svg](https://raw.githubusercontent.com/yoshi389111/github-profile-3d-contrib/main/docs/demo/profile-night-green.svg)

example: night rainbow version

![svg](https://raw.githubusercontent.com/yoshi389111/github-profile-3d-contrib/main/docs/demo/profile-night-rainbow.svg)



