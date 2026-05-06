<!DOCTYPE html>
<html>
<head>
    <title>Pizza Delivery App</title>
    <style>
        body {
            font-family: Arial;
            background: #222;
            color: white;
            text-align: center;
        }

        .box {
            background: #333;
            padding: 20px;
            margin: 50px auto;
            width: 300px;
            border-radius: 10px;
        }

        select, button {
            width: 90%;
            padding: 10px;
            margin: 10px;
        }

        button {
            background: green;
            color: white;
            border: none;
        }
    </style>
</head>

<body>

<div class="box">
    <h2>🍕 Pizza Order</h2>

    <label>Choose Size:</label>
    <select id="size">
        <option>Small</option>
        <option>Medium</option>
        <option>Large</option>
    </select>

    <label>Choose Crust:</label>
    <select id="crust">
        <option>Thin</option>
        <option>Cheese Burst</option>
        <option>Pan</option>
    </select>

    <label>Choose Toppings:</label>
    <select id="topping">
        <option>Veggies</option>
        <option>Paneer</option>
        <option>Chicken</option>
    </select>

    <button onclick="orderPizza()">Place Order</button>

    <p id="output"></p>
</div>

<script>
function orderPizza() {
    let size = document.getElementById("size").value;
    let crust = document.getElementById("crust").value;
    let topping = document.getElementById("topping").value;

    document.getElementById("output").innerHTML =
        "Order Placed ✅<br>" +
        "Size: " + size + "<br>" +
        "Crust: " + crust + "<br>" +
        "Topping: " + topping + "<br>" +
        "Status: Preparing 🍕";
}
</script>

</body>
</html>
