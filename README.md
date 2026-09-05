🎮 [Play Echo of Choices](https://meme-random-card-game-tmxiaf8penynnrd6rgkzdc.streamlit.app/)

🃏 Simple Card Game

A simple and flexible card-drawing game built with Python and Streamlit.

This project is designed to be easy to customize and reuse. The card system is separated from the visual content, allowing you to create different types of card games without rebuilding the entire system.

Just add your images to the "nanami" folder, organize them by rarity, and run the game.

✨ Features

- 🎲 Random card drawing
- ⭐ Rarity-based drop rates
- 🖼️ Automatically loads images from folders
- 📦 Card collection system
- 🔢 Tracks duplicate cards
- 🎨 Simple dark-themed interface
- 🛠️ Easy to customize
- 🔄 Reusable for different card game themes

📁 Folder Structure

project/
│
├── meme_game.py
├── README.md
│
└── nanami/
    ├── Common/
    │   ├── image1.png
    │   ├── image2.jpg
    │   └── ...
    │
    ├── Rare/
    │   ├── image1.png
    │   └── ...
    │
    ├── Epic/
    │   ├── image1.png
    │   └── ...
    │
    └── Legendary/
        ├── image1.png
        └── ...

The folder name determines the card's rarity:

- Common — Common cards
- Rare — Rare cards
- Epic — Epic cards
- Legendary — Legendary cards

Supported Image Formats

- ".jpg"
- ".jpeg"
- ".png"
- ".webp"

Simply place your images inside the appropriate rarity folder.

🎲 Drop Rates

The default drop rates are:

Rarity| Drop Rate
Legendary| 5%
Epic| 15%
Rare| 30%
Common| 50%

The game first selects a rarity based on the drop rates, then randomly selects an image from that rarity's folder.

You can easily change the drop rates in "meme_game.py".

🧩 Simple & Flexible

The main idea of this project is to keep the system simple while making the content easy to replace.

The code handles the card system, while the images are stored separately in the "nanami" folder.

This means you can change the theme simply by replacing or adding images.

For example, the same system can be used to create:

- 😂 Meme cards
- 🐱 Animal cards
- ⚔️ Fantasy cards
- 🎮 Game character cards
- 🤖 AI cards
- 🏎️ Racing cards
- 🌌 Sci-fi cards
- Or any theme you want

You don't need to rewrite the entire game.

Just:

Add images
     ↓
Put them into the rarity folders
     ↓
Run the game
     ↓
Start collecting

⚙️ Customization

Card-related settings such as names, descriptions, power values, colors, and drop rates can be customized directly in "meme_game.py".

For example:

DROP_RATE = {
    "Legendary": 5,
    "Epic": 15,
    "Rare": 30,
    "Common": 50
}

Modify these values to create your own card system.

▶️ Run the Game

1. Install Streamlit

pip install streamlit

2. Run the Game

streamlit run meme_game.py

The game will start locally and open in your web browser.

💡 Philosophy

This project follows a simple idea:

«Simple system. Flexible content.»

The goal isn't to create one specific card game, but to provide a simple system that can be reused for many different ideas.

Change the images.
Change the card data.
Create a completely different game.

One system, many possibilities. 🃏✨
