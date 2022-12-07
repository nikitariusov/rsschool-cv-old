# **Nikita Usov**

## **My contacts**

* **Location:** Dnipro, Ukraine
* **Telegram:** nikitariusov
* **Email:** nikitariusov@gmail.com
* **GitHub:**  [nikitariusov][gitHub]
* **Discord:** Nikita Usov (@nikitariusov)


## **About Me**

I am rapidly moving towards frontend and backend development. I am already making parsers for collecting data on the Internet, creating document processors, and parsers for collecting data for business, but I want to learn how to create interactive sites. I am constantly developing and I believe that nothing is impossible. To accomplish this task, I am ready to study new material, all new technologies are amenable to development.


## **Skills**

* Python 3 
* Python libraries: BeautifulSoup, Request, openpyxl
* HTML
* CSS
* JS
* Git
* PyCharm
* Visual Studio Code


## **Code Example**
### **Python** ###

```
from bs4 import BeautifulSoup
from Request import get_html, get_response


def pars_info(html_data):

    soup = BeautifulSoup(html_data, 'html.parser')
    cards_company = soup.find_all('div', class_='cart-company-lg')

    dict_keys = ["Название", "Сайт", "Почта", "Телефон",
                 "Вид деятельности"]
    data_base = []
    
    for card in cards_company:
        data_company = {}
        dict_value = []
        
        mail = card.find('a', target="_blank", rel=None)
        site = card.find('a', rel="nofollow", target="_blank")
```