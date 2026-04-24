# rahul-portfolio
rahul-portfolio
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Rahul Selokar | Cloud & DevOps Engineer</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(135deg, #0f172a, #020617);
  color: #fff;
}

.container {
  max-width: 900px;
  margin: auto;
  padding: 20px;
}

/* Glass Effect */
.glass {
  background: rgba(255,255,255,0.05);
  backdrop-filter: blur(10px);
  border-radius: 15px;
  padding: 20px;
  margin-top: 20px;
}

/* Header */
.center {
  text-align: center;
}

/* Typing */
.typing {
  color: #00f7ff;
  font-weight: bold;
  font-size: 18px;
}

/* Buttons */
.btn {
  display: inline-block;
  padding: 8px 15px;
  margin: 5px;
  border-radius: 20px;
  text-decoration: none;
  color: #fff;
  background: linear-gradient(45deg, #00f7ff, #0077ff);
  font-size: 13px;
}

/* Badges */
.badge {
  display: inline-block;
  padding: 6px 10px;
  margin: 5px;
  border-radius: 20px;
  font-size: 12px;
  background: #1e293b;
}

/* Sections */
h2 {
  border-bottom: 1px solid #334155;
  padding-bottom: 5px;
}

.card {
  background: #020617;
  padding: 15px;
  border-left: 3px solid #00f7ff;
  margin-top: 10px;
}
</style>

</head>

<body>

<div class="container">

  <!-- HEADER -->

  <div class="glass center">
    <h1>👋 Hi, I'm Rahul Selokar</h1>

    <div class="typing" id="typing"></div>

    <p>
      <img src="https://komarev.com/ghpvc/?username=rahulselokar27&label=Profile+Views&color=0e75b6" />
    </p>

    <a href="https://www.linkedin.com/in/rahul-selokar-771387402" class="btn">LinkedIn</a>
    <a href="https://selokartrader.online" class="btn">Portfolio</a>
    <a href="https://github.com/rahulselokar27" class="btn">GitHub</a>

  </div>

  <!-- ABOUT -->

  <div class="glass">
    <h2>👋 About Me</h2>
    <p>
      I specialize in building and automating cloud infrastructure on AWS using tools like EC2, VPC, S3, and RDS.
    </p>
    <p>
      I work with Terraform and CI/CD pipelines (GitHub Actions, Jenkins) to deploy scalable applications.
    </p>
    <p>
      I build reliable, secure, and self-healing systems 🚀
    </p>
  </div>

  <!-- EXPERIENCE -->

  <div class="glass">
    <h2>💼 Experience</h2>

    <div class="card">
      <b>Student Intern – Cloudblitz</b><br>
      Jan 2026 – Present<br>
      📍 Nagpur, India
      <ul>
        <li>Managing AWS cloud infrastructure</li>
        <li>Working on CI/CD pipelines & Terraform</li>
      </ul>
    </div>

  </div>

  <!-- TECH STACK -->

  <div class="glass">
    <h2>🛠 Tech Stack</h2>

    <h3>☁️ Cloud & DevOps</h3>
    <span class="badge">AWS</span>
    <span class="badge">Terraform</span>
    <span class="badge">Docker</span>
    <span class="badge">Kubernetes</span>
    <span class="badge">Jenkins</span>

    <h3>💻 Languages</h3>
    <span class="badge">Python</span>
    <span class="badge">Bash</span>
    <span class="badge">Linux</span>
    <span class="badge">Git</span>

  </div>

  <!-- GITHUB STATS -->

  <div class="glass center">
    <h2>📊 GitHub Stats</h2>

    <img src="https://github-readme-stats.vercel.app/api?username=rahulselokar27&show_icons=true&theme=tokyonight" width="100%"/>

    <img src="https://github-readme-streak-stats.herokuapp.com/?user=rahulselokar27&theme=tokyonight" width="100%"/>

  </div>

</div>

<!-- Typing Script -->

<script>
const text = ["Cloud & DevOps Engineer", "AWS | Docker | Kubernetes", "Automation Enthusiast 🚀"];
let i=0, j=0, current="", isDeleting=false;

function type() {
  current = text[i];
  
  if(isDeleting){
    j--;
  } else {
    j++;
  }

  document.getElementById("typing").innerHTML = current.substring(0,j);

  if(!isDeleting && j === current.length){
    isDeleting = true;
    setTimeout(type, 1000);
    return;
  }

  if(isDeleting && j === 0){
    isDeleting = false;
    i = (i+1)%text.length;
  }

  setTimeout(type, isDeleting ? 50 : 100);
}

type();
</script>

</body>
</html>
