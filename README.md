<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>All Funny Memes - Movies & Shows</title>
    <style>
        body { font-family: Arial, sans-serif; background-color: #f0f0f0; text-align: center; }
        h1 { color: #333; }
        .category { margin: 20px; }
        .meme-gallery { display: flex; flex-wrap: wrap; justify-content: center; }
        .meme { margin: 10px; max-width: 300px; }
        img { width: 100%; height: auto; border-radius: 10px; }
    </style>
</head>
<body>
    <h1>Welcome to All Funny Memes!</h1>
    <p>allfunnymeme.com - Hilarious memes for every movie and TV show. Scroll and laugh!</p>

    <div class="category">
        <h2>Movies</h2>
        <div class="meme-gallery">
            <div class="meme">
                <img src="https://example.com/avengers-meme.jpg" alt="Avengers Meme">
                <p>Avengers: Infinity War Plot Twist</p>
            </div>
            <div class="meme">
                <img src="https://example.com/starwars-meme.jpg" alt="Star Wars Meme">
                <p>Star Wars: Force Be With You</p>
            </div>
            <!-- Add more movie memes here -->
        </div>
    </div>

    <div class="category">
        <h2>TV Shows</h2>
        <div class="meme-gallery">
            <div class="meme">
                <img src="https://example.com/friends-meme.jpg" alt="Friends Meme">
                <p>Friends: Central Perk Vibes</p>
            </div>
            <div class="meme">
                <img src="https://example.com/breakingbad-meme.jpg" alt="Breaking Bad Meme">
                <p>Breaking Bad: Chemistry Lessons</p>
            </div>
            <!-- Add more show memes here -->
        </div>
    </div>

    <script>
        // Simple search function
        function searchMemes() {
            const query = document.getElementById('search').value.toLowerCase();
            const memes = document.querySelectorAll('.meme');
            memes.forEach(meme => {
                const alt = meme.querySelector('img').alt.toLowerCase();
                meme.style.display = alt.includes(query) ? 'block' : 'none';
            });
        }
    </script>
    <input type="text" id="search" placeholder="Search memes..." onkeyup="searchMemes()">
</body>
</html>
