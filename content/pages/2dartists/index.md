+++
title = ''
date = 2024-08-12T19:33:18+02:00
draft = false
+++

<style>
.grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Exactly 3 columns */
    gap: 20px; /* Space between cards */
}

.card {
    display: flex;
    flex-direction: row;
    align-items: center;
    background-color: #1e1e1e;
    border-radius: 12px;
    padding: 15px;
    gap: 35px;
    border: 2px solid #ffffff;
    box-sizing: border-box;
}

.card .artist-info {
    display: flex;
    align-items: center;
    gap: 10px;
    width: max-content;
}

.card .artist-info img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border: 2px solid #fff;
}

.card .artist-info .name {
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 30px;
}

.card .icons {
    display: flex;
    justify-content: flex-start;
    gap: 8px;
    width: fit-content;
}

.icons span {
    width: 20px;
    height: 20px;
    border-radius: 50%;
    background-color: #ffffff;
    display: inline-block;
}

.tags {
    display: flex;
    flex-direction: column;
    gap: 5px;
}

.tag {
    display: inline-block;
    padding: 5px 10px;
    font-size: 0.8rem;
    font-weight: bold;
    border-radius: 8px;
    text-transform: uppercase;
    text-align: center;
}

.tag-sfw {
    background-color: #4caf50;
    color: #fff;
}

.tag-nsfw {
    background-color: #f44336;
    color: #fff;
}

.tag-style {
    background-color: orange;
    color: #fff;
}
</style>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.0/css/all.min.css">

<div class="grid" id="card-grid">
<div class="card">
            <div class="artist-info">
                <img src="placeholder2.png" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Testy1</span>
                <div class="icons">
                        <a href="https://t.me/Zenonclaw" class="social-link" aria-label="Telegram">
                            <i class="fab fa-telegram-plane"></i>
                        </a>
                        <a href="https://zenonclaw.tumblr.com" class="social-link" aria-label="Tumblr">
                            <i class="fab fa-tumblr"></i>
                        </a>
                        <a href="https://x.com/zenonclaw" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-style">Realistic</span>
            </div>
        </div>

<div class="card">
            <div class="artist-info">
                <img src="placeholder.png" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Testy2</span>
                <div class="icons">
                        <a href="https://t.me/Zenonclaw" class="social-link" aria-label="Telegram">
                            <i class="fab fa-telegram-plane"></i>
                        </a>
                        <a href="https://zenonclaw.tumblr.com" class="social-link" aria-label="Tumblr">
                            <i class="fab fa-tumblr"></i>
                        </a>
                        <a href="https://x.com/zenonclaw" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-nsfw">NSFW</span>
                <span class="tag tag-style">Toony</span>
            </div>
        </div>

<div class="card">
            <div class="artist-info">
                <img src="placeholder.png" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Testy3</span>
                <div class="icons">
                        <a href="https://t.me/Zenonclaw" class="social-link" aria-label="Telegram">
                            <i class="fab fa-telegram-plane"></i>
                        </a>
                        <a href="https://zenonclaw.tumblr.com" class="social-link" aria-label="Tumblr">
                            <i class="fab fa-tumblr"></i>
                        </a>
                        <a href="https://x.com/zenonclaw" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-style">Toony</span>
            </div>
        </div>

<div class="card">
            <div class="artist-info">
                <img src="placeholder2.png" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Testy4</span>
                <div class="icons">
                        <a href="https://t.me/Zenonclaw" class="social-link" aria-label="Telegram">
                            <i class="fab fa-telegram-plane"></i>
                        </a>
                        <a href="https://zenonclaw.tumblr.com" class="social-link" aria-label="Tumblr">
                            <i class="fab fa-tumblr"></i>
                        </a>
                        <a href="https://x.com/zenonclaw" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-nsfw">NSFW</span>
                <span class="tag tag-style">Realistic</span>
            </div>
        </div>
        <-- Cards go above here-->
    </div>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const grid = document.querySelector('.grid'); // Get the grid container
        const cards = Array.from(grid.querySelectorAll('.card')); // Get all the card elements inside the grid

        // Randomly shuffle the array of cards
        for (let i = cards.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1)); // Get a random index
            [cards[i], cards[j]] = [cards[j], cards[i]]; // Swap the cards
        }

        // Clear the grid and append the shuffled cards
        grid.innerHTML = '';
        cards.forEach(card => grid.appendChild(card)); // Append each shuffled card back into the grid
    });
</script>