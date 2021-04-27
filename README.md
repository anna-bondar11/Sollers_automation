
Sollers_automation

newman run postman_collections/API_Web-calc.postman_collection.json  prep_data    

newman run postman_collections/API_Web-calc.postman_collection.json  WEB-calc-tests -e environment_variables/master_var.json -d iterations/API-Web-calc-year-mileage.json 