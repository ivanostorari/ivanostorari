
## Olá! Eu sou Ivan Wagner 👋

- 🔭 I'm currently working on Back End with C#...
  
- 🌱 I'm studying C#, .Net, Html, Css, JavaScript, Angular, Sql...
  
- 😄 Pronouns: He/Him...
  
<div align="center">
  <a href="https://github.com/ivanostorari">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=ivanostorari&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ivanostorari&layout=compact&langs_count=7&theme=dracula"/>
</div>

## Tecnologias que eu uso no meu dia a dia:    

<div style="display: inline_block">
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white" />

  <img align="center" alt="html5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  
  <img align="center" alt="css" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />

  <img align="center" alt="js" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" />

</div><br/> 

## Tecnologias em desenvolvimento:
  
<div style="display: inline_block">
    
  <img align="center" alt="ts" src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" />

  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" />
  
  <img align="center" alt="react" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" /> 
  
</div><br/>

## Tecnologias que ainda vou desenvolver:

<div style="display: inline_block">
 
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" />
  
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" />
  
</div><br/>

<div style="display: inline_block">
  
[![Youtube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@IvanOstorari-ue1cr/playlists)
[![linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ivan-wagner-ostorari-filho-11977134/?trk=opento_sprofile_goalscard)

</div><br/>
name: Generate Datas
on:
schedule: # execute every 12 hours
- cron: "* */12 * * *"
workflow_dispatch:
jobs:
build:
name: Jobs to update datas
runs-on: ubuntu-latest
steps:
# Snake Animation
- uses: Platane/snk@master
id: snake-gif
with:
github_user_name: DevBatista1
svg_out_path: dist/github-contribution-grid-snake.svg
- uses: crazy-max/ghaction-github-pages@v2.1.3
with:
target_branch: output
build_dir: dist
env:
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


