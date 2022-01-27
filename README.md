# Introducao_WebScraping
Uilizando BeautifulSoup.
<h6>import requests
from bs4 import BeautifulSoup


resposta = requests.get('https://g1.globo.com/')
content = resposta.content

site = BeautifulSoup(content, 'html.parser')

reg = site.find('div', attrs={'class': 'feed-post-body'} )
print(reg.prettify())
</h6>
