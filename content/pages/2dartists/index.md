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
    flex-direction: center; /* Stack elements vertically */
    justify-content: space-between;
    background-color: #1e1e1e;
    border-radius: 12px;
    padding: 15px;
    border: 2px solid #ffffff;
    box-sizing: border-box;
}

.card .artist-info {
    display: flex;
    align-items: center;
    gap: 10px;
    width: fit-content;
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
    align-items: center;
    justify-content: flex-start; /* Align to the left */
    gap: 8px;
    margin-top: 50px; /* Space above icons */
    margin-left: 60px; /* Align icons under artist name */
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
    flex-direction: column; /* Tags in a row */
    gap: 5px; /* Space between tags */
    margin-top: auto; /* Push tags to the bottom of the card */
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

<div class="grid" id="card-grid">
    <div class="card">
        <div class="artist-info">
            <img src="https://via.placeholder.com/50" alt="Artist">
            <span class="name">Teeeeest</span>
            <div class="icons">
                <span style="background-color: #f56;"></span>
                <span style="background-color: #f90;"></span>
                <span style="background-color: #09f;"></span>
            </div>
        </div>
        <div class="tags">
            <span class="tag tag-sfw">SFW</span>
            <span class="tag tag-nsfw">NSFW</span>
        </div>
    </div>
    <!-- Additional cards here -->
</div>

<script>
    // Shuffle function
    function shuffle(array) {
        for (let i = array.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1));
            [array[i], array[j]] = [array[j], array[i]];
        }
    }

    // Example card data (dynamic cards)
    const cards = [
        `<div class="card">
            <div class="artist-info">
                <img src="placeholder.png" alt="Artist">
                <span class="name">Weewoothefirst</span>
            </div>
            <div class="icons">
                <span style="background-color: #f56;"></span>
                <span style="background-color: #f90;"></span>
                <span style="background-color: #09f;"></span>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-nsfw">NSFW</span>
            </div>
        </div>`,
        `<div class="card">
            <div class="artist-info">
                <img src="placeholder2.png" alt="Artist">
                <span class="name">Colvery</span>
            </div>
            <div class="icons">
                <span style="background-color: #5f5;"></span>
                <span style="background-color: #ff5;"></span>
                <span style="background-color: #05f;"></span>
            </div>
            <div class="tags">
                <span class="tag tag-sfw">SFW</span>
                <span class="tag tag-nsfw">NSFW</span>
            </div>
        </div>`
    ];

    // Shuffle and append dynamic cards
    const grid = document.getElementById('card-grid');
    shuffle(cards); // Shuffle the cards array
    grid.innerHTML += cards.join(''); // Append shuffled cards to the existing ones
</script>