Nivo Slider Widget for Yii2
========================
A customizable nivo slider plugin for Yii2.

Installation
------------
The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require "amilna/yii2-nivo-slider" "*"
```

or add

```json
"amilna/yii2-nivo-slider" : "*"
```
to the require section of your application's `composer.json` file.

Since this extensions stil in dev stages, be sure also add following line in `composer.json` file.


Usage
-----
In view:

```php

use amilna\nivoslider\NivoSlider;

echo NivoSlider::widget([
		'dataProvider'=>$dataProvider, // active data provider or just image array
		'targetId'=>'nivoslider',	//id of rendered nivoslider (the container will constructed by the widget with the given id)		
		'imageKey'=>'image', //model attribute to be used as background
		'theme' => 'default', //available themes: default, bar, dark, light
 
 		'css' => '', // url of css to overide default css relative from @web	  		
		
		
		//	example to overide default options	more options on http://docs.dev7studios.com/jquery-plugins/nivo-slider
		'options'=>[
				'effect'=> 'boxRandom',
				'manualAdvance'=>false,
				'controlNav'=> false				
			],		
		 						
 	]); 
```
