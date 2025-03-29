# conference-database

1) API для поиска всех прошедших конференций:
   Crossref: https://api.crossref.org/works - пока этим пользовался, но он кажется не выдает по умолчанию ссылку на конфу, могу получить doi и название конфы.
   OpenAlex: https://api.openalex.org/sources - стоит попробовать, вдруг лучше первого варианта

2) Сайты-агрегаторы будущих конференций:
   ConferenceAlerts: https://conferencealerts.com
   All Conference Alert: https://www.allconferencealert.com
   WikiCFP: http://www.wikicfp.com/cfp (тут часто уже есть вся инфа и про даты, и про место, и про топики, и про коммитет даже иногда. ну и конечно сам урл на конференцию)

3) Пайплайн заполнение информации по будущим конференциям:
   Хожу по сайтам-агрегаторам из пункта 2, получаю урл, дату, место проведения. На сайте нахожу страницы speakers, topics и обрабатываю их с помощью llm.
   
# Основные ноутбуки:
   1. get_crossref_conference (colab)
   2. llm_conference (kaggle)

# Модели:
  gemma3 (4b params, 128k token context window)
  phi3:mini (3.8b params, 4k token context window)
  mistral (7b params, 32k token context window)
  deepseek-r1 (7b params, 128k token context window) 
  ...
