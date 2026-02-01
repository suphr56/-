<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>[ชื่อคุณ] | Portfolio</title>
    <meta name="description" content="Portfolio ของ [ชื่อคุณ] รวมผลงานด้าน Web / Design / Programming">

    
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;500;700&display=swap" rel="stylesheet">

    <style>
     #about {
    padding: 4rem 10%;
    background: #fff;
     }
        
        /* ตั้งค่าพื้นฐาน */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Sarabun', sans-serif;
        }

        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }

        /* Navigation Bar */
        header {
            background: #ffffff;
            padding: 1rem 10%;
            position: sticky;
            top: 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            z-index: 1000;
            transition: 0.3s;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
            margin-left: 2rem;
            font-weight: 500;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #007bff;
        }

        /* Hero Section */
        .hero {
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(135deg, #007bff 0%, #00d4ff 100%);
            color: white;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        .hero button:hover {
             transform: translateY(-2px);
             box-shadow: 0 15px 20px rgba(0,0,0,0.2);
         }


        /* Works Section */
        #works {
            padding: 4rem 10%;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .work-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            transition: 0.3s;
        }

        .work-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .work-card h3, .work-card p, .work-card a {
            padding: 10px 20px;
            display: block;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            background: #333;
            color: white;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo">MyBrand</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#works">Works</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <h1>สวัสดี, ฉันคือ [ชื่อของคุณ]</h1>
        <p>นักสร้างสรรค์ผลงานด้าน [ศิลปะ / เขียนโปรแกรม / งานเขียน]</p>
        <button onclick="document.querySelector('#works').scrollIntoView({behavior: 'smooth'})">ดูผลงานของฉัน</button>
    </section>

    <section id="works">
        <h2>ผลงานล่าสุด</h2>
        <div class="grid-container">
            <div class="work-card">
                <img src="https://via.placeholder.com/400x250" alt="ชื่อโปรเจกต์">
                <h3>ชื่อโปรเจกต์ 1</h3>
                <p>คำอธิบายสั้นๆ เกี่ยวกับเทคนิคหรือสิ่งที่ทำ</p>
                <a href="#">อ่านเพิ่มเติม</a>
            </div>
            <div class="work-card">
                <img src="https://via.placeholder.com/400x250" alt="ชื่อโปรเจกต์">
                <h3>ชื่อโปรเจกต์ 2</h3>
                <p>คำอธิบายสั้นๆ เกี่ยวกับเทคนิคหรือสิ่งที่ทำ</p>
                <a href="#">อ่านเพิ่มเติม</a>
            </div>
        </div>
    </section>

    <section id ="about">
        <h2 style="text-align: center; margin-bottom: 2rem;">เกี่ยวกับฉัน</h2>
        <div class="about-container" style="display: flex; flex-wrap: wrap; gap: 3rem; align-items: center;">
            <div class="about-img" style="flex: 1; min-width: 300px;">
                <img src="https://via.placeholder.com/400x400" alt="รูปของฉัน" style="width: 100%; border-radius: 20px; box-shadow: 10px 10px 0px #007bff;">
            </div>
            <div class="about-text" style="flex: 1; min-width: 300px;">
                <h3>สวัสดี! ฉันคือ [ชื่อของคุณ]</h3>
                <p style="margin: 1rem 0;"> ฉันชอบเรียนรู้เทคโนโลยีใหม่ๆ และพัฒนาตัวเองอยู่เสมอ</p>
                <div class="skills">
                    <span style="display: inline-block; background: #e7f3ff; color: #007bff; padding: 5px 15px; border-radius: 20px; margin: 5px;">HTML/CSS</span>
                    <span style="display: inline-block; background: #e7f3ff; color: #007bff; padding: 5px 15px; border-radius: 20px; margin: 5px;">JavaScript</span>
                    <span style="display: inline-block; background: #e7f3ff; color: #007bff; padding: 5px 15px; border-radius: 20px; margin: 5px;">Design</span>
                </div>
            </div>
        </div>
    </section>
<section id="contact" style="padding: 4rem 10%; background: #f4f7f6;">
    <h2 style="text-align: center; margin-bottom: 2rem;">ติดต่อฉัน</h2>

    <div class="contact-card" style="
        max-width: 600px;
        margin: 0 auto;
        background: white;
        padding: 2rem;
        border-radius: 15px;
        box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        text-align: center;
    ">
        <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
            หากสนใจผลงานหรืออยากพูดคุยเพิ่มเติม สามารถดูโค้ดและติดต่อฉันได้ที่ GitHub
        </p>

        <div style="margin-bottom: 1.5rem;">
            <strong>GitHub :</strong>
            <p style="margin-top: 0.5rem; font-size: 1.05rem;">
                github.com/<span style="color:#007bff;">your-github-username</span>
            </p>
        </div>

        <a 
            href="https://github.com/your-github-username"
            target="_blank"
            style="
                display: inline-block;
                background: #24292e;
                color: white;
                padding: 12px 30px;
                border-radius: 30px;
                text-decoration: none;
                font-size: 1rem;
                transition: 0.3s;
            "
            onmouseover="this.style.opacity='0.8'"
            onmouseout="this.style.opacity='1'"
        >
            ไปที่ GitHub ของฉัน
        </a>
    </div>
</section>



     <p>&copy; <span id="year"></span> [ชื่อของคุณ]. All rights reserved.</p>


    <script>
        // ส่วนการทำงาน JavaScript
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetSection = document.querySelector(targetId);
                if (targetSection) {
                    window.scrollTo({
                        top: targetSection.offsetTop - 70,
                        behavior: 'smooth'
                    });
                }
            });
        });

        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 50) {
                header.style.backgroundColor = '#ffffff';
                header.style.boxShadow = '0 4px 20px rgba(0,0,0,0.15)';
            } else {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.1)';
            }
        });

        const observerOptions = { threshold: 0.2 };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // ใส่ Animation ให้กับทุก Section ที่ต้องการ
        document.querySelectorAll('.work-card, #about, #contact').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'all 0.6s ease-out';
            observer.observe(el);
        });
       document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
