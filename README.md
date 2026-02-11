[index.html](https://github.com/user-attachments/files/25234286/index.html)
<div id="secret" style="display:none; position:relative; overflow:hidden;">
  <h2>💖 My Promise to You 💖</h2>
  <div id="letter" style="font-size:1.2em; line-height:1.6; white-space:pre-wrap;"></div>

  <!-- Romantic photo collage -->
  <div id="photos" style="margin-top:30px; display:flex; flex-direction:column; align-items:center;"></div>

  <!-- Glowing finale text -->
  <div id="finale" style="display:none; margin-top:40px; font-size:2em; font-weight:bold; color:#b30059; text-shadow:0 0 10px #ff99cc, 0 0 20px #ff66b2;">
    💍 I love you forever 💍
  </div>

  <!-- Floating hearts container -->
  <div id="hearts"></div>
</div>

<style>
  /* Floating hearts style */
  #hearts {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    overflow: hidden;
  }
  .heart {
    position: absolute;
    color: #ff3366;
    font-size: 24px;
    animation: floatUp 6s linear infinite;
    opacity: 0.8;
  }
  @keyframes floatUp {
    0% { transform: translateY(100vh) scale(0.8); opacity: 0.8; }
    50% { opacity: 1; }
    100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
  }
</style>

<script>
  function typeLetter(text, elementId, callback) {
    let i = 0;
    function typing() {
      if (i < text.length) {
        document.getElementById(elementId).textContent += text.charAt(i);
        i++;
        setTimeout(typing, 50); // typing speed
      } else {
        if (callback) callback();
      }
    }
    typing();
  }

  function revealLetter() {
    const message = `
I know sometimes you feel I don’t give you first priority…
But the truth is, you are not just my first priority — you are my only one.

You thought I was cheating, or hiding behind games, but that was never true.
I was never good at chatting until you came into my life.
I started learning it only for you, because before you, I never talked to anyone like this.
You changed me, ra bangaram.

I waited for your messages, your calls, and when you entered my life, it felt like a dream.
Every year, month, day, hour, minute, second — you are my soulmate, my wife, my everything.

I promise I will never leave you. I will fight until my last breath for you.
I will never cheat you. I just need your support, and I know you will stand beside me.
I will always respect your ideas, your words, your alochanalu.
If I am wrong, tell me. If I lie, punish me. Because listening to my wife is my duty.

Time keeps ticking, but I miss you every single day.
I promise I will never break my promise.
I will fight and fix everything with you.

Last but not least… I love you, nukaalu.

Yours forever,
Your soulmate — mi bava 💍
    `;

    typeLetter(message, "letter", () => {
      revealPhotos();
    });
  }

  function revealPhotos() {
    const photoList = [
      "photo1.jpeg",
      "photo2.jpeg",
      "photo3.jpeg",
      "photo4.jpeg",
      "photo5.jpeg",
      "photo6.jpeg",
      "photo7.jpeg",
      "photo8.jpeg",
      "photo9.jpeg"
    ];

    const container = document.getElementById("photos");

    photoList.forEach((src, i) => {
      const img = document.createElement("img");
      img.src = src;
      img.alt = "Promise Photo";
      img.style.opacity = 0;
      img.style.transition = "opacity 1.5s ease-in";
      img.style.maxWidth = "350px";
      img.style.borderRadius = "15px";
      img.style.margin = "15px 0";
      img.style.boxShadow = "0 4px 10px rgba(0,0,0,0.3)";
      container.appendChild(img);

      setTimeout(() => {
        img.style.opacity = 1;
        // After last photo, show finale text + hearts
        if (i === photoList.length - 1) {
          setTimeout(() => {
            document.getElementById("finale").style.display = "block";
            startHearts();
          }, 3000);
        }
      }, i * 3000); // each photo fades in every 3 seconds
    });
  }

  function startHearts() {
    const heartsContainer = document.getElementById("hearts");
    setInterval(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.textContent = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = (20 + Math.random() * 20) + "px";
      heartsContainer.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }, 500); // new heart every 0.5s
  }
</script>
![photo1 jpeg](https://github.com/user-attachments/assets/3a20f895-aead-4e3d-8195-ce16ae0e87ec)
![photo2 jpeg](https://github.com/user-attachments/assets/836351b5-8042-4bbe-838e-924efe94016c)
![photo3 jpeg](https://github.com/user-attachments/assets/94c9bd29-1f0d-4f4b-a787-9b5cfe68b7b7)
![photo4 jpeg](https://github.com/user-attachments/assets/c4d3b8ff-1b07-4823-b94e-691315149fbd)
![photo5 jpeg](https://github.com/user-attachments/assets/1e586468-d948-48dd-b4fa-cb347145262c)
![photo6 jpeg](https://github.com/user-attachments/assets/ff492e21-9761-4bad-a11f-70e560bcc0c7)
![photo7 jpeg](https://github.com/user-attachments/assets/7f640b6c-a0e2-458d-876c-c0ae0e0b83c0)
![photo8 jpeg](https://github.com/user-attachments/assets/d90af07b-ad42-4ae6-85ba-fcc3495801cd)
![photo9 jpeg](https://github.com/user-attachments/assets/d74a4b2b-49d1-497c-910e-6b55cae708d5)
![photo10 jpeg](https://github.com/user-attachments/assets/33c58bfd-f103-4b85-8a85-e3756894ba91)
