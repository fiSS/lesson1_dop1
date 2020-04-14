# Модальные окна

## Usage
  1. При помощи querySelector получить со страницы кнопку ('.more'), само модально окно с классом overlay: document.querySelector('.overlay') и крестик document.querySelector('.popup-close').
  
  2. Открытие модального окна. Повесил обработчи событий на кнопку, что при клике на "more" запускается функция, что при клике на эту кнопку "overlay" должен изменять свои стили overlay.style.display = "block" принимает блочную модель, так же применяется анмация прописанная в css: (при помощи "this" обращаемся к кнопке непосредственно на которую нажали) this.classList.add('more-splash') Добавляем новый class,
  для блокировки скролла при открытии модального окна document.body.style.overflow = 'hidden' из стилей.
  3. Закрытие модального окна, на "close" навесить обработчик событий клика и выполняются обратные операции как в открытии окна.
