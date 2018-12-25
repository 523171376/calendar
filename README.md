# calendar

var data = [
			{
				"day": "2018-12-11",
				"type": "1",
				"id": "xxdd00xxxx",
				"room":[
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "1"
					}
				]
			},
			{
				"day": "2018-12-12",
				"type": "2",
				"room":[
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "1"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					}
				]
			},
			{
				"day": "2018-12-13",
				"type": "3"
			},
			{
				"day": "2018-12-14",
				"type": "4",
				"room":[
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "1"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "1"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "3",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "1"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					},
					{
						"meetting": [
							{
								"meetId": "xxdd00xxxx",
								"type": "1",
								"booked": "1"
						   },
						   {
								"meetId": "xxdd00xxxx",
								"type": "2",
								"booked": "0"
						   }
						],
						"roomId": "xxdd00xxxx",
						"type": "2"
					}
				]
			}
		];

// 初始化
WC.calender.init({
selecter: 'calendar_container',
toolbar: 'calendar_toolbar',
currentData: data,
preMonth: {
'btn': 'wc_pre_month',
'call': function(preTime){
setTimeout(function(){
WC.calender.load(data3, preTime);
}, 1000 * 2);
}
},
nextMonth: {
'btn': 'wc_next_month',
'call': function(nextTime){
setTimeout(function(){
WC.calender.load(data2, nextTime);
}, 1000 * 2);
}
},
dayClick: function(arg){
//				console.log(arg.day);
//				console.log(arg.id);
//				console.log(arg.room.length);
}, 
roomClick: function(arg){
//				console.log(arg.booked);
//				console.log(arg.meetId);
}
});
