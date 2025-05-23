<!--
// Fullscript:  <script src="https://gist.github.com/ryanlanciaux/3e29e75bd32efee9681c2ab85b99cc6f.js"></script>


// This app initially started from Flavio Copes analytics example
// but diverged quite a bit to generate images as well as track views
// https://flaviocopes.com/count-visits-static-site/

const express = require('express')
const app = express()

// no db - so global var to keep track of count
let counter = 0

function getCountImage(count) {
  // This is not the greatest way for generating an SVG but it'll do for now
  const countArray = count.toString().padStart(6, '0').split('');

  const parts = countArray.reduce((acc, next, index) => `
        ${acc}
        <rect id="Rectangle" fill="#000000" x="${index * 32}" y="0.5" width="29" height="29"></rect>
        <text id="0" font-family="Courier" font-size="24" font-weight="normal" fill="#00FF13">
            <tspan x="${index * 32 + 7}" y="22">${next}</tspan>
        </text>
`, '');
  
  return `<?xml version="1.0" encoding="UTF-8"?>
<svg width="189px" height="30px" viewBox="0 0 189 30" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <title>Count</title>
    <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
      ${parts}
    </g>
</svg>
`
}

// get the image
app.get('/count.svg', (req, res) => {
  counter++;
  
  // This helps with GitHub's image cache 
  //   see more: https://rushter.com/counter.svg
  res.set({
  'content-type': 'image/svg+xml',
  'cache-control': 'max-age=0, no-cache, no-store, must-revalidate'
  })
  
  // Send the generated SVG as the result
  res.send(getCountImage(counter));
})

const listener = app.listen(process.env.PORT, () => {
  console.log('Your app is listening on port ' + listener.address().port)
})

The following is a page hits counter which does not seem to be working (I keep it here, so it will continue to count just in case it starts working again):</br> 
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Ftzucker02%2F&count_bg=%238E6CC9&title_bg=%23191717&icon=github.svg&icon_color=%23E7E7E7&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)
-->


# [![Hits](https://hits.sh/github.com/tzucker02/hits.svg?style=plastis&color=blue&view=today-total&extraCount=512&label=Profile_Views:Today/Total)](https://hits.sh/github.com/tzucker02/hits/)
<!--
*Important to Note: For the hit counter, since it only starts counting once you add it to your profile, I have included the number of visitors who had already visited my profile at the time I added this counter.*


# ![](https://komarev.com/ghpvc/?username=tzucker02&color=blueviolet&style=plastic&base=300)

# You are Visitor #:  ![Visitor Count](https://profile-counter.glitch.me/tzucker02/count.svg)
-->
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSGlQXWqbQZJOfxE7MtMvIs9--VPgCp-dHPGA&s" height="20" width="20"></a>If you would like to customize your own GitHub profile page, I put together a set of [directions to help](https://github.com/tzucker02/How-to-customize-your-GitHub-profile/raw/main/profile_customization.pdf), which you are more than welcome to use. You should also check out this collection of [Github readme.md widgets](https://github.com/madushadhanushka/github-readme) and this [GitHub profile customization page](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/personalizing-your-profile)!  I have not tried [this GitHub page](https://docs.github.com/en/get-started/start-your-journey/setting-up-your-profile) yet, I will change this when I do. I have used a couple of the cards located [here](https://github.com/vn7n24fzkq/github-profile-summary-cards). You can see them at the bottom of this page. (NOTE: I have since updated my own GitHub profile README quite a bit.)  Some of the examples you may no longer see on this page, while others you may see are new and/or different.) I also "asked" claude.ai to generate how to customize your Github profile, and it came up with [this](https://github.com/tzucker02/customization/blob/main/README.md).

<!--
https://hits-app.vercel.app/hits?url=https://github.com/tzucker02/
-->
![github](https://github.com/user-attachments/assets/38faefe1-f176-4a18-9d24-1a1276988253)

<!--
<img src="https://widgetbite.com/banner?title=Tom%20Zucker-Scharff&subtitle=Data%20Analyst%2C%20Visualizer%20%26%20Dashboard%20developer&backgroundpalette=harvest&fontpalette=twilight&titletransform=none&subtitletransform=rotate" width=100% height=100%/>
-->

### <img src="https://cdn.iconscout.com/icon/free/png-256/free-switch-position-icon-download-in-svg-png-gif-file-formats--users-turnover-employee-replace-tiny-pack-user-interface-icons-3381102.png" height="30" width="30"></a> I follow back!  
(if my # of followers doesn't match my # of following, it just means I haven't checked it yet today)

Hi! I'm Tom.  I am a data analyst with a background in data visualization, technical writing, computer hardware, and software.  Welcome to my GitHub page!

- data analysis
- data visualization
- VBA programming
- dashboard development
- data reporting
- Python programming

## Projects

Check out my [portfolio and resources page](https://github.com/tzucker02/Projects/blob/main/README.md) where you can see different repos, projects, and data science resources (if you are looking for some [cheatsheets for Python](https://github.com/tzucker02/Projects/blob/main/Python%20Cheatsheets.md), [Python code snippets](https://github.com/tzucker02/PythonCode/blob/main/README.md),  [course links](https://github.com/tzucker02/course_material/blob/main/README.md), [datasets I am no longer using](https://github.com/tzucker02/Projects/blob/main/Dataset_Sources.md#datasets-I-am-no-longer-using), or [datasets links](https://github.com/tzucker02/Projects/blob/main/Dataset_Sources.md) try those links instead.) If you are interested in the Titanic dataset, there is a dictionary for the cleansed (PMLB) version [here](https://github.com/tzucker02/PythonCode/blob/main/Titanic_dictionary.md), and the original PMLB dictionary is [here](https://github.com/EpistasisLab/pmlb/blob/master/datasets/titanic/metadata.yaml).

## Some Tools

<!--  - Websites: [Resume]() , [Personal]() -->
- **Programming**: *Python* , Git, Visual Studio Code, VBA
- **Data Visualization**: Power BI, [Tableau](https://public.tableau.com/app/profile/thomaszuckerscharff/vizzes)
- **Reference Managers**: [EndNote](https://www.endnote.com) , [Zotero](https://www.zotero.org/tcszucker/library), Mendeley, F1000
- **Operating Systems**: Windows, MACOS, Linux, iOS, Android


<!-- Replace the fields below with the information requested. Remember to remove the encapsulating <> characters. -->

![Github Stats](https://github-readme-stats.vercel.app/api?username=tzucker02&count_private=true&show_icons=true&include_all_commits=true)

Here are a few of my projects:
<table>
  <thead align="center">
    <tr border: none;>
      <td><b>📘 Project</b></td>
      <td><b>⭐ Stars</b></td>
      <td><b>🤝 Forks</b></td>
      <td><b><img src="https://cdn.iconscout.com/icon/premium/png-256-thumb/git-commit-4241545-3517850.png" height="15" width="15">&nbsp;&nbsp;</b>    Commits</b></td>
      <td><b><img src="https://cdn-icons-png.freepik.com/256/15452/15452650.png?semt=ais_hybrid" height="15" width="15">      Contributors</b></td>
      <td><b><img src="https://cdn-icons-png.flaticon.com/256/3161/3161694.png" height="25" width="20">&nbsp;&nbsp;&nbsp;Traffic</b></td>
      <td><b><img src="https://raw.githubusercontent.com/pulsecron/pulse/HEAD/pulse.png" height="15" width="15">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Created </b></td>
    </tr>
  </thead>
  <body align="center">
    <div align="center">
    <tr>
      <td><a href="https://github.com/tzucker02/Projects" target="_blank"><b>Portfolio Page</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/Projects?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/Projects?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/Projects?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/Projects?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/Projects/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/Projects"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker02/Course_content_by_week" target="_blank"><b>Course by week</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/Course_content_by_week?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/Course_content_by_week?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/Course_content_by_week?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/Course_content_by_week?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/Course_content_by_week/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>  
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/Course_content_by_week"></td>
    <!--
      <td><img alt="Commits" src="https://img.shields.io/github/commits/tzucker02/Course_content_by_week?style=flat-square&labelColor=343b41"/></td>
    </tr>
    -->    
    <tr>
      <td><a href="https://github.com/tzucker02/course_material"><b>Course Material</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/course_material?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/course_material?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/course_material?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/course_material?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/course_material/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/course_material"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker02/Data-science-readings"><b>Data Science Readings</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/Data-science-readings?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/Data-science-readings?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/Data-science-readings?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/Data-science-readings?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/Data-science-readings/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/Data-science-readings"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker02/How-to-customize-your-GitHub-profile"><b>How to customize your GitHub profile</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/How-to-customize-your-GitHub-profile?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/How-to-customize-your-GitHub-profile?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/How-to-customize-your-GitHub-profile?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/How-to-customize-your-GitHub-profile?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/How-to-customize-your-GitHub-profile/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/How-to-customize-your-GitHub-profile"></td>
      <!--
      [insights for customization repo](https://github.com/tzucker02/How-to-customize-your-GitHub-profile/pulse)
      -->
    </tr>
<!--     <tr>
      <td><a href="https://github.com/tzucker02/dx699_milestone1"><b>DX699 Milestone 1</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/dx699_milestone1?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/dx699_milestone1?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/dx699_milestone1?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/dx699_milestone1?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/dx699_milestone1/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/dx699_milestone1"></td>
    </tr> -->
    <tr>
      <td><a href="https://github.com/tzucker02/Links"><b>Python Cheatsheets</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/Links?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/Links?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/Links?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/links?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/Links/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/Links"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker02/PythonCode"><b>Python Code Snippets</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/PythonCode?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/PythonCode?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/PythonCode?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/PythonCode?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/PythonCode/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/PythonCode"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker02/customization"><b>Python Code Snippets</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/customization?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/customization?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/customization?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/customization?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/customization/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/customization"></td>
    </tr>
    <tr>
      <td><a href="https://github.com/tzucker/scriptfromAJZS"><b>Aram Zucker-Scharff's brew script for setting up Python on a MAC</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/tzucker02/scriptfromAJZS?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/tzucker02/scriptfromAJZS?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Commits" src="https://img.shields.io/github/commit-activity/t/tzucker02/scriptfromAJZS?style=plastic"</td>
      <td><img alt="Contributors" src="https://img.shields.io/github/contributors/tzucker02/scriptfromAJZS?style=plastic&cacheSeconds=600"</td>
      <td><a href="https://github.com/tzucker02/scriptfromAJZS/graphs/traffic"><img alt="Traffic" src="https://img.shields.io/badge/Traffic-brown?style=plastic&cacheSeconds=600"</a></td>
      <td><img alt="GitHub Created At" src="https://img.shields.io/github/created-at/tzucker02/scriptfromAJZS"></td>
    </tr>
    <tr>
      <td cols=4><a href="https://public.tableau.com/app/profile/thomaszuckerscharff/vizzes" target="_blank"><b>My Tableau Public profile</b></a></td>
    </tr>   
    </div>
  </tbody>
</table>

<!-- other counters 
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Flinkedin.com%2Fin%2Fthomaszuckerscharff&count_bg=%2328262B&title_bg=%23055090&icon=linkedin.svg&icon_color=%23CEDCE9&title=LinkedIn&edge_flat=false)](https://hits.seeyoufarm.com)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Ffacebook.com%2Ftzuckerscharff&count_bg=%236D6A72&title_bg=%23468FCD&icon=facebook.svg&icon_color=%23FFFFFF&title=Facebook&edge_flat=false)](https://hits.seeyoufarm.com)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fdiscord.com%2Fchannels%2Ftomzuckerscharff_98477&count_bg=%236D6A72&title_bg=%23BCCAD7&icon=discord.svg&icon_color=%23101011&title=Discord&edge_flat=false)](https://hits.seeyoufarm.com)

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=tzucker02&theme=dark)](https://github.com/tzucker02/github-readme-streak-stats)

![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Ftzucker02&label=VISITORS&countColor=%23d9e3f0&style=plastic&labelStyle=upper)
-->

[![GitHub Streak](https://streak-stats.demolab.com?user=tzucker02)](https://git.io/streak-stats)

<!--

This graphic tends to show older statistics. To see the latest click the gitclear link in the lower right-hand corner.
<a href='https://www.gitclear.com/snap_changelogs/c721b538-61fd-4fc9-bf0e-7542e4f046f3' target='_blank'><img src='https://www.gitclear.com/snap_changelogs/c721b538-61fd-4fc9-bf0e-7542e4f046f3.png' /></a>


[GitHub insights for customization repo](https://github.com/tzucker02/How-to-customize-your-GitHub-profile/pulse)
-->
## More stats graphs
![Profile Summary Card](http://github-profile-summary-cards.vercel.app/api/cards/stats?username=tzucker02&theme=nord_dark)![Profile Card](http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=tzucker02&theme=nord_dark&utcOffset=-5)![Profile Summary Card](http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=tzucker02&theme=nord_dark)

<!--
Analytics.pageView = async function (payload) {
  if (payload.uid === 1) {
    return;
  }	
  local.pageViews += 1;
-->


## Connect with me

[![Static Badge](https://img.shields.io/badge/Thomas%20ZuckerScharff-blue?style=plastic&logo=facebook&logoColor=white&logoSize=auto&labelColor=Blue&color=blue&link=https%3A%2F%2Fwww.facebook.com%2Ftzuckerscharff)](https://www.facebook.com/tzuckerscharff)
[![Static Badge](https://img.shields.io/badge/Thomas%20ZuckerScharff-Black?style=plastic&logo=discord&logoColor=white&logoSize=auto&labelColor=black&color=black&link=https%3A%2F%2Fwww.discord.com%2Fchannels%2Ftomzuckerscharff_98477)](https://discord.com/channels/tomzuckerscharff)
[![Static Badge](https://img.shields.io/badge/IN_Thomas%20ZuckerScharff-blue?style=plastic&logoColor=white&link=https%3A%2F%2Fwww.linkedin.com%2Fin%2Fthomaszuckerscharff)](https://www.linkedin.com/in/thomaszuckerscharff)
[![Static Badge](https://img.shields.io/badge/Thomas%20ZuckerScharff-blue?style=plastic&logo=bluesky&logoColor=white&logoSize=auto&cacheSeconds=https%3A%2F%2Fbsky.app%2Fprofile%2Fnewyorkmyc-tzs.bsky.social)](https://bsky.app/profile/newyorkmyc-tzs.bsky.social)
[![Static Badge](https://img.shields.io/badge/Thomas%20ZuckerScharff-purple?style=plastic&logo=udemy&logoColor=white&link=https%3A%2F%2Fwww.udemy.com%2Fuser%2Fthomas-zucker-scharff%2F)](https://www.udemy.com/user/thomas-zucker-scharff)

<!--
## Hey 👋, This is Thomas Zucker-Scharff
[![Gmail Badge](https://img.shields.io/badge/-tzucker@bu.edu-c14438?style=flat&logo=Gmail&logoColor=white&link=mailto:tzucker@bu.edu)](mailto:tzucker@bu.edu) 
[![Linkedin Badge](https://img.shields.io/badge/-thomaszuckerscharff-0072b1?style=flat&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/thomaszuckerscharff/)](https://www.linkedin.com/in/thomaszuckerscharff/) [![Github Badge](https://img.shields.io/badge/-tzucker02-grey?style=flat&logo=github&logoColor=white&link=https://github.com/tzucker02/)](https://www.github.com/tzucker02/) [![Twitter Badge](https://img.shields.io/badge/-cyberdad-00acee?style=flat&logo=twitter&logoColor=white&link=https://twitter.com/cyberdad/)](https://www.twitter.com/cyberdad/) <p align='left'>I am a Data analyst, data visualizer and dashboard developer using Power BI and Tableau for visualizations and Python for analysis.</p>
## Some of my Github Stats
<p align=left> <img src=https://komarev.com/ghpvc/?username=tzucker02 alt=tzucker02 /> </p>

[![Github stats](https://github-readme-stats.vercel.app/api?username=tzucker02&show_icons=true&include_all_commits=true)](https://github.com/tzucker02/github-readme-stats)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=tzucker02&layout=compact)](https://github.com/tzucker02/github-readme-stats)
-->
