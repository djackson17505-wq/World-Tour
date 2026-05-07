<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8" />
<title>Pets Website</title>

<style>
body {
    font-family: Verdana, Garamond, sans-serif;
    font-size: 11pt;
}

table {
    width: 65%;
    margin-left: auto;
    margin-right: auto;
}

a {
    color: black;
    text-decoration: none;
    margin: 0 10px;
}

a:hover {
    background: purple;
    color: white;
}

.navlist {
    display: inline;
}

.content {
    margin: 20px;
}

p.withmargin {
    margin-left: 30pt;
    margin-right: 30pt;
}

.title {
    font-size: xx-large;
    color: navy;
    font-family: "Bauhaus 93", Verdana;
    text-align: center;
}

.subtitle {
    font-size: large;
    color: navy;
    font-family: "Bauhaus 93", Verdana;
    text-align: center;
}

/* JS section */
section {
    display: none;
    margin-top: 40px;
}

.active {
    display: block;
}
</style>
</head>

<body>

<!-- NAVIGATION  -->
<div style="text-align:center; margin-top:20px;">
    <ul>
        <li class="navlist"><a href="#" onclick="showPage('home')">Home</a></li>
        <li class="navlist"><a href="#" onclick="showPage('dogs')">Dogs</a></li>
        <li class="navlist"><a href="#" onclick="showPage('cats')">Cats</a></li>
        <li class="navlist"><a href="#" onclick="showPage('other animals')">Other Animals</a></li>
    </ul>
</div>

<!-- HOME -->
<section id="home" class="active">

<div class="title">Find you new best friend</div>
<div class="subtitle">Animals Available for Adoption</div>

<div class="content">
<p class="withmargin">
Having a pet can make your life better. Pets help you feel less lonely and reduce stress. 
They encourage you to exercise, especially dogs that need daily walks. 
Taking care of a pet also gives you a daily routine and a sense of responsibility. 
Pets provide unconditional companionship and can even help you meet new people. 
For families, they teach children kindness and care for others.
</p>

<p class="withmargin" style="font-style: italic; text-align:center;">
E-mail us at <a href="lovepetpet@gmail.com ">lovepetpet@gmail.com</a>
</p>
</div>

</section>


<!-- DOGS -->
<section id="dogs">

<div class="title">DOGS</div>

<p>VVVV DOGS.</p>

<ul>
<li><b>A:</b> XXXX.</li>
<li><b>B:</b> XXX.</li>
<li><b>C:</b> XXXX.</li>
</ul>

<table>
<tr>
<th>CCCC</th>
<th>CCCC</th>
<th>CCC</th>
</tr>
<tr>
<td><img src="https://jpg" width="420"></td>
<td><img src="https://" width="420"></td>
<td><img src="https://" width="420"></td>
</tr>
</table>

</section>


<!-- CATS -->
<section id="cats">

<div class="title">Cats</div>

<h3>About the class</h3>
<p>Watch video/audio to learn about pets:</p>

<audio controls>
<source src="https://files.catbox.moe/ymuima.mp3" type="audio/mpeg">
</audio>

</section>



<!-- OTHER ANIMALS -->
<section id="other animals">

<div class="title">VVVVV  Other Animals</div>

<form>
<fieldset>
First name: <input type="text" name="firstname"><br><br>
Last name: <input type="text" name="lastname"><br><br>
Email: <input type="text" name="email"><br><br>

Would you like to plan?
<input type="radio" name="A" value="yes"> Yes
<input type="radio" name="B" value="no"> No

<br><br>

Interests:<br>
<input type="checkbox"> A
<input type="checkbox"> B
<input type="checkbox"> C

<br><br>

Days:
<select name="days">
<option>3 days</option>
<option>5 days</option>
<option>7 days</option>

</select>

<br><br>

Notes:<br>
<textarea rows="3" cols="50"></textarea>

</fieldset>

<br>
<input type="submit" value="Submit">
<input type="reset" value="Reset">
</form>

</section>



<!-- JAVASCRIPT -->
<script>
function showPage(pageId) {

let pages = document.querySelectorAll("section");

pages.forEach(p => {
p.classList.remove("active");
});

document.getElementById(pageId).classList.add("active");
}
</script>

</body>
</html>
