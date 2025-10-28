<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MTechLab Engineerings</title>
<style>
/* -------------------- General Styles -------------------- */
* { box-sizing:border-box; margin:0; padding:0; font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
body { background:#f4f6f8; color:#333; line-height:1.6; }
a { text-decoration:none; color:inherit; }

/* Header */
header {
    background: linear-gradient(90deg,#1a73e8,#4285f4);
    color:white; padding:25px 20px; text-align:center; position:sticky; top:0; z-index:1000;
    box-shadow:0 4px 10px rgba(0,0,0,0.1);
}
header h1{ font-size:32px; margin-bottom:10px; }
nav a{ color:white; margin:0 15px; font-weight:bold; transition:0.3s; }
nav a:hover{ text-decoration:underline; }

/* Sections */
section{ padding:60px 20px; max-width:1200px; margin:auto; }
h2{ text-align:center; margin-bottom:40px; color:#1a73e8; font-size:28px; }

/* About Section */
#about {
    background-color: #ffffff;
    padding: 50px 20px;
    max-width: 1000px;
    margin: 40px auto;
    border-radius: 15px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.1);
}
#about h2 {
    text-align: center;
    color: #1a73e8;
    font-size: 28px;
    margin-bottom: 25px;
}
#about p {
    color: #555;
    font-size: 16px;
    margin-bottom: 15px;
}
#about ul {
    list-style-type: disc;
    margin-left: 20px;
    margin-bottom: 15px;
}
#about ul li {
    margin-bottom: 10px;
    line-height: 1.5;
}

/* Tutors grid */
.tutors-grid{ display:grid; grid-template-columns: repeat(auto-fit, minmax(250px,1fr)); gap:25px; }
.tutor-card{
    background:#fff; border-radius:15px; padding:25px; text-align:center;
    box-shadow:0 6px 15px rgba(0,0,0,0.1); transition: transform 0.4s, box-shadow 0.4s;
    opacity:0; transform:translateY(30px); animation:fadeInUp 0.8s forwards;
}
.tutor-card:nth-child(1){ animation-delay:0.1s; }
.tutor-card:nth-child(2){ animation-delay:0.3s; }
@keyframes fadeInUp{ to{opacity:1; transform:translateY(0);} }
.tutor-card:hover{ transform:translateY(-10px); box-shadow:0 12px 25px rgba(0,0,0,0.15); }
.tutor-card h3{ color:#1a73e8; margin-bottom:10px; font-size:22px; }
.tutor-card p{ color:#555; font-size:14px; margin:5px 0; }
.tutor-card a.contact-btn{
    display:inline-block; margin-top:15px; background:linear-gradient(90deg,#1a73e8,#4285f4);
    color:white; padding:10px 18px; border-radius:8px; font-weight:bold; transition:0.3s;
}
.tutor-card a.contact-btn:hover{ background:linear-gradient(90deg,#155ab6,#1a52a3); }

/* Form */
form{
    max-width:500px; margin:auto; background:#fff; padding:35px 25px;
    border-radius:15px; box-shadow:0 6px 15px rgba(0,0,0,0.1);
    display:flex; flex-direction:column; gap:18px;
    opacity:0; transform:translateY(30px); animation:fadeInUp 1s forwards;
}
input, select, button{ padding:12px; font-size:15px; border-radius:8px; border:1px solid #ccc; width:100%; }
button{ background:linear-gradient(90deg,#1a73e8,#4285f4); color:white; border:none; cursor:pointer; font-weight:bold; transition:0.3s; }
button:hover{ background:linear-gradient(90deg,#155ab6,#1a52a3); }

/* Footer */
footer{ background:linear-gradient(90deg,#1a73e8,#4285f4); color:white; text-align:center; padding:25px 20px; margin-top:40px; }

/* Modal */
#successModal{ display:none; position:fixed; z-index:2000; left:0; top:0; width:100%; height:100%; overflow:auto; background-color: rgba(0,0,0,0.4); }
#successModal .modal-content{ background:white; margin:15% auto; padding:30px; border-radius:12px; width:90%; max-width:400px; text-align:center; animation:fadeInUp 0.5s forwards; }
#successModal button{ margin-top:20px; }

/* Responsive */
@media (max-width:600px){ header h1{ font-size:24px;} h2{ font-size:22px;} }

</style>
</head>
<body>

<header>
    <h1>MTechLab Engineerings</h1>
    <nav><a href="#about">About</a><a href="#tutors">Tutors</a><a href="#application">Apply</a></nav>
</header>

<!-- About Section -->
<section id="about">
    <h2>About MTechLab Engineerings</h2>
    <p>
        MTechLab Engineerings is a dynamic company offering a wide range of professional and educational services.
        We deliver <strong>high-quality programming, IT support, and advanced education</strong> to students, businesses, and community learners.
        Our goal is to empower you through <strong>innovation, practical skills, and professional services</strong>.
    </p>
    <p>Our services include:</p>
    <ul>
        <li>Development and training in <strong>HTML, Python, VB.NET, C, C#, and Java</strong> — for both individuals and companies.</li>
        <li>Operating system installations, laptop flashing, phone OS updates, and system recovery services.</li>
        <li>Tutoring in subjects such as <strong>Pure Maths, Software Engineering, Statistics, and Business</strong> up to advanced and ordinary levels.</li>
        <li>Programming courses from <strong>ECD to tertiary</strong> levels, teaching programming languages from scratch.</li>
    </ul>
    <p>
        Whether you’re a student, business, or community learner, MTechLab Engineerings provides the tools, knowledge, and support you need to succeed.
    </p>
</section>

<!-- Tutors Section -->
<section id="tutors">
    <h2>Our Tutors</h2>
    <div class="tutors-grid">
        <div class="tutor-card">
            <h3>DoxllerTech</h3>
            <p>Role: Tutor, Programmer</p>
            <p>Email: <a href="mailto:hacktillwedie@gmail.com">hacktillwedie@gmail.com</a></p>
            <p>Contact: <a href="tel:+263782068207">+263782068207</a></p>
            <p>Brand: DoxllerTech</p>
            <a class="contact-btn" href="mailto:hacktillwedie@gmail.com">Contact</a>
        </div>
        <div class="tutor-card">
            <h3>TechRyder</h3>
            <p>Role: Tutor, Designer, Engineer</p>
            <p>Email: <a href="mailto:j1techryder@gmail.com">j1techryder@gmail.com</a></p>
            <p>Contact: <a href="tel:+263774861688">+263774861688</a></p>
            <a class="contact-btn" href="mailto:j1techryder@gmail.com">Contact</a>
        </div>
    </div>
</section>

<!-- Application Form -->
<section id="application">
    <h2>Student Application</h2>
    <form id="applicationForm">
        <input type="text" id="studentName" placeholder="Full Name" required>
        <input type="email" id="studentEmail" placeholder="Email" required>
        <input type="tel" id="studentPhone" placeholder="Phone Number (e.g. +26377xxxxxxx)" required>
        <select id="preferredTutor" required>
            <option value="">Select Preferred Tutor</option>
            <option value="DoxllerTech">DoxllerTech</option>
            <option value="TechRyder">TechRyder</option>
        </select>
        <button type="submit">Submit Application</button>
    </form>
</section>

<footer><p>&copy; 2025 TechRyder & DoxllerTech</p></footer>

<!-- Success Modal -->
<div id="successModal">
    <div class="modal-content">
        <h3>Application Submitted!</h3>
        <p>Your application has been sent. Both you and the tutor will receive a confirmation SMS.</p>
        <button onclick="closeModal()">Close</button>
    </div>
</div>

<script>
const modal = document.getElementById("successModal");
function closeModal(){ modal.style.display="none"; }

document.getElementById("applicationForm").addEventListener("submit", async function(e){
    e.preventDefault();
    const name = document.getElementById("studentName").value;
    const email = document.getElementById("studentEmail").value;
    const phone = document.getElementById("studentPhone").value;
    const tutor = document.getElementById("preferredTutor").value;

    if(name && email && phone && tutor){
        try{
            const response = await fetch("/submit_application", {
                method:"POST",
                headers:{"Content-Type":"application/json"},
                body:JSON.stringify({name,email,phone,tutor})
            });
            const result = await response.json();
            if(result.status==="success"){
                modal.style.display="block";
                this.reset();
            } else { alert("Error: "+result.message); }
        } catch(err){ console.error(err); alert("Failed to submit application. Try again."); }
    } else { alert("Please fill all fields!"); }
});
</script>

</body>
</html>
ss
