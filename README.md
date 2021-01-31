# Video Game Skin Rater

A skin is an item that players purchase to change the appearance of their avatar. This item is purely for cosmetics and give no player advantage since Fortnite (which is what this data is based on) only uses one type of hitbox. Found in `skin_rater.ipynb`, this is a project that **1) analyzes the trends of Fortnite users regarding the skins that Epic Games produce** and **2) aims to predict how much these users would like future skins.** 

Data were scraped from https://progameguides.com/fortnite-skins-list/ using BeautifulSoup and are saved under `fortnite_skins.csv`. Two separate models were attempted - one to analyze images only and one that incorporates categorical data (whether the skin is male/female, a holiday skin, etc.) through an ensemble.


## Use Cases
**This is a useful project for both providers and consumers.**
* **Providers:** The gaming company would want to know if their players would like the skin they designed and plan on releasing. They have two use cases. First, they can price the skin according to the predicted rating. If it receives a high rating from the model, they can price the skin accordingly and charge more money. Second, they can edit the skin if it receives a low predicted rating.
  * Note: Markets within video games also have very limited space. For example, Valorant only displays 4 skins within one day. If a skin is rated high, providers will know to put the skin in the shop more often than disliked skins (if rarity isn't a factor).
* **Consumers:** Consumers care about how their friends and other players will like the skin they want to buy. This model predicts how the community as a whole will judge a skin.
