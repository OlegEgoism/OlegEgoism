<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Oleg Pustovalov | Tech Stack</title>
  <style>
    :root {
      --bg-primary: #f8f9fa;
      --card-bg: #ffffff;
      --text-primary: #2d3748;
      --text-secondary: #4a5568;
      --accent: #4299e1;
      --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
      --shadow-hover: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
      --border-radius: 12px;
      --transition: all 0.3s ease;
    }

    @media (prefers-color-scheme: dark) {
      :root {
        --bg-primary: #1a202c;
        --card-bg: #2d3748;
        --text-primary: #f7fafc;
        --text-secondary: #cbd5e0;
        --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.3);
      }
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
      background: var(--bg-primary);
      color: var(--text-primary);
      line-height: 1.6;
      padding: 2rem;
      transition: var(--transition);
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
    }

    /* Header Styles */
    .header {
      text-align: center;
      padding: 2rem 0 3rem;
      animation: fadeInDown 0.6s ease;
    }

    .header h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .header p {
      color: var(--text-secondary);
      font-size: 1.1rem;
      margin: 0.5rem 0;
    }

    .contacts {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin-top: 1rem;
      flex-wrap: wrap;
    }

    .contact-link {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      color: var(--accent);
      text-decoration: none;
      font-weight: 500;
      transition: var(--transition);
      padding: 0.5rem 1rem;
      border-radius: 8px;
    }

    .contact-link:hover {
      background: var(--accent);
      color: white;
      transform: translateY(-2px);
    }

    /* Section Styles */
    .section {
      margin-bottom: 3rem;
      animation: fadeInUp 0.6s ease;
    }

    .section-title {
      font-size: 1.8rem;
      margin-bottom: 1.5rem;
      padding-bottom: 0.75rem;
      border-bottom: 3px solid var(--accent);
      display: inline-block;
    }

    /* Tech Grid */
    .tech-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
      gap: 1.25rem;
    }

    .tech-card {
      background: var(--card-bg);
      border-radius: var(--border-radius);
      padding: 1.25rem 1rem;
      text-align: center;
      box-shadow: var(--shadow);
      transition: var(--transition);
      cursor: default;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 0.75rem;
    }

    .tech-card:hover {
      transform: translateY(-6px);
      box-shadow: var(--shadow-hover);
    }

    .tech-card img {
      width: 64px;
      height: 64px;
      object-fit: contain;
      transition: var(--transition);
      filter: grayscale(10%);
    }

    .tech-card:hover img {
      filter: grayscale(0%);
      transform: scale(1.1);
    }

    .tech-card span {
      font-weight: 500;
      font-size: 0.95rem;
      color: var(--text-primary);
    }

    /* Category Section */
    .category {
      margin-bottom: 2.5rem;
    }

    .category-title {
      font-size: 1.3rem;
      color: var(--text-secondary);
      margin-bottom: 1rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .category-title::before {
      content: '';
      width: 4px;
      height: 20px;
      background: var(--accent);
      border-radius: 2px;
    }

    /* Animations */
    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* Responsive */
    @media (max-width: 768px) {
      body { padding: 1rem; }
      .header h1 { font-size: 2rem; }
      .tech-grid { grid-template-columns: repeat(auto-fill, minmax(110px, 1fr)); gap: 1rem; }
      .tech-card { padding: 1rem 0.75rem; }
      .tech-card img { width: 56px; height: 56px; }
    }

    @media (max-width: 480px) {
      .tech-grid { grid-template-columns: repeat(3, 1fr); }
      .contacts { flex-direction: column; align-items: center; }
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Header -->
    <header class="header">
      <h1>👋 Привет! Я Олег Пустовалов</h1>
      <p>Fullstack Developer & Data Engineer</p>
      <div class="contacts">
        <a href="mailto:olegpustovalov220@gmail.com" class="contact-link">
          📧 olegpustovalov220@gmail.com
        </a>
        <a href="https://t.me/OlegEgoism" target="_blank" class="contact-link">
          ✈️ @OlegEgoism
        </a>
      </div>
    </header>

    <!-- Tech Stack -->
    <section class="section">
      <h2 class="section-title">🛠 Мой стек технологий</h2>
      
      <!-- Languages & Frameworks -->
      <div class="category">
        <div class="category-title">Языки и фреймворки</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python">
            <span>Python</span>
          </div>
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript">
            <span>JavaScript</span>
          </div>
          <div class="tech-card">
            <img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="Django">
            <span>Django</span>
          </div>
          <div class="tech-card">
            <img src="https://cdn.worldvectorlogo.com/logos/fastapi.svg" alt="FastAPI">
            <span>FastAPI</span>
          </div>
          <div class="tech-card">
            <img src="https://miro.medium.com/v2/1*K0a7xINk0RM5gfXGSN68cw.png" alt="React">
            <span>React</span>
          </div>
          <div class="tech-card">
            <img src="https://archive.org/download/github.com-streamlit-streamlit_-_2020-06-10_07-36-23/cover.jpg" alt="Streamlit">
            <span>Streamlit</span>
          </div>
        </div>
      </div>

      <!-- Frontend & Styling -->
      <div class="category">
        <div class="category-title">Frontend & Стилизация</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://www.svgrepo.com/show/21671/css.svg" alt="CSS">
            <span>CSS</span>
          </div>
          <div class="tech-card">
            <img src="https://www.svgrepo.com/show/330083/bootstrap.svg" alt="Bootstrap">
            <span>Bootstrap</span>
          </div>
          <div class="tech-card">
            <img src="https://cdn.prod.website-files.com/62038ffc9cd2db4558e3c7b7/623b43bcfcec4ae2e50ca6e3_rest.svg" alt="REST API">
            <span>REST API</span>
          </div>
          <div class="tech-card">
            <img src="https://s3.amazonaws.com/kinlane-productions2/bw-icons/bw-openapi-spec.png" alt="Swagger">
            <span>Swagger</span>
          </div>
        </div>
      </div>

      <!-- Databases -->
      <div class="category">
        <div class="category-title">Базы данных</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg" alt="PostgreSQL">
            <span>PostgreSQL</span>
          </div>
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg" alt="MySQL">
            <span>MySQL</span>
          </div>
          <div class="tech-card">
            <img src="https://cdn.worldvectorlogo.com/logos/mongodb-icon-1.svg" alt="MongoDB">
            <span>MongoDB</span>
          </div>
          <div class="tech-card">
            <img src="https://www.svgrepo.com/show/342166/redis.svg" alt="Redis">
            <span>Redis</span>
          </div>
          <div class="tech-card">
            <img src="https://imply.io/wp-content/uploads/2024/02/image-3.png" alt="ClickHouse">
            <span>ClickHouse</span>
          </div>
          <div class="tech-card">
            <img src="https://upload.wikimedia.org/wikipedia/commons/b/bb/Apache_Hive_logo.svg" alt="Hive">
            <span>Hive</span>
          </div>
        </div>
      </div>

      <!-- DevOps & Tools -->
      <div class="category">
        <div class="category-title">DevOps & Инструменты</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg" alt="Docker">
            <span>Docker</span>
          </div>
          <div class="tech-card">
            <img src="https://cdn.worldvectorlogo.com/logos/aws-logo.svg" alt="AWS">
            <span>AWS</span>
          </div>
          <div class="tech-card">
            <img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" alt="Git">
            <span>Git</span>
          </div>
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Postman.svg" alt="Postman">
            <span>Postman</span>
          </div>
          <div class="tech-card">
            <img src="https://www.svgrepo.com/show/303576/rabbitmq-logo.svg" alt="RabbitMQ">
            <span>RabbitMQ</span>
          </div>
        </div>
      </div>

      <!-- Analytics & BI -->
      <div class="category">
        <div class="category-title">Аналитика & BI</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://cdn.worldvectorlogo.com/logos/grafana.svg" alt="Grafana">
            <span>Grafana</span>
          </div>
          <div class="tech-card">
            <img src="https://app.yunohost.org/default/v3/logos/71a23aee2309aa0ffa9c960dc818b03d933058d4c93f8e6dd41ea238ee843938.png" alt="Superset">
            <span>Superset</span>
          </div>
          <div class="tech-card">
            <img src="https://avatars.githubusercontent.com/u/52467369?s=200&v=4" alt="Cube">
            <span>Cube</span>
          </div>
          <div class="tech-card">
            <img src="https://avatars.mds.yandex.net/get-sprav-products/1521147/2a000001917fe180a8de459ad2d2b9d2a159/M_height" alt="icCube">
            <span>icCube</span>
          </div>
          <div class="tech-card">
            <img src="https://images.g2crowd.com/uploads/product/image/social_landscape/social_landscape_1192e5c87a2b0217f83a08250bb29519/datahub.png" alt="DataHub">
            <span>DataHub</span>
          </div>
          <div class="tech-card">
            <img src="https://www.sunzinet.com/hs-fs/hubfs/00.%20SUNZINET%20Website%20Assets/03.%20Service%20Pages/10.%20All%20Technology%20partner%20Pages/apache%20nifi%20agentur%20SUNZINET%20-%20fachinformatiker%20f%C3%BCr%20systemintegration.png?width=860&height=674&name=apache%20nifi%20agentur%20SUNZINET%20-%20fachinformatiker%20f%C3%BCr%20systemintegration.png" alt="NiFi">
            <span>NiFi</span>
          </div>
        </div>
      </div>

      <!-- OS & IDE -->
      <div class="category">
        <div class="category-title">ОС & Среды разработки</div>
        <div class="tech-grid">
          <div class="tech-card">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c7/Windows_logo_-_2012.png/500px-Windows_logo_-_2012.png" alt="Windows">
            <span>Windows</span>
          </div>
          <div class="tech-card">
            <img src="https://user-images.githubusercontent.com/39632170/109294252-25681c80-7857-11eb-9ec4-4fbdad9fadfc.png" alt="Ubuntu">
            <span>Ubuntu</span>
          </div>
          <div class="tech-card">
            <img src="https://img.icons8.com/color/200/mac-logo.png" alt="macOS">
            <span>macOS</span>
          </div>
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pycharm/pycharm-original.svg" alt="PyCharm">
            <span>PyCharm</span>
          </div>
          <div class="tech-card">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/webstorm/webstorm-original.svg" alt="WebStorm">
            <span>WebStorm</span>
          </div>
        </div>
      </div>
    </section>
  </div>

  <script>
    // Плавное появление карточек при загрузке
    document.addEventListener('DOMContentLoaded', () => {
      const cards = document.querySelectorAll('.tech-card');
      cards.forEach((card, index) => {
        card.style.opacity = '0';
        card.style.transform = 'translateY(20px)';
        card.style.transition = 'opacity 0.4s ease, transform 0.4s ease';
        setTimeout(() => {
          card.style.opacity = '1';
          card.style.transform = 'translateY(0)';
        }, 100 * index);
      });
    });
  </script>
</body>
</html>
