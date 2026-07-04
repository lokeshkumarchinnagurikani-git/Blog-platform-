<section class="posts">

    <h2>Latest News</h2>

    <div class="post">
    <header class="hero">

     
        

.comment{
    background:#FFF8E1;
    padding:10px;
    margin-top:10px;
    border-radius:5px;
}

textarea{
    width:100%;
    padding:10px;
    margin-top:10px;
    border:1px solid #ccc;
    border-radius:5px;
}

button{
    background:#FBC02D;
    color:#333;
    border:none;
    padding:10px 20px;
    margin-top:10px;
    border-radius:5px;
    cursor:pointer;
}

button:hover{
    background:#F9A825;
}
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>NEW C</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<header>

<div class="logo">
NEW C
</div>

<nav>

<a href="index.html">Home</a>

<a href="login.html">Login</a>

<a href="register.html">Register</a>

<a href="dashboard.html">Dashboard</a>

</nav>

</header>

<section class="hero">

<div class="overlay">

<h1 class="main-title">
NEW C
</h1>

<p class="sub-title">
Post the News Only
</p>

<a href="login.html" class="btn">
Login
</a>

<a href="register.html" class="btn">
Register
</a>

</div>

</section>

<section class="about">

<h2>
About NEW C
</h2>

<p>

NEW C is a simple online news platform where registered users can
publish news articles and allow readers to comment on them.
The platform provides secure login, easy news posting,
and an interactive comment system.

</p>

</section>

<section class="features">

<div class="card">

<h3>
📰 Post News
</h3>

<p>

Share the latest news with readers.

</p>

</div>

<div class="card">

<h3>
💬 Comments
</h3>

<p>

Readers can post comments and discuss news.

</p>

</div>

<div class="card">

<h3>
🔒 Secure Login
</h3>

<p>

Only registered users can post news.

</p>

</div>

</section>

<footer>

<p>

© 2026 NEW C | Post the News Only

</p>

</footer>

</body>

</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Login - NEW C</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="form-container">

<h2>Customer Login</h2>

<form id="loginForm">

<input type="email"
id="loginEmail"
placeholder="Enter Email"
required>

<input type="password"
id="loginPassword"
placeholder="Enter Password"
required>

<button type="submit">
Login
</button>

<p style="text-align:center;margin-top:15px;">
Don't have an account?

<a href="register.html">
Register
</a>

</p>

</form>

</div>

<script src="script.js"></script>

</body>
</html>

const registerForm=document.getElementById("registerForm");
const loginForm=document.getElementById("loginForm");
const newsForm=document.getElementById("newsForm");

let users=JSON.parse(localStorage.getItem("users"))||[];
let news=JSON.parse(localStorage.getItem("news"))||[];

if(registerForm){

registerForm.addEventListener("submit",function(e){

e.preventDefault();

const user={
name:document.getElementById("name").value,
email:document.getElementById("email").value,
password:document.getElementById("password").value
};

users.push(user);

localStorage.setItem("users",JSON.stringify(users));

alert("Registration Successful");

window.location="login.html";

});

}

if(loginForm){

loginForm.addEventListener("submit",function(e){

e.preventDefault();

let email=document.getElementById("loginEmail").value;
let password=document.getElementById("loginPassword").value;

let found=users.find(u=>u.email===email&&u.password===password);

if(found){

localStorage.setItem("currentUser",found.name);

alert("Login Successful");

window.location="dashboard.html";

}else{

alert("Invalid Email or Password");

}

});

}

if(newsForm){

displayNews();

newsForm.addEventListener("submit",function(e){

e.preventDefault();

const post={

title:document.getElementById("newsTitle").value,

content:document.getElementById("newsContent").value,

author:localStorage.getItem("currentUser"),

comments:[]

};

news.unshift(post);

localStorage.setItem("news",JSON.stringify(news));

newsForm.reset();

displayNews();

});

}

function displayNews(){

let container=document.getElementById("newsContainer");

if(!container) return;

container.innerHTML="";

news.forEach((post,index)=>{

container.innerHTML+=`

<div class="post">

<h3>${post.title}</h3>

<p>${post.content}</p>

<p><b>Posted By:</b> ${post.author}</p>

<input id="comment${index}" placeholder="Write a comment">

<button onclick="addComment(${index})">

Post Comment

</button>

<button onclick="editPost(${index})">

Edit

</button>

<button onclick="deletePost(${index})">

Delete

</button>

<div id="comments${index}">

${post.comments.map(c=>`<div class="comment">${c}</div>`).join("")}

</div>

</div>

`;

});

}

function addComment(index){

let box=document.getElementById("comment"+index);

if(box.value=="") return;

news[index].comments.push(box.value);

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

function editPost(index){

let newTitle=prompt("Edit Title",news[index].title);

let newContent=prompt("Edit Content",news[index].content);

if(newTitle!=null){

news[index].title=newTitle;

news[index].content=newContent;

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

}

function deletePost(index){

if(confirm("Delete this News?")){

news.splice(index,1);

localStorage.setItem("news",JSON.stringify(news));

displayNews();

}

}

function logout(){

localStorage.removeItem("currentUser");

window.location="login.html";

}





