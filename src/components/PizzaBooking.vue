<template>
<div class="row">
  <div id="home" class="col-sm-12 text-center">
    <div class="background">
      <h1>Welcome to Tutto Bello</h1>
      <h2>Pizza Order</h2>
      
      <div class="col-sm-12 col-md-8" style="background-color: #ffffff">
		<table class="table" style="width: 100%;">
			<thead class="thead-default">
				<tr>
					<th align="left">Pizza</th>
					<th align="left">Price</th>
					<th align="left">Quantity</th>
				</tr>
			</thead>
			<tbody v-for="pizza in menuItems" :key="pizza.name">
				<tr>
					<td ><b>{{pizza.name}}</b></td>
				</tr>
				<tr v-for="opt in pizza.opts" :key="opt.size">
					<td>{{opt.size}}</td>
					<td>{{opt.price}}</td>
					<td><QuantityButton></QuantityButton></td>
				</tr>
			</tbody>
		</table>
  </div>
    </div>

  </div>
</div>
</template>

<script>
import Components from "creative-library";
export default {
    name: 'PizzaBooking',
    data () {
        return {
            menuItems: [{name: 'DIAVOLA', opts: [{size: 'Large', price: '149 kr'}, {size: 'Regular', price: '119 kr'}]},
            {name: 'MARGHERITA', opts: [{size: 'Large', price: '140 kr'}, {size: 'Regular', price: '99 kr'}]},
            {name: 'NAPOLETANA', opts: [{size: 'Large', price: '149 kr'}, {size: 'Regular', price: '115 kr'}]}]
        }
    }
}
</script>

<style src='creative-library/dist/creative.css'></style>
<style>
#home{
  background: url('https://i2.wp.com/www.splendidcomms.com/wp-content/uploads/2018/07/Dominos.jpg');
  height: 105vh;
  padding: 30px;
}
h1,h2{
  margin: 4% auto;
  text-align: center;
}
.background{
  background: rgba(255,255,255,.1);
  padding: 10px 0;
}
</style>