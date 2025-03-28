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
   
