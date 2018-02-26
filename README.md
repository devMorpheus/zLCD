# zLCD
Arduino library for ST7920

Функции библиотеки:

Инициализация аппартной spi 1 или 2 шины
  initHwSpi(номер spi, пин rs)

Инициализация аппартной spi  шины  
  initHwSpi(пин rs)

Инициализация программной spi  шины   
  initSwSpi(пин rs, пин e, пин rw)

Инициализация 8 битной параллельной шины  
  init8bit(пины d0-d7, пин rs, пин e, пин rw)

Инициализация дисплея выполняется после инициализации одной из шин  
  begin()

Отключение аппаратного spi давая возможность другим библиотекам использовать spi шину с иной частотой sck
  free_spi()

Выставить шрифт   
  setFont(размер шрифта по x, размер шрифта по y, имя шрифта)

Инвертирование цвета шрифта
  invertingText(1/0 или true/false)

Нарисовать текст
  drawText(координата x, координата y, текст или переменная)

Продолжить рисовать текст, выполняется после drawText, продолжит рисовать после последнего символа
  resumeDrawText(текст или переменная)

Нарисовать пиксель  
  drawPixel(координата x, координата y, цвет 1/0)

Нарисовать горизонтальную линию
  drawHLine(координата x, координата y, длина линии, толщина линии, цвет 1/0)

Нарисовать вертикальную линию
  drawVLine(координата x, координата y, длина линии, толщина линии, цвет 1/0)

Нарисовать коробку с рамкой
  drawBox(координата x, координата y, ширина коробки, высота коробки, толщина рамки, цвет 1/0)

Нарисовать залитую коробку  
  drawFillBox(координата x, координата y, ширина коробки, высота коробки, цвет 1/0)

Нарисовать круг  
  drawCircle(координата x, координата y, радиус, цвет 1/0)

Нарисовать массив изображения  
  drawBitmap(координата x, координата y, ширина, высота, массив, цвет 1/0)

Заполнить буфер arduino  
  fillBuffer(цвет заполнения 1/0)

Очистить буфер arduino
  clearBuffer()

Очистить дисплей, тип отчиски 0 - быстрый, 1 - красивый
  clear(тип очистки, цвет очистки 1/0)

Отправить буфер arduino в дисплей  
  sendBuffer(тип отправки)
