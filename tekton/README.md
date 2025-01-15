# Ngrok으로 github-eventlistener와 연결하여 Webhook 설정

ngrok config add-authtoken [your_token]

# option 1) Ephemeral Domain
ngrok http http:localhost:32000

# option 2) Static Domain
ngrok http --url=[your_static_domain]:[port]

ngrok을 통해 받은 주소를 webhook에 등록.