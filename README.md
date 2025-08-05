# web-application
<!DOCTYPE html>
<html>
<head>
    <title>Online Ticket Booking</title>
    <link rel="stylesheet"href="body.css">
  <style>
    body {

      font-family: Arial, sans-serif;
      background: #f0f2f5;
      padding: 40px;
    }
    h2 {
      color: #333;
    }
    form {
      background: white;
      padding: 20px;
      border-radius: 8px;
      width: 300px;
    }
    label {
      display: block;
      margin-bottom: 10px;
    }
    input, select, button {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      margin-bottom: 15px;
    }
    button {
      background-color: #28a745;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #218838;
    }
  </style>

</head>
<body>

  <h2>Online Ticket Booking</h2>

  <form action="/book" method="POST">
    <label>
      Full Name:
      <input type="text" name="name" required>
    </label>

    <label>
      Email:
      <input type="email" name="email" required>
    </label>

    <label>
      Journey Date:
      <input type="date" name="date" required>
    </label>
<label>
   From:
   <select From="From"required>
      <option value="">Select</option>
      <option value="kakinada">kakinada</option>
      <option value="vijayanagaram">vijayanagaram</option>
      <option value="rajahmundry">rajahmundry</option>
      <option value="srikakulam">srikakulam</option>
   </select>
</label>
 
    <label>
      Destination:
      <select name="destination" required>
        <option value="">Select</option>
        <option value="vizag">vizag</option>
        <option value="Dwarapudi">Dwarapudi</option>
        <option value="vijayawada">vijayawada</option>
        <option value="anakapally">ankapally</option>
      </select>
    </label>

    <label>
      Number of Tickets:
      <input type="number" name="tickets" min="1" max="10" required>
    </label>

    <button type="submit">Book Ticket</button>
  </form>

</body>
</html>
