Readme file of Assignment

************ TASK2 Migration & seeding************

************  Commands to be executes************

1.php artisan migrate

2.php artisan db:seed -- class=CountriesTableSeeder

************ ************ ************ ************ ************ 



1.Once the project setup has been done.run the project.

2.You will see list available countries with ISO code

3.Filter- It will give you result of the selected country code.

************ INTERNAL WORKING OF TASK2 ************

1.You will see http://localhost:8000/ URL (vary according to your port no.)

2.Route 
	i.Location --LARAVEL_ROOT/routes/web.php
	
	ii.usage --
	Route::get('/', 'CountriesController@CountriesListView');

3.controller  
	i.location--LARAVEL_ROOT/app/Http/Controllers/CountriesController
	
	ii.CountriesController function checks wheather iso exist or not.
	
		-if not then it selects all the data from db else only filtered data.

4.VIEW
	i.location--LARAVEL_ROOT/resources/views/countries-list.blade.php 
	
	ii.what is .blade after view name --Blade is the simple, yet a powerful templating engine provided with Laravel.
	
	iii.use of blade template--- for reducing or simplifying the code that you write in your view
	
	e.g     <?php echo strtoupper('hello') ?>(PHP VIEW .php ) ==   {{strtoupper('hello')}} (BLADE VIEW .blade.php).
	
	iv.this view shows the list of  available countries
	

						   	


















