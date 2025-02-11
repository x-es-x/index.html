#index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Work Immersion</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            text-align: center;
            overflow-x: hidden;
        }
        .container {
            max-width: 900px;
            margin: 80px auto;
            padding: 25px;
            background: rgba(255, 255, 255, 0.15);
            border-radius: 12px;
            backdrop-filter: blur(12px);
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
            animation: fadeIn 1s ease-in-out;
            position: relative;
        }
        .slider {
            position: relative;
            width: 100%;
            height: 250px;
            overflow: hidden;
        }
        .slide {
            position: absolute;
            width: 100%;
            opacity: 0;
            transform: translateX(100%);
            transition: opacity 0.8s ease, transform 0.8s ease-in-out;
        }
        .slide.active {
            opacity: 1;
            transform: translateX(0);
        }
        .arrow-left, .arrow-right {
            font-size: 40px;
            cursor: pointer;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            color: white;
        }
        .arrow-left { left: 10px; }
        .arrow-right { right: 10px; }
        .hidden { display: none; }
        button {
            background-color: #ff6b6b;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 8px;
            transition: background 0.3s;
        }
        button:hover { background-color: #ff4040; }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>
    <main>
        <!-- Home Page -->
        <section id="home">
            <div class="container">
                <h1>Welcome to My Work Immersion Experience</h1>
                <p>Mabuhay Mahal Tana! I am <strong>Bodegas, Erlene S.</strong>, a Grade <strong>12</strong> student from <strong>Spain</strong>.</p>  
                <p>This website will showcase my journey at <strong>Calapan Cable</strong> through my narrative and journal.</p>
                <button onclick="showSection('experience')">Read</button>
            </div>
        </section>

        <!-- Experience Section -->
        <section id="experience" class="hidden">
            <div class="container">
                <h2>Narrative Report</h2>
                <div class="slider" id="narrative-slider">
                    <div class="slide active"><h3>My experiences</h3><p>My work immersion at Calapan Cable was both challenging and rewarding. I gained valuable lessons in discipline, patience, and teamwork. On the first day, we had an orientation with Mr. Jason C. Rivera, who explained the rules and expectations for our work. After that, I was paired with my partner, Reymar, and we were assigned the task of cleaning and organizing a large number of books under the supervision of Ma’am Ellaine. She gave us instructions on how to properly clean and arrange them. The work required patience and attention to detail, which helped us understand the importance of following instructions carefully.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>The following days were exhausting as we continued cleaning and sorting books for long hours. Mr. Jason provided feedback to help us improve our work, and we had to stay focused despite the tiring tasks. We were required to stand for most of the day, with only a lunch break allowed. Mobile phones were not permitted during work hours, which helped us concentrate on our tasks. Though the work was repetitive, I remained determined to complete it properly. After several days, we finished cleaning and moved on to organizing the books into their correct categories, making sure they were neatly arranged.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>In the second week, our responsibilities changed. In the mornings, we observed office work and learned how documents were processed and managed. In the afternoons, we continued sorting books. Later, we were assigned to write down customer information, which had to be recorded neatly and accurately. Another important task was counting payment slips. Each pad had to contain exactly 100 slips, so we had to be extremely careful. Any mistake meant we had to count everything again. This required patience, focus, and teamwork to ensure accuracy. The repetitive nature of the task made it difficult, but we worked hard to complete it correctly.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>On the final day of our immersion, we completed the last batch of payment slip counting. In the afternoon, we prepared for the recognition program, which marked the official end of our 10-day Work Immersion Program. The ceremony acknowledged our efforts and gave us a chance to reflect on our experiences. We also had a small gathering where we shared our thoughts about the immersion. Overall, my work immersion at Calapan Cable taught me valuable skills in organization, discipline, and responsibility. Even though it was challenging, I gained real workplace experience that will help me in the future. The program was a great way to conclude our journey, and I am grateful for everything I learned.</p></div>
                </div>
                <button onclick="showSection('journal')">Next</button>
                <button onclick="showSection('home')">Home</button>
                <span class="arrow-left" onclick="moveSlide('narrative-slider', 'prev')">&#8592;</span>
                <span class="arrow-right" onclick="moveSlide('narrative-slider', 'next')">&#8594;</span>
            </div>
        </section>

        <!-- Journal Section -->
        <section id="journal" class="hidden">
            <div class="container">
                <h2>Journal Entry</h2>
                <div class="slider" id="journal-slider">
                    <div class="slide active"><h3>My experiences</h3><p>My work immersion at Calapan Cable was both challenging and rewarding. I gained valuable lessons in discipline, patience, and teamwork. On the first day, we had an orientation with Mr. Jason C. Rivera, who explained the rules and expectations. I was paired with my partner, Reymar, and we were assigned to clean and organize a large number of books under Ma’am Ellaine's supervision. She guided us on the proper cleaning process, which required patience and attention to detail. At first, it seemed simple, but the overwhelming number of books made it physically exhausting. By the end of the day, my arms and legs were sore.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>The following days were just as tiring as we continued cleaning and sorting books for long hours. Mr. Jason gave us feedback to improve our work, and we had to stay focused despite the repetitive tasks. We stood for most of the day with only a lunch break, and mobile phones were not allowed during work hours. The lack of breaks and monotonous work made it hard to stay motivated, but I reminded myself that it was part of the learning process. After several days, we finally completed the cleaning and moved on to organizing the books into proper categories, ensuring everything was arranged correctly to avoid confusion later.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>In the second week, our tasks changed slightly. In the mornings, we observed office work and learned how employees managed paperwork and records, giving us insight into office operations. In the afternoons, we continued sorting books before taking on a new task: writing down customer information. This required neat and accurate handwriting, making it challenging, especially with the large volume of data. Another major task was counting payment slips, ensuring each pad had exactly 100 slips. Any mistake meant recounting everything. This required patience, focus, and teamwork to maintain accuracy. Despite the repetitive nature of the task, we stayed committed to getting it right.</p></div>
                    <div class="slide"><h3>My experiences</h3><p>On the final day, we completed our last tasks in the morning before preparing for the recognition program in the afternoon. The event marked the end of our work immersion, and we were recognized for our efforts. It felt rewarding to see our hard work acknowledged, and we ended the program with a small gathering, sharing food and reflecting on our experiences. Although the 10-day work immersion was exhausting and repetitive, it taught me discipline, perseverance, and the value of teamwork. Despite the challenges, I learned the importance of patience and accuracy in any job, and I was proud of what we had accomplished.</p></div>
                </div>
                <button onclick="showSection('thank-you')">Next</button>
                <button onclick="showSection('home')">Home</button>
                <span class="arrow-left" onclick="moveSlide('journal-slider', 'prev')">&#8592;</span>
                <span class="arrow-right" onclick="moveSlide('journal-slider', 'next')">&#8594;</span>
            </div>
        </section>

        <!-- Thank You Section -->
        <section id="thank-you" class="hidden">
            <div class="container">
                <h2>Thank You!</h2>
                <p>Thank you for exploring my work immersion journey.</p>
                <button onclick="showSection('home')">Home</button>
            </div>
        </section>
    </main>

    <script>
        function showSection(sectionId) {
            document.querySelectorAll("section").forEach(section => {
                section.classList.add("hidden");
            });
            document.getElementById(sectionId).classList.remove("hidden");
        }

        function moveSlide(sliderId, direction) {
            const slider = document.getElementById(sliderId);
            const slides = slider.children;
            let activeIndex = Array.from(slides).findIndex(slide => slide.classList.contains("active"));

            slides[activeIndex].classList.remove("active");

            if (direction === "next") {
                activeIndex = (activeIndex + 1) % slides.length;
            } else {
                activeIndex = (activeIndex - 1 + slides.length) % slides.length;
            }

            slides[activeIndex].classList.add("active");
        }
    </script>
</body>
</html>
