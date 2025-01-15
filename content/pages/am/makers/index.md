+++
title = ''
date = 2024-08-12T19:33:18+02:00
draft = false
+++

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.0/css/all.min.css">

<div class="grid" id="card-grid">
<div class="card">
            <div class="artist-info">
                <img src="https://pbs.twimg.com/profile_images/1633127743100420096/J6k-F1v3_400x400.jpg" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">Arget & Lazuli</span>
                <div class="social-links">
                        <a href="https://linktr.ee/argetandlazuli" class="social-link" aria-label="Website">
                            <i class="fa fa-globe"></i>
                        </a>
                        <a href="https://x.com/ArgetandLazuli" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                        <a href="https://bsky.app/profile/argetandlazuli.bsky.social" class="social-link" aria-label="Bluesky">
                            <i class="fab fa-bluesky"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-style">Maker</span>
            </div>
        </div>

<div class="card">
            <div class="artist-info">
                <img src="https://pbs.twimg.com/profile_images/1864417030251655168/ah_tCGkl_400x400.jpg" alt="Artist" class="medium-zoom-image">
            </div>
            <div style="
    display: flex;
    flex-direction: column;">
                <span class="name">FurbittenStudio</span>
                <div class="social-links">
                        <a href="https://linktr.ee/FurBittenStudios" class="social-link" aria-label="Website">
                            <i class="fa fa-globe"></i>
                        </a>
                        <a href="https://x.com/furbittenStudio" class="social-link" aria-label="Twitter">
                            <i class="fa-brands fa-x-twitter"></i>
                        </a>
                </div>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-style">Maker</span>
            </div>
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