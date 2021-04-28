#Sollers Postman API automation testing

## Установка
1.	Установка Node.js, npm	
2.	Установка  newman	
sudo npm install -g newman
3.	Установка html reporter	
npm install -g newman-reporter-html
4.	Установка html-extra reporter	
npm install -g newman-reporter-htmlextra

## Запуск

*Подготовка параметров*  

`newman run postman_collections/API_Web-calc.postman_collection.json --folder prep_data`    

*Запуск полных тестов Калькулятора*  

`newman run postman_collections/API_Web-calc.postman_collection.json --folder WEB-calc-tests -e environment_variables/master_var.json -d iterations/API-Web-calc-year-mileage.json` 

*Быстрая проверка расчетов Калькулятора* 

`newman run postman_collections/API_Web-calc.postman_collection.json --folder WEB-calc-tests -e environment_variables/master_var.json -d iterations/API-Web-calc-year-mileage_short.json` 
