const int buttonPin = 2; // Пин кнопки
const int buttonPin2 = 10; // Пин кнопки
const int ledPin = 13; // Пин светодиода
const int ledPin2 = 7;
int buttonState = 0; // Переменная для хранения состояния кнопки
int buttonState2 = 0;


void setup() {
 pinMode(ledPin, OUTPUT); // Настройка пина светодиода как выхода
 pinMode(buttonPin, INPUT); // Настройка пина кнопки как входа
 pinMode(ledPin2, OUTPUT); // Настраиваем пин 7 как выход
 pinMode(buttonPin2, INPUT); // Настройка пина кнопки как входа
}
void loop() {
 buttonState = digitalRead(buttonPin); // Считываем состояние кнопки
  buttonState2 = digitalRead(buttonPin2); // Считываем состояние кнопки

 if (buttonState == 0) { // Если кнопка нажата
 digitalWrite(ledPin, HIGH); // Включаем светодиод
 } else {
 digitalWrite(ledPin, LOW); // Выключаем светодиод
 }
 if(buttonState2 == 0){
  digitalWrite(ledPin2, HIGH); // Включаем светодиод
   delay(100); // Задержка 0,1 секунд
 //} else {

 digitalWrite(ledPin2, LOW); // Выключаем светодиод

delay(300); // Задержка 0,3 секунд
 }


 }







