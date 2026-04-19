# 🚀 Warframe Market Price Checker

Hello! 👋 Welcome to this small repository. 

This is a **100% homemade, non-professional** project. I created it as a personal tool to quickly check the selling prices of certain items (mainly Arbitration and Syndicate mods) on [Warframe Market](https://warframe.market/). 

If you are tired of searching item by item on the website to figure out how much to sell your mods for, this little *Jupyter Notebook* does the dirty work for you by automatically querying the API.

## 🛠️ What exactly does it do?

* **Concurrent Requests**: It uses multiple threads (`ThreadPoolExecutor`) to fetch several items at once so you don't have to wait forever.
* **Seller Filter**: It only considers users who are currently online (`online` or `ingame`).
* **Price Calculation**: It grabs the 5 lowest selling prices for each item and calculates the **median** (average) to give you a suggested, realistic selling price.
* **Clean Format**: It displays all the data in a neat table using `pandas`, ready to read, with the item name formatted so you can easily copy and paste it into the game chat.

## ⚙️ Requirements

To run this Notebook on your computer, you will need Python installed along with a couple of libraries. You can install them by running:

```bash
pip install requests pandas notebook
