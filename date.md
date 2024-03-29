# Date

|                                                                                                                                                                                                                                                                  |         |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| [How to get Date values with vanilla JavaScript](https://gomakethings.com/how-to-get-date-values-with-vanilla-javascript/)                                                                                                                                       | 4/14/23 |
| [Automatic night mode with vanilla JS](https://gomakethings.com/automatic-night-mode-with-vanilla-js/)                                                                                                                                                           | 12/7    |
| [How to create and work with timestamps in vanilla JS](https://gomakethings.com/how-to-create-and-work-with-timestamps-in-vanilla-js/?mc\_cid=2d3f04ec35\&mc\_eid=\[UNIQID])                                                                                     | 9/26    |
| [How to get the relative time between two dates with vanilla JS](https://gomakethings.com/how-to-get-the-relative-time-between-two-dates-with-vanilla-js/?mc\_cid=0cd90d97a3\&mc\_eid=\[UNIQID])                                                                 | 9/23    |
| [How to get the date N seconds, minutes, hours, or days in the past or future with vanilla JS](https://gomakethings.com/how-to-get-the-date-n-seconds-minutes-hours-or-days-in-the-past-or-future-with-vanilla-js/?mc\_cid=b7bc299017\&mc\_eid=\[UNIQID])        | 9/22    |
| [Converting and formatting dates and times with the vanilla JS Intl.DateTimeFormat() constructor](https://gomakethings.com/converting-and-formatting-dates-and-times-with-the-vanilla-js-intl.datetimeformat-constructor/?mc\_cid=1e27b71591\&mc\_eid=\[UNIQID]) | 8/27    |
| [https://epoch.now.sh/](https://epoch.now.sh/)                                                                                                                                                                                                                   |         |
| [https://date-fns.org/](https://date-fns.org/)                                                                                                                                                                                                                   |         |

### Static methods

|                                                                                                      |                                                                                                            |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| [.now()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/Date/now) | The **`Date.now()`** method returns the number of milliseconds elapsed since January 1, 1970 00:00:00 UTC. |
| [.getMonth()](https://gomakethings.com/getting-formatted-months-with-vanilla-js/)                    | 1/8/2020                                                                                                   |
| .getTime()                                                                                           |                                                                                                            |

{% code title="Timestamp math" %}
```javascript
var second = 1000;
var minute = 1000 * 60;
var hour = 1000 * 60 * 60;
var day = 1000 * 60 * 60 * 24;
var week = 1000 * 60 * 60 * 24 * 7;
var year = 1000 * 60 * 60 * 24 * 7 * 52;

//Multiply the number of time units you want by the formula above.
//For example, to jump 11 hours in the future or past
//you would multiply the hour numbers above by 11.
```
{% endcode %}

| libraries                                      |       |
| ---------------------------------------------- | ----- |
| [https://momentjs.com/](https://momentjs.com/) | 10/19 |
