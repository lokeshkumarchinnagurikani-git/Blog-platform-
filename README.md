
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>NEWS C | Post & Read News</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<link rel="stylesheet" href="style.css">
</head>

<body>

<!-- ================= HEADER ================= -->

<header class="header">

<div class="logo">

<h1>NEWS C</h1>

<p>Post & Read News</p>

</div>

<nav>

<ul class="nav-links">

<li><a href="#">Home</a></li>

<li><a href="#">Today's News</a></li>

<li><a href="#">Categories</a></li>

<li><a href="#">Dashboard</a></li>

<li><a href="#">Login</a></li>

</ul>

</nav>

</header>

<!-- ================= HERO ================= -->

<section class="hero">

<div class="hero-content">

<h2>Welcome to NEWS C</h2>

<p>
Read today's latest news and publish your own news articles
with images.
</p>

<a href="#" class="btn">Read Today's News</a>

</div>

</section>

<!-- ================= TODAY NEWS ================= -->

<section class="today-news">

<h2>Today's Headlines</h2>

<div class="news-container">

<!-- News Card 1 -->

<div class="news-card">

<img src="images/news1.jpg" alt="News">

<div class="news-content">

<h3>ISRO Launches New Satellite Successfully</h3>

<p>
The satellite was launched successfully today and will
improve communication services across India.
</p>

<button>Read More</button>

</div>

</div>

<!-- News Card 2 -->

<div class="news-card">

<img src="images/news2.jpg" alt="News">

<div class="news-content">

<h3>Heavy Rain Alert Across Several States</h3>

<p>
The weather department has issued heavy rainfall warnings
for multiple districts.
</p>

<button>Read More</button>

</div>

</div>

<!-- News Card 3 -->

<div class="news-card">

<img src="images/news3.jpg" alt="News">

<div class="news-content">

<h3>India Wins International Cricket Series</h3>

<p>
India secured a memorable victory in the final match with
excellent batting performance.
</p>

<button>Read More</button>

</div>

</div>

<!-- News Card 4 -->

<div class="news-card">

<img src="images/news4.jpg" alt="News">

<div class="news-content">

<h3>AI Technology Changing Education</h3>

<p>
Artificial Intelligence is helping students learn faster
through smart educational platforms.
</p>

<button>Read More</button>

</div>

</div>

</div>

</section>
<!-- ================= LOGIN SECTION ================= -->

<section id="login" class="login-section">

    <h2>User Login</h2>

    <form id="loginForm">

        <input type="text" id="username" placeholder="Username" required>

        <input type="password" id="password" placeholder="Password" required>

        <button type="submit">Login</button>

    </form>

</section>

<!-- ================= DASHBOARD ================= -->

<section id="dashboard" class="dashboard">

    <h2>User Dashboard</h2>

    <p>Welcome! Read today's news or publish your own news.</p>

    <div class="dashboard-menu">

        <button id="postNewsBtn">Post News</button>

        <button id="viewNewsBtn">View My Posts</button>

        <button id="logoutBtn">Logout</button>

    </div>

</section>

<!-- ================= POST NEWS ================= -->

<section id="post-news" class="post-news">

    <h2>Post Your News</h2>

    <form id="newsForm">

        <input type="text"
               id="newsTitle"
               placeholder="News Title"
               required>

        <input type="text"
               id="newsCategory"
               placeholder="Category"
               required>

        <input type="text"
               id="newsImage"
               placeholder="Image URL or images/news.jpg"
               required>

        <textarea id="newsDescription"
                  rows="8"
                  placeholder="Write your news..."
                  required></textarea>

        <button type="submit">
            Publish News
        </button>

    </form>

</section>

<!-- ================= FOOTER ================= -->

<footer>

    <h3>NEWS C</h3>

    <p>Post & Read News</p>

    <p>&copy; 2026 NEWS C. All Rights Reserved.</p>

</footer>

<!-- ================= JAVASCRIPT ================= -->

<script src="script.js"></script>

</body>
</html>
/* ===========================
   NEWS C - style.css
   Part 2A
=========================== */

/* Google Font */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

/* Reset */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#f4f8f4;
    color:#222;
    line-height:1.6;
}

/* Scroll Bar */
::-webkit-scrollbar{
    width:10px;
}

::-webkit-scrollbar-track{
    background:#e8e8e8;
}

::-webkit-scrollbar-thumb{
    background:#2e8b57;
    border-radius:20px;
}

::-webkit-scrollbar-thumb:hover{
    background:#1d6b42;
}

/* Header */
.header{
    width:100%;
    background:#ffffff;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:18px 8%;
    box-shadow:0 4px 12px rgba(0,0,0,.08);
    position:sticky;
    top:0;
    z-index:1000;
}

/* Logo */
.logo h1{
    color:#2e8b57;
    font-size:34px;
    font-weight:700;
}

.logo p{
    color:#666;
    font-size:14px;
}

/* Navigation */
.nav-links{
    display:flex;
    list-style:none;
    gap:25px;
}

.nav-links li{
    list-style:none;
}

.nav-links a{
    text-decoration:none;
    color:#222;
    font-weight:500;
    transition:.3s;
}

.nav-links a:hover{
    color:#2e8b57;
}

/* Hero Section */
.hero{
    height:80vh;
    background:url("images/news-banner.jpg") center/cover no-repeat;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:#fff;
    position:relative;
}

.hero::before{
    content:"";
    position:absolute;
    inset:0;
    background:rgba(0,0,0,.55);
}

.hero-content{
    position:relative;
    z-index:2;
    max-width:700px;
    padding:20px;
}

.hero-content h2{
    font-size:50px;
    margin-bottom:20px;
}

.hero-content p{
    font-size:20px;
    margin-bottom:30px;
}

/* Button */
.btn{
    display:inline-block;
    background:#2e8b57;
    color:#fff;
    text-decoration:none;
    padding:14px 35px;
    border-radius:8px;
    transition:.3s;
    font-weight:600;
}

.btn:hover{
    background:#1f6b43;
    transform:translateY(-3px);
}

/* Section Heading */
.today-news{
    width:90%;
    margin:60px auto;
}

.today-news h2{
    text-align:center;
    font-size:36px;
    color:#2e8b57;
    margin-bottom:40px;
}<img width="954" height="551" alt="1000172415" src="https://github.com/user-attachments/assets/265dacd1-6329-42ca-8fd2-ed1083130b9b" />
<img src="https://github.com/user-attachments/assets/265dacd1-6329-42ca-8fd2-ed1083130b9b" alt="NEWS C Logo">
/* ===========================
   NEWS C - style.css
   Part 2B
=========================== */

/* Logo */
.logo{
    display:flex;
    align-items:center;
    gap:15px;
}

.logo img{
    width:70px;
    height:70px;
    border-radius:50%;
    object-fit:cover;
    border:3px solid #2e8b57;
}

.logo h1{
    color:#2e8b57;
    font-size:32px;
    font-weight:700;
}

.logo p{
    color:#666;
    font-size:14px;
}

/* Today's News */
.news-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.news-card{
    background:#fff;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 8px 20px rgba(0,0,0,.12);
    transition:.3s;
}

.news-card:hover{
    transform:translateY(-10px);
    box-shadow:0 15px 30px rgba(0,0,0,.18);
}

.news-card img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.news-content{
    padding:20px;
}

.news-content h3{
    color:#2e8b57;
    margin-bottom:12px;
}

.news-content p{
    color:#555;
    margin-bottom:20px;
    line-height:1.6;
}

.news-content button{
    background:#2e8b57;
    color:#fff;
    border:none;
    padding:10px 25px;
    border-radius:6px;
    cursor:pointer;
    transition:.3s;
}

.news-content button:hover{
    background:#1d6b42;
}

/* Login Section */
.login-section{
    width:100%;
    padding:80px 20px;
    background:#eef8ef;
}

.login-section h2{
    text-align:center;
    color:#2e8b57;
    margin-bottom:30px;
}

#loginForm{
    max-width:420px;
    margin:auto;
    background:#fff;
    padding:35px;
    border-radius:12px;
    box-shadow:0 5px 15px rgba(0,0,0,.15);
}

#loginForm input{
    width:100%;
    padding:14px;
    margin:12px 0;
    border:1px solid #ccc;
    border-radius:8px;
    font-size:16px;
}

#loginForm input:focus{
    outline:none;
    border-color:#2e8b57;
}

#loginForm button{
    width:100%;
    padding:14px;
    border:none;
    background:#2e8b57;
    color:#fff;
    border-radius:8px;
    font-size:16px;
    cursor:pointer;
    transition:.3s;
}

#loginForm button:hover{
    background:#1d6b42;
}

/* Dashboard */
.dashboard{
    padding:80px 8%;
    background:#ffffff;
}

.dashboard h2{
    text-align:center;
    color:#2e8b57;
    margin-bottom:15px;
}

.dashboard p{
    text-align:center;
    color:#555;
    margin-bottom:35px;
}

.dashboard-menu{
    display:flex;
    justify-content:center;
    gap:20px;
    flex-wrap:wrap;
}

.dashboard-menu button{
    background:#2e8b57;
    color:#fff;
    border:none;
    padding:14px 28px;
    border-radius:8px;
    cursor:pointer;
    transition:.3s;
    font-size:15px;
}

.dashboard-menu button:hover{
    background:#1d6b42;
    transform:scale(1.05);
}

/* ===========================
   NEWS C - style.css
   Part 2C
=========================== */

/* ===== POST NEWS SECTION ===== */

.post-news{
    width:100%;
    padding:80px 20px;
    background:#f8fff8;
}

.post-news h2{
    text-align:center;
    color:#2e8b57;
    font-size:34px;
    margin-bottom:30px;
}

#newsForm{
    max-width:800px;
    margin:auto;
    background:#ffffff;
    padding:35px;
    border-radius:15px;
    box-shadow:0 8px 20px rgba(0,0,0,.12);
}

#newsForm input,
#newsForm textarea,
#newsForm select{
    width:100%;
    padding:14px;
    margin:12px 0;
    border:1px solid #ccc;
    border-radius:8px;
    font-size:16px;
}

#newsForm textarea{
    resize:vertical;
    min-height:180px;
}

#newsForm input:focus,
#newsForm textarea:focus,
#newsForm select:focus{
    outline:none;
    border-color:#2e8b57;
    box-shadow:0 0 8px rgba(46,139,87,.3);
}

#newsForm button{
    width:100%;
    padding:15px;
    background:#2e8b57;
    color:#fff;
    border:none;
    border-radius:8px;
    font-size:18px;
    cursor:pointer;
    transition:.3s;
}

#newsForm button:hover{
    background:#1c6c42;
}

/* ===== FOOTER ===== */

footer{
    background:#1d1d1d;
    color:#ffffff;
    text-align:center;
    padding:40px 20px;
}

footer h3{
    color:#2ecc71;
    font-size:28px;
    margin-bottom:10px;
}

footer p{
    margin:8px 0;
    color:#ddd;
}

/* ===== ANIMATIONS ===== */

@keyframes fadeUp{

    from{
        opacity:0;
        transform:translateY(30px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }

}

.hero-content,
.news-card,
.login-section,
.dashboard,
.post-news{

    animation:fadeUp .8s ease;

}

/* ===== RESPONSIVE ===== */

@media(max-width:992px){

.header{
    flex-direction:column;
    text-align:center;
}

.nav-links{
    margin-top:20px;
    flex-wrap:wrap;
    justify-content:center;
}

.hero h2{
    font-size:40px;
}

}

@media(max-width:768px){

.hero{
    height:70vh;
}

.hero-content h2{
    font-size:32px;
}

.hero-content p{
    font-size:17px;
}

.news-container{
    grid-template-columns:1fr;
}

.dashboard-menu{
    flex-direction:column;
}

.dashboard-menu button{
    width:100%;
}

.logo{
    flex-direction:column;
}

.logo img{
    width:60px;
    height:60px;
}

}

@media(max-width:480px){

.header{
    padding:15px;
}

.logo h1{
    font-size:26px;
}

.today-news h2,
.post-news h2,
.dashboard h2,
.login-section h2{
    font-size:28px;
}

.hero-content h2{
    font-size:26px;
}

.hero-content p{
    font-size:15px;
}

.btn{
    padding:12px 24px;
}

#loginForm,
#newsForm{
    padding:20px;
}

footer h3{
    font-size:22px;
}

}

/* ===== END OF STYLE.CSS ===== */
/* ===========================================
   NEWS C - script.js
   Part 3A
   Login, Dashboard & Logout
=========================================== */

// Demo Users
const users = [
    {
        username: "admin",
        password: "admin123",
        name: "Administrator"
    },
    {
        username: "lokesh",
        password: "12345",
        name: "Lokesh Kumar"
    },
    {
        username: "user1",
        password: "news123",
        name: "News Reporter"
    }
];

// Get HTML Elements
const loginForm = document.getElementById("loginForm");
const dashboard = document.getElementById("dashboard");
const loginSection = document.getElementById("login");
const logoutBtn = document.getElementById("logoutBtn");

// Hide Dashboard Initially
if (dashboard) {
    dashboard.style.display = "none";
}

// Login
if (loginForm) {

    loginForm.addEventListener("submit", function (e) {

        e.preventDefault();

        const username =
            document.getElementById("username").value.trim();

        const password =
            document.getElementById("password").value.trim();

        const user = users.find(
            u =>
                u.username === username &&
                u.password === password
        );

        if (user) {

            localStorage.setItem(
                "loggedInUser",
                JSON.stringify(user)
            );

            alert("Welcome " + user.name + "!");

            showDashboard();

        } else {

            alert("Invalid Username or Password");

        }

    });

}

// Show Dashboard
function showDashboard() {

    if (loginSection)
        loginSection.style.display = "none";

    if (dashboard)
        dashboard.style.display = "block";

    const user =
        JSON.parse(localStorage.getItem("loggedInUser"));

    if (user) {

        dashboard.innerHTML = `

        <h2>Welcome, ${user.name}</h2>

        <p>You have successfully logged in to NEWS C.</p>

        <div class="dashboard-menu">

            <button id="postNewsBtn">
                📰 Post News
            </button>

            <button id="viewNewsBtn">
                📄 My Posts
            </button>

            <button id="logoutBtn">
                🚪 Logout
            </button>

        </div>

        `;

        document
            .getElementById("logoutBtn")
            .addEventListener("click", logout);

    }

}

// Auto Login
window.onload = function () {

    const user =
        JSON.parse(localStorage.getItem("loggedInUser"));

    if (user) {

        showDashboard();

    }

};

// Logout
function logout() {

    localStorage.removeItem("loggedInUser");

    alert("Logged Out Successfully");

    location.reload();

}

// Dashboard Buttons
document.addEventListener("click", function (e) {

    if (e.target.id === "postNewsBtn") {

        const postSection =
            document.getElementById("post-news");

        if (postSection) {

            postSection.scrollIntoView({
                behavior: "smooth"
            });

        }

    }

    if (e.target.id === "viewNewsBtn") {

        alert("Your published news will appear here in Part 3B.");

    }

});

/* ===========================================
   NEWS C - script.js
   Part 3B
   Post News, Display News, Search News
=========================================== */

// Load saved news
let newsList = JSON.parse(localStorage.getItem("newsList")) || [];

// Elements
const newsForm = document.getElementById("newsForm");

// Create News Section
const newsDisplay = document.createElement("section");
newsDisplay.id = "userNews";
newsDisplay.className = "today-news";

newsDisplay.innerHTML = `
<h2>Published News</h2>

<input
type="text"
id="searchNews"
placeholder="Search News..."
style="width:100%;padding:12px;margin-bottom:20px;border-radius:8px;border:1px solid #ccc;">

<div id="newsContainer" class="news-container"></div>
`;

document.body.appendChild(newsDisplay);

// Publish News
if(newsForm){

newsForm.addEventListener("submit",function(e){

e.preventDefault();

const title=document.getElementById("newsTitle").value;

const category=document.getElementById("newsCategory").value;

const image=document.getElementById("newsImage").value;

const description=document.getElementById("newsDescription").value;

const user=JSON.parse(localStorage.getItem("loggedInUser"));

const news={

id:Date.now(),

title,

category,

image,

description,

author:user ? user.name : "Guest",

date:new Date().toLocaleDateString()

};

newsList.unshift(news);

localStorage.setItem("newsList",JSON.stringify(newsList));

displayNews(newsList);

newsForm.reset();

alert("News Published Successfully!");

});

}

// Display News
function displayNews(newsArray){

const container=document.getElementById("newsContainer");

if(!container) return;

container.innerHTML="";

if(newsArray.length===0){

container.innerHTML="<h3>No News Available</h3>";

return;

}

newsArray.forEach(news=>{

container.innerHTML+=`

<div class="news-card">

<img src="${news.image}" alt="News Image">

<div class="news-content">

<h3>${news.title}</h3>

<p><b>Category:</b> ${news.category}</p>

<p>${news.description}</p>

<p><b>Author:</b> ${news.author}</p>

<p><b>Date:</b> ${news.date}</p>

<button class="readBtn">Read More</button>

</div>

</div>

`;

});

}

// Load Existing News
displayNews(newsList);

// Search News
document.addEventListener("input",function(e){

if(e.target.id==="searchNews"){

const keyword=e.target.value.toLowerCase();

const filtered=newsList.filter(news=>

news.title.toLowerCase().includes(keyword) ||

news.category.toLowerCase().includes(keyword) ||

news.description.toLowerCase().includes(keyword)

);

displayNews(filtered);

}

});

// Read More Button
document.addEventListener("click",function(e){

if(e.target.classList.contains("readBtn")){

alert("Full news feature will be enhanced in Part 3C.");

}

});
/* ==================================================
   NEWS C - Part 3C-1
   Edit, Delete & Like News
================================================== */

// Total Likes
let totalLikes = JSON.parse(localStorage.getItem("totalLikes")) || {};

// Display News
function displayNews(newsArray){

    const container = document.getElementById("newsContainer");

    if(!container) return;

    container.innerHTML = "";

    if(newsArray.length === 0){

        container.innerHTML = "<h3>No News Available</h3>";
        return;

    }

    newsArray.forEach(news=>{

        const likes = totalLikes[news.id] || 0;

        container.innerHTML += `

        <div class="news-card">

            <img src="${news.image}" alt="News">

            <div class="news-content">

                <h3>${news.title}</h3>

                <p><b>Category:</b> ${news.category}</p>

                <p>${news.description}</p>

                <p><b>Author:</b> ${news.author}</p>

                <p><b>Date:</b> ${news.date}</p>

                <button class="likeBtn"
                        data-id="${news.id}">
                    👍 Like (${likes})
                </button>

                <button class="editBtn"
                        data-id="${news.id}">
                    ✏ Edit
                </button>

                <button class="deleteBtn"
                        data-id="${news.id}">
                    🗑 Delete
                </button>

            </div>

        </div>

        `;

    });

}

// Like
document.addEventListener("click",function(e){

    if(e.target.classList.contains("likeBtn")){

        const id = e.target.dataset.id;

        if(!totalLikes[id]){

            totalLikes[id] = 0;

        }

        totalLikes[id]++;

        localStorage.setItem(
            "totalLikes",
            JSON.stringify(totalLikes)
        );

        displayNews(newsList);

    }

});

// Delete
document.addEventListener("click",function(e){

    if(e.target.classList.contains("deleteBtn")){

        const id = Number(e.target.dataset.id);

        if(confirm("Delete this news?")){

            newsList = newsList.filter(
                news => news.id !== id
            );

            localStorage.setItem(
                "newsList",
                JSON.stringify(newsList)
            );

            displayNews(newsList);

        }

    }

});

// Edit
document.addEventListener("click",function(e){

    if(e.target.classList.contains("editBtn")){

        const id = Number(e.target.dataset.id);

        const news = newsList.find(
            item => item.id === id
        );

        if(!news) return;

        const newTitle = prompt(
            "Edit News Title",
            news.title
        );

        if(newTitle !== null){

            news.title = newTitle;

        }

        const newDescription = prompt(
            "Edit Description",
            news.description
        );

        if(newDescription !== null){

            news.description = newDescription;

        }

        localStorage.setItem(
            "newsList",
            JSON.stringify(newsList)
        );

        displayNews(newsList);

        alert("News Updated Successfully");

    }

});
<button class="commentBtn" data-id="${news.id}">💬 Comment</button>

<button class="shareBtn" data-id="${news.id}">📤 Share</button>

<button class="bookmarkBtn" data-id="${news.id}">❤️ Bookmark</button>

/* ============================================
   NEWS C - script.js
   Part 3C-2A
   Comments, Share & Bookmark
============================================ */

// Load Bookmarks
let bookmarks = JSON.parse(localStorage.getItem("bookmarks")) || [];

// Load Comments
let comments = JSON.parse(localStorage.getItem("comments")) || {};

// Update displayNews() buttons
// Add these buttons inside each news-card after the Like/Edit/Delete buttons

/*
<button class="commentBtn" data-id="${news.id}">💬 Comment</button>
<button class="shareBtn" data-id="${news.id}">📤 Share</button>
<button class="bookmarkBtn" data-id="${news.id}">❤️ Bookmark</button>
*/

// ======================
// COMMENT
// ======================

document.addEventListener("click", function (e) {

    if (e.target.classList.contains("commentBtn")) {

        const id = e.target.dataset.id;

        const text = prompt("Enter your comment:");

        if (text && text.trim() !== "") {

            if (!comments[id]) {

                comments[id] = [];

            }

            comments[id].push(text);

            localStorage.setItem(
                "comments",
                JSON.stringify(comments)
            );

            alert("Comment Added Successfully!");

        }

    }

});

// ======================
// SHARE
// ======================

document.addEventListener("click", function (e) {

    if (e.target.classList.contains("shareBtn")) {

        const id = Number(e.target.dataset.id);

        const news = newsList.find(item => item.id === id);

        if (!news) return;

        if (navigator.share) {

            navigator.share({

                title: news.title,

                text: news.description,

                url: window.location.href

            });

        } else {

            navigator.clipboard.writeText(window.location.href);

            alert("Website link copied to clipboard!");

        }

    }

});

// ======================
// BOOKMARK
// ======================

document.addEventListener("click", function (e) {

    if (e.target.classList.contains("bookmarkBtn")) {

        const id = Number(e.target.dataset.id);

        if (!bookmarks.includes(id)) {

            bookmarks.push(id);

            localStorage.setItem(
                "bookmarks",
                JSON.stringify(bookmarks)
            );

            alert("News Bookmarked ❤️");

        } else {

            alert("Already Bookmarked");

        }

    }

});

// ======================
// VIEW COMMENTS
// ======================

function showComments(newsId) {

    if (!comments[newsId] || comments[newsId].length === 0) {

        alert("No Comments Yet");

        return;

    }

    let list = "Comments\n\n";

    comments[newsId].forEach((comment, index) => {

        list += (index + 1) + ". " + comment + "\n";

    });

    alert(list);

}

// ======================
// VIEW BOOKMARKS
// ======================

function viewBookmarks() {

    const savedNews = newsList.filter(news =>
        bookmarks.includes(news.id)
    );

    if (savedNews.length === 0) {

        alert("No Bookmarked News");

        return;

    }

    displayNews(savedNews);

}
/* ===========================================
   NEWS C - script.js
   Part 3C-2B
   User Profile, Statistics, Admin Controls
=========================================== */

// Logged-in User
const currentUser = JSON.parse(localStorage.getItem("loggedInUser"));

// ==========================
// USER PROFILE
// ==========================

function showProfile() {

    if (!currentUser) {
        alert("Please login first.");
        return;
    }

    alert(
`NEWS C USER PROFILE

Name : ${currentUser.name}
Username : ${currentUser.username}

Welcome to NEWS C!
Enjoy Posting & Reading News.`
    );
}

// ==========================
// NEWS STATISTICS
// ==========================

function showStatistics() {

    const totalNews = newsList.length;

    const totalBookmarks = bookmarks.length;

    const totalComments =
        Object.values(comments).reduce(
            (sum, item) => sum + item.length,
            0
        );

    const totalLikeCount =
        Object.values(totalLikes).reduce(
            (sum, item) => sum + item,
            0
        );

    alert(
`NEWS C STATISTICS

📰 Total News : ${totalNews}

👍 Total Likes : ${totalLikeCount}

💬 Total Comments : ${totalComments}

❤️ Total Bookmarks : ${totalBookmarks}`
    );

}

// ==========================
// ADMIN PANEL
// ==========================

function adminPanel() {

    if (!currentUser) {

        alert("Please login.");

        return;

    }

    if (currentUser.username !== "admin") {

        alert("Access Denied!\nOnly Admin can access this panel.");

        return;

    }

    alert(
`ADMIN PANEL

✔ Manage News
✔ Delete Any News
✔ View Website Statistics
✔ Manage Users`
    );

}

// ==========================
// CREATE EXTRA BUTTONS
// ==========================

window.addEventListener("load", function () {

    const dashboard =
        document.querySelector(".dashboard-menu");

    if (!dashboard) return;

    // Profile
    const profileBtn =
        document.createElement("button");

    profileBtn.innerHTML = "👤 Profile";

    profileBtn.onclick = showProfile;

    dashboard.appendChild(profileBtn);

    // Statistics
    const statsBtn =
        document.createElement("button");

    statsBtn.innerHTML = "📊 Statistics";

    statsBtn.onclick = showStatistics;

    dashboard.appendChild(statsBtn);

    // Admin
    const adminBtn =
        document.createElement("button");

    adminBtn.innerHTML = "🛡 Admin Panel";

    adminBtn.onclick = adminPanel;

    dashboard.appendChild(adminBtn);

});

// ==========================
// WEBSITE READY
// ==========================

console.log("NEWS C Loaded Successfully.");

alert("Welcome to NEWS C - Post & Read News");


<img width="833" height="405" alt="1000172425" src="https://github.com/user-attachments/assets/29001c72-4817-459c-ba04-fb480ec69d4c" />
<img width="512" height="776" alt="1000172424" src="https://github.com/user-attachments/assets/d44f0d0a-8b23-4d21-8458-75ffea27b93d" />
<img width="1073" height="488" alt="1000172423" src="https://github.com/user-attachments/assets/085a7b9a-844f-4b97-a77d-3b7b52dd9aa8" />
<img width="1075" height="558" alt="1000172422" src="https://github.com/user-attachments/assets/75c5193c-77b9-4860-b03c-165e2e234bfe" />
<img width="1080" height="633" alt="1000172421" src="https://github.com/user-attachments/assets/961b86f2-9827-4d5a-935f-6fed4c5bae75" />
<img width="1080" height="475" alt="1000172420" src="https://github.com/user-attachments/assets/f936be18-2764-4fbd-a865-ffff15e6ed8a" />
<img width="1058" height="1153" alt="1000172419" src="https://github.com/user-attachments/assets/0fd8c38c-8af8-489e-b299-539006360ef3" />
<img width="1075" height="676" alt="1000172418" src="https://github.com/user-attachments/assets/a57a3cfc-da69-4c70-ab8d-1765f1205540" />
<img width="1070" height="947" alt="1000172417" src="https://github.com/user-attachments/assets/6ed3b380-a98c-4234-8c75-e9efa45dd774" />
<img width="983" height="556" alt="1000172426" src="https://github.com/user-attachments/assets/c5c5e107-fa8b-4f6c-a865-0047c10b189d" />



const defaultNews = [

{
id:1,
title:"ISRO Successfully Launches New Satellite",
category:"Science",
image:"https://github.com/user-attachments/assets/29001c72-4817-459c-ba04-fb480ec69d4c",
description:"ISRO successfully launched a new communication satellite from Sriharikota.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:2,
title:"Indian Cricket Team Wins ODI Series",
category:"Sports",
image:"https://github.com/user-attachments/assets/d44f0d0a-8b23-4d21-8458-75ffea27b93d",
description:"India defeated Australia to win the ODI series.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:3,
title:"Heavy Rain Alert Issued",
category:"Weather",
image:"https://github.com/user-attachments/assets/085a7b9a-844f-4b97-a77d-3b7b52dd9aa8",
description:"Heavy rainfall warning issued for several states.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:4,
title:"AI Technology Changing Education",
category:"Technology",
image:"https://github.com/user-attachments/assets/75c5193c-77b9-4860-b03c-165e2e234bfe",
description:"Artificial Intelligence is transforming education.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:5,
title:"Stock Market Closes Higher",
category:"Business",
image:"https://github.com/user-attachments/assets/961b86f2-9827-4d5a-935f-6fed4c5bae75",
description:"Stock market closed higher after strong banking performance.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:6,
title:"New Express Highway Opened",
category:"National",
image:"https://github.com/user-attachments/assets/f936be18-2764-4fbd-a865-ffff15e6ed8a",
description:"Government inaugurated a new express highway.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:7,
title:"Scientists Discover New Marine Species",
category:"Science",
image:"https://github.com/user-attachments/assets/0fd8c38c-8af8-489e-b299-539006360ef3",
description:"Researchers discovered a rare marine species.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:8,
title:"International Football Championship Begins",
category:"Sports",
image:"https://github.com/user-attachments/assets/a57a3cfc-da69-4c70-ab8d-1765f1205540",
description:"International football championship has begun.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:9,
title:"Government Announces Student Scholarship",
category:"Education",
image:"https://github.com/user-attachments/assets/6ed3b380-a98c-4234-8c75-e9efa45dd774",
description:"New scholarship program announced for students.",
author:"NEWS C",
date:"06 July 2026"
},

{
id:10,
title:"Electric Vehicle Sales Increase",
category:"Automobile",
image:"https://github.com/user-attachments/assets/c5c5e107-fa8b-4f6c-a865-0047c10b189d",
description:"Electric vehicle sales increased significantly.",
author:"NEWS C",
date:"06 July 2026"
}

];
// ===============================
// NEWS C Backend Configuration
// ===============================

// Firebase Configuration
const firebaseConfig = {

apiKey: "YOUR_API_KEY",

authDomain: "YOUR_PROJECT.firebaseapp.com",

projectId: "YOUR_PROJECT_ID",

storageBucket: "YOUR_PROJECT.appspot.com",

messagingSenderId: "YOUR_SENDER_ID",

appId: "YOUR_APP_ID"

};

// Future Initialization
// firebase.initializeApp(firebaseConfig);
