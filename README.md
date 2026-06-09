<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vedant Digital Card</title>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: linear-gradient(135deg,#d3d3d3,#f5f5f5);
    display: flex;
    justify-content: center;
    padding: 15px;
}

.card {
    width: 100%;
    max-width: 400px;
    border-radius: 20px;
    overflow: hidden;
}

.header {
    background: #000;
    padding: 20px;
    border-radius: 20px;
    color: white;
}

.logo {
    text-align: center;
    margin-bottom: 10px;
    font-weight: bold;
    color: gold;
}

.profile {
    display: flex;
    align-items: center;
    gap: 15px;
}

.profile img {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    border: 2px solid white;
}

.info h2 {
    font-size: 16px;
}

.info p {
    font-size: 14px;
    opacity: 0.8;
}

.save-btn {
    margin-top: 15px;
    background: #777;
    color: white;
    text-align: center;
    padding: 10px;
    border-radius: 10px;
    cursor: pointer;
}

.save-btn:hover {
    background:#46c34c;
}

.item {
    background: #000;
    color: white;
    padding: 15px;
    border-radius: 10px;
    margin: 10px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
    transition: 0.3s;
}

.item:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(212,175,55,0.35);
}

.call-highlight {
    border: 1px solid gold;
}

.map iframe {
    width: 100%;
    height: 200px;
    border-radius: 10px;
    margin-top: 10px;
}

.footer {
    background:#000;
    display: flex;
    justify-content: center;
    padding: 15px;
}
</style>
</head>

<body>

<div class="card">

<div class="header">
    <div class="logo"><img src="download (5).jpg" width="360" height="100"></div>

    <div class="profile">
        <img src="WhatsApp Image 2026-06-09 at 6.17.24 PM.jpeg" alt="profile">
        <div class="info">
            <h2>Mr. Vedant Kalbande</h2>
			<p>CA Finalist</p>
            <p>Institute of Chartered Accountants of India</p>
        </div>
    </div>

    <div class="save-btn" onclick="saveContact()">Save Contact</div>
</div>

<div class="item call-highlight" onclick="callNow()">
    <span><i class="fa-solid fa-phone-volume" style="color:gold;"></i> Call</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="whatsapp()">
    <span><i class="fa-brands fa-whatsapp" style="color:gold;"></i> WhatsApp</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="instagram()">
    <span><i class="fa-brands fa-instagram" style="color:gold;"></i> Instagram</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="youtube()">
    <span>
        <i class="fa-brands fa-youtube" style="color:gold;"></i>
        YouTube
    </span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="linkedin()">
    <span><i class="fa-brands fa-linkedin" style="color:gold;"></i> LinkedIn</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="email()">
    <span><i class="fa-solid fa-envelope" style="color:gold;"></i> Email</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="website()">
    <span><i class="fa-solid fa-globe" style="color:gold;"></i> Website</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="map()">
    <span><i class="fa-solid fa-map" style="color:gold;"></i> Location</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="map">
  <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d12268.959012656296!2d79.14356385!3d21.1368559!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e1!3m2!1sen!2sin!4v1777024533849!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</div>

<div class="footer">
    <img src="Untitled design.jpg" width="80" height="80">
</div>

</div>

<script>

// ACTIONS
function callNow() {
    window.location.href = "tel:+918007795091";
}

function whatsapp() {
    window.open("https://wa.me/9834084471", "_blank");
}

function instagram() {
    window.open("https://instagram.com/vedannt7", "_blank");
}
	
function youtube() {
    window.location.href = "https://www.youtube.com/@mka.india.corp.youtube";
}

function linkedin() {
    window.open("https://linkedin.com",Vedant Kalbande "_blank");
}

function email() {
    window.location.href = "vedantkalbande@gmail.com";
}

function website() {
    window.open("https://www.madhukusumassociates.com", "_blank");
}

function map() {
    window.open("https://maps.app.goo.gl/JmyySgbAHcTFEjwv8", "_blank");
}

// VCARD DOWNLOAD
function saveContact() {
    const vcard = `BEGIN:VCARD
VERSION:3.0
FN:Vedant Kalbande
ORG:Madhu Kusum Associates
TEL:+919834084471
EMAIL:vedantkalbande.com
END:VCARD`;

    const blob = new Blob([vcard], { type: "text/vcard" });
    const url = URL.createObjectURL(blob);

    const a = document.createElement("a");
    a.href = url;
    a.download = "contact.vcf";
    a.click();
}

</script>

</body>
</html>

