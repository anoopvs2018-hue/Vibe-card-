<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Tap Vibe - ANOOP V S</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

body {
    background: #f2f4f7;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
}

.card {
    width: 100%;
    max-width: 420px;
    background: white;
    border-radius: 25px;
    padding: 30px 22px;
    text-align: center;
    box-shadow: 0 10px 35px rgba(0,0,0,0.12);
}

.logo {
    width: 90px;
    height: 90px;
    margin: 0 auto 15px;
    border-radius: 50%;
    background: linear-gradient(135deg, #111, #555);
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 25px;
    font-weight: bold;
}

h1 {
    font-size: 28px;
    margin-bottom: 5px;
    color: #111;
}

.company {
    font-size: 17px;
    color: #777;
    margin-bottom: 8px;
}

.profession {
    display: inline-block;
    background: #111;
    color: white;
    padding: 7px 16px;
    border-radius: 20px;
    font-size: 14px;
    margin-bottom: 25px;
}

.buttons {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
}

.button {
    text-decoration: none;
    padding: 15px 10px;
    border-radius: 15px;
    background: #f1f2f4;
    color: #111;
    font-size: 15px;
    font-weight: bold;
    display: block;
}

.save {
    grid-column: 1 / -1;
    background: #111;
    color: white;
}

.qr-section {
    margin-top: 25px;
    padding-top: 20px;
    border-top: 1px solid #eee;
}

.qr-section h3 {
    margin-bottom: 12px;
    font-size: 17px;
}

#qrcode {
    display: flex;
    justify-content: center;
}

.footer {
    margin-top: 22px;
    color: #999;
    font-size: 12px;
}
</style>
</head>

<body>

<div class="card">

    <div class="logo">TV</div>

    <h1>ANOOP V S</h1>

    <div class="company">Tap Vibe</div>

    <div class="profession">Freelancer</div>

    <div class="buttons">

        <a class="button" href="tel:+971525670646">
            📞 Call
        </a>

        <a class="button"
           href="https://wa.me/971525670646"
           target="_blank">
            💬 WhatsApp
        </a>

        <a class="button"
           href="mailto:anoopvs2018@gmail.com">
            📧 Email
        </a>

        <a class="button"
           href="https://www.instagram.com/be_water_m.y_friend/"
           target="_blank">
            📸 Instagram
        </a>

        <a class="button"
           href="https://www.google.com/maps?q=24.4305,54.3589"
           target="_blank">
            📍 Location
        </a>

        <a class="button save"
           href="anoop.vcf"
           download="ANOOP_VS.vcf">
            👤 Save Contact
        </a>

    </div>

    <div class="qr-section">
        <h3>Scan My Tap Vibe Card</h3>
        <div id="qrcode"></div>
    </div>

    <div class="footer">
        Powered by Tap Vibe
    </div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>

<script>
const cardURL = "https://anoopvs2018-hue.github.io/Tap-vibe-card/";

new QRCode(document.getElementById("qrcode"), {
    text: cardURL,
    width: 180,
    height: 180
});
</script>

</body>
</html>
