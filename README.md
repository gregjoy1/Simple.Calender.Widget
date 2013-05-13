Simple.Calender.Widget
======================

A simple, easily customizable calender widget written in Javascript.
Avoided using JQuery simply because I really didn't need it...

Anyone is free to contribute, and tell me the downfalls of this script (everyone was a noob once - I'm still one).

Demo: http://www.gregjoy.co.uk/static/pages/SimpleCalenderWidget/

To use this widget, include it and call:

SimpleCalenderWidget.initialise(<Desired parent DOM element>, <optional event data>);

You can set this event data afterwards if preferred with:

SimpleCalenderWidget.setEventData(<event data>);

The layout of the event data is:

eventData = 
{
	year:{
		month:{
			day:[
				event:{
					id:id,
					time:time,
					title:title
				},
			],
		},
	},
}

Example:

eventData = 
{
	2013:{
		5:{
			10:[
				0:{
					id:'12',
					time:'09:00',
					title:'Nice title text'
				},
				1:{
					id:'13',
					time:'13:30',
					title:'Another nice title text'
				},
			],
			11:[
				0:{
					id:'11',
					time:'09:00',
					title:'Some text'
				}
			]
		},
	},
}

For any complaints, questions, constructive advice or criticism, I encourage you wholeheartedly to contact me.