# README
選課小幫手整個伺服器維護的操作手冊

## [CAL](https://github.com/Stufinite/cal)

每年都要把js的學期號碼更新
1. `cal/static/timetable/js/Timetable.js` -> 裏面的 `this.semester`
2. `cal/static/timetable/js/page.js` -> 裏面有兩個 `semester` 變數

## [scrawler](https://github.com/Stufinite/scrawler)

快要到下一次選課的時候

執行 `python run.py <新的學期數 e.q. 1071>`

## [inferno](https://github.com/Stufinite/slothTw)

每學期也都需要更新一下課程心得的條目

`python manage.py updateCourse 課程.json`：就可以插入新的課程到心得版，課程.json請去執行[scrawler專案](https://github.com/stufinite/scrawler)，執行完之後目錄下就會出現 `課程.json`
