Chatbot for food orders online delivery using Dialogflow
===================
Build a chatbot for food orders online delivery using Google's Dialogflow ES. This bot supports two options,

1) New Order
2) Track Order

3) New Order: Sample Conversation

```
Bot: How can I help you? You can say things like (1) New Order (2) Track Order
User: New Order
Bot: What would you like to have? You can say things like 2 pizzas, one vada pav.
     Only order from this list: Vada Pav, Pav Bhaji, Mango Lassi, Pizza, Rava Dosa, Masala Dosa, Samosa
User: I would like to have 2 Rava Dosa and one plate of samosa
Bot: Added 2 Rava Dosa and 1 Samosa. Anything else?
User: Oh yes, add one mango lassi, please
Bot: Sure. Now we have 2 Rava Dosa, 1 Samosa and 1 Mango Lassi. Anything else?
User: Well, you know my cholesterol came high so let's remove Samosa
Bot: Sure. Now we have 2 Rava Dosa, and 1 Mango Lassi. Anything else?
User: Nope. That's it
Bot: Awesome. Your order is placed. Order id # 45. Your total bill is 19$ which you can pay at the time of delivery!
```

2) Track Order: Sample Conversation

```Bot: How can I help you? You can say things like (1) New Order (2) Track Order
User: Track Order
Bot: What is your order id?
User: 45
Bot: Order # 45, is in transit
User: How about 41
Bot: ORder # 41 is delivered
```


Directory structure
===================
backend: Contains Python FastAPI backend code
db: contains the dump of the database. you need to import this into your MySQL db by using MySQL workbench tool
dialogflow_assets: this has training phrases etc. for our intents
frontend: website code

Install these modules
======================

pip install mysql-connector
pip install "fastapi[all]"

OR just run pip install -r requirements.txt to install both in one shot

To start fastapi backend server
================================
1. Go to backend directory in your command prompt
2. Run this command: uvicorn main:app --reload

ngrok for https tunneling
================================
1. To install ngrok, go to https://ngrok.com/download and install ngrok version that is suitable for your OS
2. Extract the zip file and place ngrok.exe in a folder.
3. Open windows command prompt, go to that folder and run this command: ngrok http 80000

NOTE: ngrok can timeout. you need to restart the session if you see session expired message.

Project Snapshots
===================

![Screenshot 2023-12-07 132244](https://github.com/stha1122/OrderEaseBot/assets/122188963/061da9a9-c2b0-488b-bfc7-641fc8724450)

![Screenshot 2023-12-07 132305](https://github.com/stha1122/OrderEaseBot/assets/122188963/e02ee4fe-9c66-4f06-b704-92e31537bb42)

![Screenshot 2023-12-07 132311](https://github.com/stha1122/OrderEaseBot/assets/122188963/34ed4c3b-bfe9-4db8-964a-fc69ca87007a)



