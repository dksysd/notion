# notion dday formula
`empty(prop("End")) ? "free" : if(formatDate(end(prop("End")), "YYYY,MM,DD") == formatDate(now(), "YYYY,MM,DD"), "D-day", if(end(prop("End")) < now(), concat("D+", format(dateBetween(end(prop("End")), now(), "days") * -1)), concat("D-", format(dateBetween(end(prop("End")), now(), "days") + 1))))`
### Example
![SmartSelect_20210927-120412_Notion](https://user-images.githubusercontent.com/59986697/134839829-4c2cd7eb-3e05-4d29-9f2f-51635e70db7b.jpg)
