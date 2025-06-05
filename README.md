<!-- HTML-блок с розовыми CSS стилями -->
<div align="center">
  <style>
    :root {
      --primary: #ff69b4;
      --secondary: #ff1493;
      --dark-pink: #db7093;
      --light-pink: #ffb6c1;
      --text: #fff;
    }
    body {
      text-align: center;
      font-family: 'Arial', sans-serif;
    }
    .header-gradient {
      background: linear-gradient(90deg, #ff69b4, #ff1493, #ff6b81);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      font-weight: 800;
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    .badge {
      display: inline-flex;
      align-items: center;
      padding: 0.35rem 0.7rem;
      border-radius: 1rem;
      font-size: 0.9rem;
      font-weight: 600;
      margin: 0.25rem;
      background-color: rgba(255, 105, 180, 0.2);
      border: 1px solid var(--primary);
      color: var(--text);
    }
    .badge img {
      width: 16px;
      height: 16px;
      margin-right: 6px;
    }
    .section {
      background-color: rgba(219, 112, 147, 0.15);
      border-radius: 1rem;
      padding: 1.5rem;
      margin: 1.5rem auto;
      border: 1px solid var(--primary);
      max-width: 800px;
      text-align: center;
      transition: all 0.3s ease;
    }
    .section:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
      border-color: var(--secondary);
    }
    .section h2 {
      transition: all 0.3s ease;
    }
    .section:hover h2 {
      transform: scale(1.05);
      color: var(--secondary);
    }
    .project-card {
      background-color: rgba(255, 182, 193, 0.2);
      border-radius: 0.8rem;
      padding: 1.2rem;
      margin: 1rem auto;
      transition: all 0.3s ease;
      border-left: 4px solid var(--primary);
      max-width: 700px;
      text-align: center;
      transform: translateY(0);
      box-shadow: 0 4px 6px rgba(255, 105, 180, 0.1);
    }
    .project-card:hover {
      transform: translateY(-5px) scale(1.02);
      box-shadow: 0 12px 20px rgba(255, 105, 180, 0.2);
      background-color: rgba(255, 182, 193, 0.3);
      border-left: 4px solid var(--secondary);
    }
    .project-card h3 {
      transition: all 0.3s ease;
    }
    .project-card:hover h3 {
      color: var(--secondary);
      transform: scale(1.05);
    }
    .project-card a {
      display: inline-block;
      margin-top: 10px;
      padding: 8px 16px;
      border-radius: 20px;
      background: linear-gradient(45deg, var(--primary), var(--secondary));
      color: white;
      text-decoration: none;
      transition: all 0.3s ease;
    }
    .project-card a:hover {
      transform: translateY(-2px) scale(1.05);
      box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
      background: linear-gradient(45deg, var(--secondary), var(--primary));
    }
    .contact-grid {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 1rem;
      margin: 1.5rem 0;
    }
    .contact-card {
      background: rgba(255, 105, 180, 0.1);
      border-radius: 1rem;
      padding: 1rem 1.5rem;
      border: 1px solid var(--primary);
      transition: all 0.3s ease;
      min-width: 120px;
    }
    .contact-card:hover {
      transform: translateY(-5px) scale(1.05);
      background: rgba(255, 105, 180, 0.2);
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
      border-color: var(--secondary);
    }
    .contact-card img {
      width: 24px;
      height: 24px;
      margin-bottom: 0.5rem;
      transition: all 0.3s ease;
    }
    .contact-card:hover img {
      transform: scale(1.1) rotate(5deg);
    }
    h2 {
      color: var(--primary);
      border-bottom: 2px dashed var(--light-pink);
      padding-bottom: 0.5rem;
      display: inline-block;
      margin: 0 auto 1rem;
    }
    h3 {
      color: var(--secondary);
      margin: 0.5rem 0;
    }
    p {
      margin: 0.5rem 0;
      text-align: center;
    }
    a {
      color: var(--primary);
      text-decoration: none;
      font-weight: 600;
    }
    a:hover {
      text-decoration: underline;
      color: var(--secondary);
    }
    .about-section {
      margin: 20px 0;
      text-align: center;
    }
    .about-section p {
      margin-bottom: 15px;
      line-height: 1.6;
      font-size: 1.1em;
    }
    .tags-container {
      list-style: none;
      padding: 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
    }
    .tag-item {
      background: rgba(255, 105, 180, 0.1);
      padding: 8px 15px;
      border-radius: 15px;
      border: 1px solid var(--primary);
      transition: all 0.3s ease;
    }
    .tag-item:hover {
      transform: translateY(-5px) scale(1.05);
      background: rgba(255, 105, 180, 0.2);
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
      border-color: var(--secondary);
    }
    .highlight-text {
      color: var(--primary);
      font-weight: 600;
    }
    .tech-section {
      margin: 25px 0;
    }
    .tech-category {
      margin: 20px 0;
      text-align: center;
    }
    .tech-category h3 {
      color: var(--primary);
      margin-bottom: 15px;
      font-size: 1.2em;
      display: inline-block;
      border-bottom: 2px dashed var(--light-pink);
      padding-bottom: 5px;
    }
    .tech-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
      margin: 15px 0;
    }
    .tech-item {
      background: rgba(255, 105, 180, 0.1);
      padding: 10px 18px;
      border-radius: 15px;
      border: 1px solid var(--primary);
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .tech-item:hover {
      background: rgba(255, 105, 180, 0.2);
      transform: translateY(-5px) scale(1.05);
      box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
      border-color: var(--secondary);
    }
    .tech-item img {
      width: 20px;
      height: 20px;
    }
    .counter-big {
      transition: all 0.3s ease;
    }
    .counter-big:hover {
      transform: translateY(-5px) scale(1.02);
      filter: brightness(1.1);
    }
    .counter-big img {
      transition: all 0.3s ease;
      border-radius: 8px;
    }
    .counter-big:hover img {
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.3);
    }
    /* Анимация для GIF в секции аниме */
    .anime-gif {
      transition: all 0.3s ease;
      transform: translateY(0);
    }
    .anime-gif:hover {
      transform: translateY(-5px) scale(1.05);
      box-shadow: 0 12px 20px rgba(255, 105, 180, 0.3) !important;
    }
    /* Анимация для статистики GitHub */
    .github-stats {
      transition: all 0.3s ease;
    }
    .github-stats:hover {
      transform: translateY(-5px) scale(1.02);
      filter: brightness(1.05);
    }
    .github-stats img {
      transition: all 0.3s ease;
    }
    .github-stats:hover img {
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
    }
    .project-status {
      display: inline-block;
      padding: 4px 12px;
      border-radius: 12px;
      font-size: 0.9em;
      font-weight: 600;
      margin: 5px 0;
      transition: all 0.3s ease;
    }
    .status-development {
      background: rgba(255, 214, 0, 0.2);
      border: 1px solid #ffd600;
      color: #ffd600;
    }
    .status-active {
      background: rgba(76, 175, 80, 0.2);
      border: 1px solid #4CAF50;
      color: #4CAF50;
    }
    .status-completed {
      background: rgba(33, 150, 243, 0.2);
      border: 1px solid #2196F3;
      color: #2196F3;
    }
    .status-closed {
      background: rgba(244, 67, 54, 0.2);
      border: 1px solid #F44336;
      color: #F44336;
    }
    .project-card:hover .project-status {
      transform: scale(1.05);
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }
    .coming-soon {
      text-align: center;
      padding: 2rem;
      background: rgba(255, 105, 180, 0.1);
      border-radius: 1rem;
      border: 2px dashed var(--primary);
      margin: 1rem 0;
      transition: all 0.3s ease;
    }
    .coming-soon:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
      border-style: solid;
    }
    .coming-soon h3 {
      color: var(--primary);
      margin-bottom: 1rem;
    }
    .coming-soon p {
      color: var(--secondary);
      font-style: italic;
    }
  </style>

  <!-- Аниме-стилизованный заголовок -->
  <h1 class="header-gradient">Мингалеев Ильназ</h1>
  <div class="header-container" style="text-align: center;">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=24&pause=1000&color=FF69B4&width=450&lines=Fullstack+Developer;4%2B+года+опыта;Аниме+фанат;Люблю+розовый+цвет" alt="Typing SVG">
</div>

  <!-- Блок соцсетей -->
  <div class="contact-grid">
    <a href="https://github.com/dev-pegorino" class="contact-card">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg" alt="GitHub">
      <div>GitHub</div>
    </a>
    <a href="https://t.me/adaptation_channels" class="contact-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram">
      <div>Telegram</div>
    </a>
    <a href="https://vk.com/dev_ilnazik" class="contact-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/VK.com-logo.svg" alt="VK">
      <div>VKontakte</div>
    </a>
    <a href="https://youtube.com/@your_channel" class="contact-card">
      <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="YouTube">
      <div>YouTube</div>
    </a>
    <a href="https://profile.teamkaif.ru/Dev_Ilnaz" class="contact-card">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/chrome/chrome-original.svg" alt="Portfolio">
      <div>Портфолио</div>
    </a>
  </div>
</div>

<!-- Основное содержимое -->
<div class="section">
  <h2>🌸 Обо мне</h2>
  <p class="about-section">
    Привет! Я <span class="highlight-text">Мингалеев Ильназ</span> — fullstack-разработчик с более чем 4-летним опытом. ✨
  </p>

  <div class="about-section">
    <p>Специализируюсь на разработке:</p>
    <ul class="tags-container">
      <li class="tag-item">🎨 Современные веб-приложения с красивым UI</li>
      <li class="tag-item">🤖 Чат-боты (Telegram с mini-apps, ВК, Discord)</li>
      <li class="tag-item">💻 Мобильные и десктопные приложения</li>
      <li class="tag-item">🎥 Стрим-интеграции (чаты, алерты, донаты для Twitch и YouTube)</li>
    </ul>
  </div>

  <div class="about-section">
    <p>Моя среда разработки:</p>
    <ul class="tags-container">
      <li class="tag-item">🐧 Arch Linux</li>
      <li class="tag-item">✨ Hyprland</li>
      <li class="tag-item">🎨 KDE Plasma 6</li>
      <li class="tag-item">❌ Windows? Нет, спасибо!</li>
    </ul>
  </div>
</div>

<div class="section">
  <h2>💻 Технологии и инструменты</h2>
  
  <div class="tech-section">
    <div class="tech-category">
      <h3>🛠️ Инструменты разработки</h3>
      <div class="tech-grid">
        <div class="tech-item" title="Zed Editor">
          <img src="https://zed.dev/favicon.ico" alt="Zed">
          <span>Zed</span>
        </div>
        <div class="tech-item" title="Visual Studio Code">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" alt="VSCode">
          <span>VSCode</span>
        </div>
        <div class="tech-item" title="Android Studio">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original.svg" alt="Android Studio">
          <span>Android Studio</span>
        </div>
        <div class="tech-item" title="Git">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git">
          <span>Git</span>
        </div>
        <div class="tech-item" title="Figma">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/figma/figma-original.svg" alt="Figma">
          <span>Figma</span>
        </div>
        <div class="tech-item" title="ZSH + Oh My ZSH">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bash/bash-original.svg" alt="ZSH">
          <span>ZSH + Oh My ZSH</span>
        </div>
      </div>
    </div>

    <div class="tech-category">
      <h3>🗄️ Базы данных и ORM</h3>
      <div class="tech-grid">
        <div class="tech-item" title="SQLite + aiosqlite">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sqlite/sqlite-original.svg" alt="SQLite">
          <span>SQLite + aiosqlite</span>
        </div>
        <div class="tech-item" title="MySQL + aiomysql">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg" alt="MySQL">
          <span>MySQL + aiomysql</span>
        </div>
        <div class="tech-item" title="PostgreSQL">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="PostgreSQL">
          <span>PostgreSQL</span>
        </div>
        <div class="tech-item" title="SQLAlchemy">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sqlalchemy/sqlalchemy-original.svg" alt="SQLAlchemy">
          <span>SQLAlchemy</span>
        </div>
        <div class="tech-item" title="Alembic">
          <img src="https://raw.githubusercontent.com/alembic/alembic/main/docs/build/html/_static/alembic_logo.png" alt="Alembic">
          <span>Alembic</span>
        </div>
      </div>
    </div>

    <div class="tech-category">
      <h3>🚀 Языки и технологии</h3>
      <div class="tech-grid">
        <div class="tech-item" title="Python">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python">
          <span>Python</span>
        </div>
        <div class="tech-item" title="TypeScript">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="TypeScript">
          <span>TypeScript</span>
        </div>
        <div class="tech-item" title="JavaScript">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript">
          <span>JavaScript</span>
        </div>
        <div class="tech-item" title="React">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React">
          <span>React</span>
        </div>
        <div class="tech-item" title="Next.js">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg" alt="Next.js">
          <span>Next.js</span>
        </div>
        <div class="tech-item" title="Node.js">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" alt="Node.js">
          <span>Node.js</span>
        </div>
        <div class="tech-item" title="HTML5">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" alt="HTML5">
          <span>HTML5</span>
        </div>
        <div class="tech-item" title="CSS3">
          <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" alt="CSS3">
          <span>CSS3</span>
        </div>
      </div>
    </div>

  </div>
</div>

<div class="section">
  <h2>✨ Мои проекты</h2>
  
  <div class="coming-soon">
    <h3>🎨 Проекты в разработке</h3>
    <p>В данный момент все проекты находятся в приватных репозиториях.<br>
    Скоро здесь появятся интересные проекты! ✨</p>
  </div>

  <!-- 
  <div class="project-card">
    <div class="project-status status-active">Активен</div>
    <h3>🌸 Аниме-социальная сеть</h3>
    <p>Платформа для общения аниме-фанатов с рейтингами и рекомендациями</p>
    <p>Технологии: React, Node.js, MongoDB</p>
    <!-- Дата начала: 2023-08-15 -->

    <!-- Последнее обновление: 2024-03-20 -->
    <!-- Планируемые обновления:
      - Интеграция с MyAnimeList API
      - Система достижений
      - Мобильное приложение
    -->
    <!-- <a href="#">Посмотреть проект →</a>

  </div>
  
  <div class="project-card">
    <div class="project-status status-development">В разработке</div>
    <h3>💖 Кавайный To-Do лист</h3>
    <p>Милый планировщик задач с аниме-тематикой и достижениями</p>
    <p>Технологии: Next.js, TypeScript, Firebase</p>
    <!-- Дата начала: 2024-01-10 -->
    <!-- Текущая версия: 0.8.5 -->
    <!-- Планируемый релиз: 2024-04-15 -->
    <!-- Особенности:
      - Интеграция с календарём
      - Система наград и достижений
      - Тематические скины
      - Синхронизация между устройствами
    -->
    <!-- <a href="#">Посмотреть проект →</a>
  </div>

  <div class="project-card">
    <div class="project-status status-completed">Завершён</div>
    <h3>🤖 Telegram Mini App</h3>
    <p>Мини-приложение для просмотра аниме и манги</p>
    <p>Технологии: React, TypeScript, Telegram Bot API</p>
    <!-- Дата начала: 2023-11-01 -->
    <!-- Дата завершения: 2024-02-28 -->
    <!-- Достижения:
      - 10,000+ активных пользователей
      - Рейтинг 4.8/5
      - Интеграция с 5 крупными аниме-базами
    -->
    <!-- <a href="#">Посмотреть проект →</a>
  </div>

  <div class="project-card">
    <div class="project-status status-closed">Закрыт</div>
    <h3>🎮 Twitch Overlay</h3>
    <p>Аниме-стилизованные оверлеи для стримов</p>
    <p>Технологии: JavaScript, WebSocket, Canvas</p>
    <!-- Дата начала: 2023-05-01 -->
    <!-- Дата закрытия: 2023-12-31 -->
    <!-- Причина закрытия: Переход на новую версию Twitch API -->
    <!-- Достижения:
      - 5,000+ установок
      - Использовался на 100+ каналах
    -->
    <!-- <a href="#">Архив проекта →</a>
  </div> -->
</div>

<!-- Блок "Связаться со мной" -->
<div class="section">
  <h2>📩 Связаться со мной</h2>
  <div class="contact-grid">
    <a href="https://t.me/your_telegram" class="contact-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram">
      <div>Telegram</div>
      <small>@Dev_Kitty_Ilnazik2</small>
    </a>
	<a href="https://t.me/your_telegram" class="contact-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram">
      <div>Telegram (Твинк)</div>
      <small>@Dev_Ilnaz</small>
    </a>
    <a href="https://vk.com/dev_ilnazik" class="contact-card">
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/VK.com-logo.svg" alt="VK">
      <div>VKontakte</div>
      <small>@dev_ilnazik</small>
    </a>
    <a href="https://discord.com/users/Dev_Kitty193" class="contact-card">
      <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="Discord">
      <div>Discord</div>
      <small>Dev_Kitty193</small>
    </a>
  </div>
</div>

<!-- GitHub статистика с центрированием -->
<div class="section">
  <h2>📊 GitHub статистика</h2>
  <div class="github-stats" style="display: flex; flex-direction: column; align-items: center; gap: 20px;">
    <img src="https://github-readme-stats.vercel.app/api?username=dev-pegorino&show_icons=true&theme=radical&bg_color=ffb6c1&title_color=ff1493&text_color=fff&icon_color=db7093&border_color=ff69b4&hide_border=false" alt="GitHub Stats" style="width: 100%; max-width: 500px;">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=dev-pegorino&theme=radical&background=ffb6c1&ring=ff1493&fire=ff1493&currStreakNum=fff&sideNums=ff1493&currStreakLabel=ff1493&sideLabels=fff&dates=db7093&border=ff69b4&hide_border=false" alt="GitHub Streak" style="width: 100%; max-width: 500px;">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=dev-pegorino&layout=compact&theme=radical&bg_color=ffb6c1&title_color=ff1493&text_color=fff&border_color=ff69b4&hide_border=false" alt="Top Languages" style="width: 100%; max-width: 500px;">
  </div>
</div>

<!-- Аниме секция -->
<div class="section">
  <h2>🌸 Аниме</h2>
  <div style="display: flex; align-items: center; gap: 30px; flex-wrap: wrap; justify-content: center;">
    <div style="flex: 0 1 300px;">
      <img class="anime-gif" src="https://media.giphy.com/media/26tn33aiTi1jkl6H6/giphy.gif" alt="Anime GIF" style="border-radius: 1rem; width: 100%; border: 3px solid var(--primary); box-shadow: 0 0 15px var(--primary);">
    </div>
    <div style="flex: 1 1 300px; text-align: left; max-width: 400px;">
      <h3 style="color: var(--primary); margin: 15px 0; font-size: 1.3em;">✨ Мои любимые аниме</h3>
      <p style="margin: 15px 0; font-size: 1.1em; line-height: 1.6;">
        💫 Spy x Family<br>
        ✨ Становясь волшебницей<br>
        🎭 Фарфоровая кукла<br>
        🌟 Звёздное дитя
      </p>
    </div>
  </div>
</div>

<div align="center" style="margin: 2rem 0;">
  	<div class="counter-big">
    	<img src="https://komarev.com/ghpvc/?username=dev-pegorino&label=Профиль+посетили&color=ff69b4&style=for-the-badge&width=600" alt="Profile views">
	</div>
  	<p style="color: var(--primary); font-weight: 600;">Спасибо за визит! 💕</p>
  	<img src="https://media.giphy.com/media/3o7TKMt1VVNkHV2PaE/giphy.gif" width="150" style="border-radius: 50%; border: 3px solid var(--primary);">
</div>
