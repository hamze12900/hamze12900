import requests
    import json
      
    url = "https://api.chapa.co/v1/transaction/initialize"
    payload = {
    "amount": "10",
    "currency": "ETB",
    "email": "abebech_bekele@gmail.com",
    "first_name": "Bilen",
    "last_name": "Gizachew",
    "phone_number": "0912345678",
    "tx_ref": "chewatatest-6669",
    "callback_url": "https://webhook.site/077164d6-29cb-40df-ba29-8a00e59a7e60",
    "return_url": "https://www.google.com/",
    "customization": {
    "title": "Payment for my favourite merchant",
    "description": "I love online payments"
    }
    }
    headers = {
    'Authorization': 'Bearer CHASECK-xxxxxxxxxxxxxxxx',
    'Content-Type': 'application/json'
    }
      
    response = requests.post(url, json=payload, headers=headers)
    data = response.text
    print(data)

<!---
hamze12900/hamze12900 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
