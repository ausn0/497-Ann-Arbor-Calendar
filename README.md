### Flutter calendar week
A calendar widget by week

[Dartdoc](http://indieteam.herokuapp.com/flutter-calendar-week/)


##### TODO:
- [ ] Publish to pub.dev

##### IOS | Android:
<img src="https://i.imgur.com/Qv78xwO.png" width="40%" height="40%"/> <img src="https://i.imgur.com/oUQYCbC.png" width="43.29%" height="42.45%"/>

<br>

#### Use:
```
dependencies:
  flutter_calendar_week:
    git:
      url: https://github.com/mduccc/flutter_calendar_week.git
      ref: 1.0.0
```

```Dart
CalendarWeek(
              controller: _controller,
              height: 100,
              showMonth: true,
              minDate: DateTime.now().add(
                Duration(days: -365),
              ),
              maxDate: DateTime.now().add(
                Duration(days: 365),
              ),
              
              onDatePressed: (DateTime datetime) {
                // Do something
              },
              onDateLongPressed: (DateTime datetime) {
               // Do something
              },
              onWeekChanged: () {
                // Do something
              },
              decorations: [
                DecorationItem(
                    decorationAlignment: FractionalOffset.bottomRight,
                    date: DateTime.now(),
                    decoration: Icon(
                      Icons.today,
                      color: Colors.blue,
                    )),
                DecorationItem(
                    date: DateTime.now().add(Duration(days: 3)),
                    decoration: Text(
                      'Holiday',
                      style: TextStyle(
                        color: Colors.brown,
                        fontWeight: FontWeight.w600,
                      ),
                    )),
              ],
            )
```
