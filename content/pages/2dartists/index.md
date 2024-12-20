+++
title = ''
date = 2024-08-12T19:33:18+02:00
draft = false
+++

<style>
.grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* Exactly 3 columns */
    gap: 20px; /* Space between cards */
}

.card {
    display: flex;
    flex-direction: row;
    align-items: center;
    background-color: #1e1e1e;
    border-radius: 12px;
    padding: 10px;
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
    font-size: 4rem;
    font-weight: bold;
    margin-bottom: 60px;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 0.5rem;
    margin-top: 0.5rem;
}
@media (min-width: 768px) {
    .social-links {
        justify-content: flex-start;
    }
}
.social-link {
    width: 0.5rem;
    height: 0.5rem;
    border-radius: 50%;
    background-color: rgba(255, 255, 255, 0.1);
    color: #ffffff;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    transition: transform 0.3s, background-color 0.3s;
}
.social-link:hover {
    transform: scale(1.1);
    background-color: rgba(255, 255, 255, 0.2);
    border-radius: 50%;
}

.social-link:hover svg {
    fill: #d97706
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
                <img src="https://coolkoinu.carrd.co/assets/images/image03.png?v=275d7404" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">CoolKoinu</span>
                <div class="social-links">
                        <a href="https://x.com/CoolKoinu" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                        <a href="https://bsky.app/profile/coolkoinu.bsky.social" class="social-link" aria-label="Bluesky">
                            <i class="fab fa-bluesky"></i>
                        </a>
                        <a href="https://coolkoinu.carrd.co/" class="social-link" aria-label="Website">
                            <i class="fa fa-globe"></i>
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
                <img src="https://pbs.twimg.com/profile_images/1845244376446009345/vxh_z69v_400x400.jpg" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Colvery</span>
                <div class="social-links">
                        <a href="https://x.com/Colvyri" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                        <a href="https://bsky.app/profile/colvery.bsky.social" class="social-link" aria-label="Bluesky">
                            <i class="fab fa-bluesky"></i>
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
                <img src="https://pbs.twimg.com/profile_images/1801716228878176257/JCswU1h8_400x400.jpg" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">SirBurnt</span>
                <div class="social-links">
                        <a href="https://x.com/Sir_Burnt" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                        <a href="https://bsky.app/profile/sirburnt.bsky.social" class="social-link" aria-label="Bluesky">
                            <i class="fab fa-bluesky"></i>
                        </a>
                        <a href="https://sirburnt.carrd.co/" class="social-link" aria-label="Website">
                            <i class="fa fa-globe"></i>
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
                <img src="https://nekotiating.carrd.co/assets/images/image01.png?v=5e1a2467" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Nekotiating</span>
                <div class="social-links">
                        <a href="https://nekotiating.carrd.co/" class="social-link" aria-label="Website">
                            <i class="fa fa-globe"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-style">Toony</span>
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