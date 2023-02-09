# calender-and-text-animation
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="Text and Animation.css">
    <title>Text and Animation</title>
</head>
<body>
    <div class="container">
        <div class="calendar">
          <header>
            <h2>December 2020</h2>
            <a class="btn-prev fontawesome-angle-left" href="#"></a>
            <a class="btn-next fontawesome-angle-right" href="#"></a>
          </header>
      
          <table>
            <thead>
              <tr>
                <td>Mo</td>
                <td>Tu</td>
                <td>We</td>
                <td>Th</td>
                <td>Fr</td>
                <td>Sa</td>
                <td>Su</td>
              </tr>
            </thead>

            <tbody>
                <td class="prev-month"> </td>
                <td class="prev-month"> </td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>6</td>
                <td>7</td>
                <td>8</td>
                <td>9</td>
                <td>10</td>
                <td>11</td>
                <td>12</td>
                <td>13</td>
                <td>14</td>
                <td>15</td>
                <td>16</td>
                <td>17</td>
                <td>18</td>
                <td>19</td>
                <td>20</td>
                <td>21</td>
                <td>22</td>
                <td>23</td>
                <td>24</td>
                <td>25</td>
                <td>26</td>
                <td>27</td>
                <td>28</td>
                <td>29</td>
                <td>30</td>
              </tr>
            </tbody>
      
          </table>
      
        </div>
      </div>
</body>
</html>


#CSS
@import url(https://weloveiconfonts.com/api/?family=fontawesome);

*[class*="fontawesome-"]:before {
  font-family: 'FontAwesome', sans-serif;
}

body {
	background: #f9f9f9;
	color: #0e171c;
  display: grid;
	font: 300 100%/1.5em 'Lato', sans-serif;
	margin: 0;
  min-height: 100vh;
  place-items: center;
}

a {
	text-decoration: none;
}

h2 {
	font-size: 2em;
	line-height: 1.25em;
	margin: .25em 0;
}

h3 {
	font-size: 1.5em;
	line-height: 1em;
	margin: .33em 0;
}

table {
	border-collapse: collapse;
	border-spacing: 0;
}

.container {
	width: 510px;
}

.calendar {
	text-align: center;
}

.calendar header {
	position: relative;
}

.calendar h2 {
	text-transform: uppercase;
}

.calendar thead {
	font-weight: 600;
	text-transform: uppercase;
}

.calendar tbody {
	color: #7c8a95;
}

.calendar tbody td:hover {
	border: 2px solid #00addf;
}

.calendar td {
	border: 2px solid transparent;
	border-radius: 50%;
	display: inline-block;
	height: 4em;
	line-height: 4em;
	text-align: center;
	width: 4em;
}

.calendar .prev-month,
.calendar .next-month {
	color: #cbd1d2;
}

.calendar .prev-month:hover,
.calendar .next-month:hover {
	border: 2px solid #cbd1d2;
}

.current-day {
	background: #00addf;
	color: #f9f9f9;
}

.event {
	cursor: pointer;
	position: relative;
}


.event.current-day:after {
	background: #f9f9f9;
}

.btn-prev,
.btn-next {
	border: 2px solid #cbd1d2;
	border-radius: 50%;
	color: #cbd1d2;
	height: 2em;
	font-size: .75em;
	line-height: 2em;
	margin: -1em;
	position: absolute;
	top: 50%;
	width: 2em;
}

.btn-prev:hover,
.btn-next:hover {
	background: #cbd1d2;
	color: #f9f9f9;
}

.btn-prev {
	left: 6em;
}

.btn-next {
	right: 6em;
}

