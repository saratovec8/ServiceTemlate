# ServiceTemlate
Cервис для создания шаблонов для исков в суд

Default ветка - corrections.

Основой является сервер на Django. Есть 2 модели - TextAlias и Template (ее надо бы убрать за ненадобностью).

С frontend'a с помощью axios данные с формы отправляются на backend, где во views.py создается документ .docx. Для рендеринга этот документ конвертируется в .pdf (нужна утилита для linux unoconv, для windows есть свои аналоги), после чего отображается на странице в <canvas>.

Шаблон всей страницы находится в index.html. Весь JS код находится в static
