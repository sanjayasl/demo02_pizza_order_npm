<template>
  <div class="main">
    <div class="top_container">
      <h2 class="title1">{{title}}</h2>
    </div>
    <div class="content">
      <div class="holder">
        <div class="left_content">
            <div style="float: left;">
                <img src="http://how2reach2every1.org/wp-content/uploads/2018/01/Logo_TV_2015.png">
            </div><br>
            <div style="float: left;">
              <ul>
              <ui>Home</ui>
              <ui>Book Tickets</ui>
              <ui>What's On</ui>
              <ui>About Us</ui>
              <ui>Get Involed</ui>
              <ui>Faq's</ui>
              <ui>Contact</ui>
              </ul>
            </div>
        </div>
        <div class="right_content">
          <table>
            <tr>
              <th>Company</th>
              <th>Contact</th>
              <th>Country</th>
            </tr>
            <tr>
              <td>Alfreds Futterkiste</td>
              <td>Maria Anders</td>
              <td>Germany</td>
            </tr>
            <tr>
              <td>Centro comercial Moctezuma</td>
              <td>Francisco Chang</td>
              <td>Mexico</td>
            </tr>
            <tr>
              <td>Ernst Handel</td>
              <td>Roland Mendel</td>
              <td>Austria</td>
            </tr>
            <tr>
              <td>Island Trading</td>
              <td>Helen Bennett</td>
              <td>UK</td>
            </tr>
            <tr>
              <td>Laughing Bacchus Winecellars</td>
              <td>Yoshi Tannamuri</td>
              <td>Canada</td>
            </tr>
            <tr>
              <td>Magazzini Alimentari Riuniti</td>
              <td>Giovanni Rovelli</td>
              <td>Italy</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'TicketBooking',
    data () {
        return {
          title: 'Book Tickets'
        }  
    }
}
</script>

<style>
.main {
  background-image: url('https://b.kisscc0.com/20180817/evq/kisscc0-dock-sunset-pier-shore-sunrise-spring-jetty-5b76eadfc119f0.484676841534520031791.png');
  background-repeat: no-repeat;
  background-position: center; 
  position: relative;
}
.top_container {
  margin: 0;
}
.title1 {
  /* margin-top: 60px;
  margin-bottom: 50px; */
  font-size: 45px;
  text-align: left;
  margin: auto;
  padding-top: 60px;
  padding-left: 15px;
  position: relative;
}
.content {
  display: inline;
  margin: auto;
  position: relative;
  padding-top: 100px;
  background-color: blue;
}
.holder {
  width: 480px;
  height: 560px;
  margin: auto;
  position: relative;
}
.left_content {
  position: absolute;
  top: 50%;
  left: 0;
  padding-left: 10px;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  background-color: blue;
}
.right_content {
  position: absolute;
  top: 50%;
  right: 0;
  padding-right: 10px;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  background-color: gold;
}
table {
    font-family: arial, sans-serif;
    border-collapse: collapse;
    width: 100%;
}

td, th {
    border: 1px solid #dddddd;
    text-align: left;
    padding: 8px;
}
</style>