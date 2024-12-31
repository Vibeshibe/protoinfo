+++
title = ''
date = 2024-08-12T19:33:18+02:00
draft = false
+++

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