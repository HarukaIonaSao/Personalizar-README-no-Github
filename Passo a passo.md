 -  Use de base conforme seus conhecimentos em linguagens e frameworks e busque outras formas de personalizaçao. Olhe o código em Raw para ter acesso ao código base
 - Troque por seu nome de usuário para os stas dea sua conta aparecerem. Busquei inspiração para as outras personalizações em outros perfis, esse é o básico. Divirtam-se!! 
 
 Olá, eu sou (seu nome),
<div align="center"><br>
 

  <a href="https://github.com/harukaionasao">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=HarukaIonaSao&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=harukaionasao&layout=compact&langs_count=7&theme=dracula">
</div><br>
Aqui são os ícones das linguagens, no site DevIcon
<div style="display: inline_block"><br>

  <img align="center" alt="Roberta-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
    
  <img align="center" alt="Rafa-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
 
  <img align="center" alt="Rafa-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
 
  //Gif da sua preferência, será necessário configurar o Github Actions, link na aba "Links Úteis"<br>
 Para imagem, é só adicionar o caminho
 
  <img align="right" alt="Rafa-pic" height="150" style="border-radius:50px;" src="https://media.discordapp.net/attachments/639956127056134178/890373478988013628/Publicacoes_Instagram_1_1.png?width=676&height=676">
</div>
  
  ##
 //redes sociais
<div> 
  <a href="https://www.youtube.com/channel/UC_-uuuZbY0AAt9CViNzvc-Q" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
  <a href="https://www.instagram.com/robertaribeiro2827/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  
  <a href = "mailto:robertaribeiro004@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/roberta-ribeiro-b5521a4b/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
 
  ![Snake animation](https://github.com/rafaballerini/rafaballerini/blob/output/github-contribution-grid-snake.svg)
 
</div>


//para a cobrinha funcionar configure o actions dentro do repositorio especial de vocês

Vá em Generate data>Runworkflow>verde

Depois em actions crie um novo, apague o q estaá escrito e cole o codigo abaixo ,alterando seu username

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
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
