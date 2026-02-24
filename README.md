<h1 align="center">Hi 👋, I'm reza ahmadi</h1>
<h3 align="center">A passionate frontend developer from iran</h3>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=rezafrontend&label=Profile%20views&color=0e75b6&style=flat" alt="rezafrontend" /> </p>

<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=rezafrontend" alt="rezafrontend" /></a> </p>

<p align="left"> <a href="https://twitter.com/none" target="blank"><img src="https://img.shields.io/twitter/follow/none?logo=twitter&style=for-the-badge" alt="none" /></a> </p>

- 🔭 I’m currently working on [fatemh motamed](https://github.com/RezaFrontEnd/tahamtan)

- 🌱 I’m currently learning **html css javascript react.js next.js**

- 👨‍💻 All of my projects are available at [https://github.com/RezaFrontEnd](https://github.com/RezaFrontEnd)

- 📝 I regularly write articles on [none](none)

- 💬 Ask me about **html css javascript react.js next.js**

- 📫 How to reach me **reza.ahmadi350@gmail.com**

- 📄 Know about my experiences [none](none)

- ⚡ Fun fact **i think i am warrior in real life**

### Blogs posts
<!-- BLOG-POST-LIST:START -->
<!-- BLOG-POST-LIST:END -->

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://dev.to/rezafrontend.dev" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/devto.svg" alt="rezafrontend.dev" height="30" width="40" /></a>
<a href="https://twitter.com/none" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="none" height="30" width="40" /></a>
<a href="https://instagram.com/reza_ahmadi_warrior" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="reza_ahmadi_warrior" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=rezafrontend&show_icons=true&locale=en&layout=compact" alt="rezafrontend" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=rezafrontend&show_icons=true&locale=en" alt="rezafrontend" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=rezafrontend&" alt="rezafrontend" /></p>
import json
import random
from datetime import datetime, timedelta

# ساخت داده برای یک سال (2025)
start_date = datetime(2025, 1, 1)
data = []

for i in range(365):
    date = start_date + timedelta(days=i)
    # روزهای جمعه و شنبه کمی پررنگ‌تر (کامیت بیشتر)
    if date.weekday() in [5, 6]:  # 5=جمعه، 6=شنبه
        count = random.randint(3, 15)
    else:
        count = random.randint(0, 8)
    data.append({"date": date.strftime("%Y-%m-%d"), "count": count})

# ذخیره JSON
with open("github_contributions_2025.json", "w") as f:
    json.dump(data, f, indent=2)

print("فایل github_contributions_2025.json ساخته شد!")
