# Best-Bite

CSS

/* Universal Styles */

html {
  font-family: 'Arvo', serif;
  font-size: 16px;
}

a {
  text-decoration: none;
}

.btn {
  display: inline-block;
  border-radius: 4px;
  padding: 10px 15px;
  color: red;
  text-align: center;
  margin-top: 15px;
}

.btn.active {
  color: white;
  background-color: red;
  box-shadow: 0 2px 4px rgba(0, 0, 0, .5);
}

.btn:hover {
  color: white;
  background-color: red;
  box-shadow: 0 2px 4px rgba(0, 0, 0, .5);
}

/* Header */

.header {
  display: flex;
  padding: 40px;
}

.header h1 {
  flex-grow: 1;
  font-size: 36px;
}

.header ul {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.header li {
  display: inline;
  margin-left: 10px;
}

.header li:first-child {
  margin-left: 0;
}

.header .btn {
  width: 100px;
  border: 1px solid red;
}

/* Jumbotron */

.jumbotron {
  display: flex;
  flex-direction: column;
  height: 445px;
  padding: 25px 60px 30px 30px;
  background: url("https://s3.amazonaws.com/codecademy-content/projects/bestbite/bg.jpg") no-repeat center center;
  background-size: cover;
  text-align: right;
}

.jumbotron :first-child {
  margin-top: 120px;
  color: red;
}

.jumbotron h2 {
  color: white;
  font-size: 60px;
  line-height: 1.1;
}

.jumbotron :last-child {
  color: orange;
}

/* Banner */

.banner {
  height: 140px;
  padding: 40px 15px 0 15px;
  background-color: #36343f;
  text-align: center;
}

.banner h3 {
  padding-bottom: 24px;
  font-size: 30px;
  color: white;
}

.banner .btn {

  border-radius: 6px;
  border: 2px solid orange;
  font-size: 18px;
  line-height: 1.33;
  color: orange;
}

.banner .btn:hover {
    background-color: orange;
    color: white;
}

.banner .btn:visited {
  color: darkblue;
}

/* Contributions */

.contributions,
.learn {
  text-align: center;
  padding-top: 80px;
}

.contributions h3,
.learn h3 {
  margin-bottom: 9px;
  border-bottom: 1px solid #eee;
  padding-bottom: 20px;
  font-size: 30px;
}

.contributions h4,
.learn h4 {
  color: red;
  margin: 30px 0 20px;
  font-size: 20px;
}

.meals,
.features {
  display: flex;
  justify-content: center;
  padding-top: 20px;
}

.meal,
.feature {
  padding: 0 60px;
}

.meal ul,
.feature ul {
  line-height: 1.4;
}

.breakfast ul li:nth-child(2n+3) {
  color: goldenrod;
  font-weight: bold;
}

.dinner ul li:nth-child(4n+1) {
  color: green;
  font-weight: bold;
}

.dessert ul li:nth-child(3n+0) {
  color: orange;
  font-weight: bold;
}

/* Footer */

footer {
  display: flex;
  justify-content: space-between;
  padding: 40px 15px;
  margin-top: 80px;
  background-color: #eee;
  font-size: 14px;
}

footer a {
  color: red;
}

footer .left {
  flex-grow: 1;
}

footer .right {
  flex-grow: 1;
  text-align: right;
}

footer .left p,
footer .right p {
  min-width: 130px;
}

/* Media Queries */

@media (max-width: 992px) {
  .meals, .features {
    flex-direction: column;
  }
}

@media (max-width: 700px) {
  .header {
    flex-direction: column;
    align-items: center;
    padding-left: 10px;
    padding-right: 10px;
  }

  .header h1 {
    margin-bottom: 20px;
  }

  .header .btn {
    font-size: 14px;
    width: 75px;
  }

  .banner {
    height: 180px;
  }
}
