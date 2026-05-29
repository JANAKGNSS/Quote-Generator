<html>
<html lang="en">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Professional Quotation Generator</title>

<style>

body{
    margin:0;
    padding:20px;
    background:#e5e5e5;
    font-family:Arial, Helvetica, sans-serif;
}

/* FORM SECTION */

.form-box{
    width:95%;
    max-width:1200px;
    margin:auto;
    background:white;
    padding:25px;
    border-radius:10px;
    box-shadow:0 0 15px rgba(0,0,0,0.1);
    margin-bottom:30px;
}

.form-box h2{
    color:#7b1113;
    margin-bottom:20px;
}

.form-box h3{
    margin-top:30px;
    color:#444;
}

input, select{
    width:100%;
    padding:10px;
    border:1px solid #ccc;
    border-radius:5px;
    box-sizing:border-box;
    margin-bottom:10px;
}

button{
    padding:12px 20px;
    border:none;
    border-radius:5px;
    cursor:pointer;
    color:white;
    font-size:15px;
}

.btn-primary{
    background:#7b1113;
}

.btn-secondary{
    background:#555;
}

.btn-danger{
    background:#c00000;
    padding:8px 12px;
}

/* TABLE */

table{
    width:100%;
    border-collapse:collapse;
    margin-top:15px;
}

table th{
    background:#7b1113;
    color:white;
    padding:12px;
    border:1px solid #ccc;
    font-size:14px;
}

table td{
    border:1px solid #ccc;
    padding:10px;
    text-align:center;
    vertical-align:middle;
}

table img{
    width:70px;
    height:70px;
    object-fit:cover;
    border-radius:6px;
    border:1px solid #ccc;
}

/* QUOTATION PAGE */

.page{
    width:95%;
    max-width:1200px;
    margin:auto;
    background:white;
    padding:40px;
    position:relative;
    box-shadow:0 0 15px rgba(0,0,0,0.15);
}

.watermark{
    position:absolute;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    font-size:120px;
    color:red;
    opacity:0.04;
    font-weight:bold;
}

.header{
    display:flex;
    justify-content:space-between;
    border-bottom:3px solid #7b1113;
    padding-bottom:20px;
}

.company-name{
    font-size:42px;
    color:#7b1113;
    font-weight:bold;
}

.company-title{
    color:#c00000;
    font-size:24px;
    margin-top:8px;
    font-weight:bold;
}

.quote-title{
    font-size:40px;
    color:#7b1113;
    font-weight:bold;
}

.quote-info{
    line-height:2;
    margin-top:20px;
}

.client{
    margin-top:30px;
    line-height:1.8;
}

.content{
    margin-top:25px;
    line-height:1.8;
}

/* TOTAL BOX */

.total-box{
    width:350px;
    margin-left:auto;
    margin-top:25px;
}

.total-box td{
    padding:12px;
}

.grand-total{
    background:#410c0d;
    color:white;
    font-weight:bold;
}

/* FOOTER */

.footer{
    margin-top:50px;
    line-height:2;
}

.signature{
    margin-top:50px;
    font-weight:bold;
}

@media print{

    .form-box{
        display:none;
    }

    body{
        background:white;
        padding:0;
    }

    .page{
        box-shadow:none;
        width:100%;
    }
}

</style>
</head>

<body>

<!-- FORM -->

<div class="form-box">

<h2>Quotation Details</h2>

<input type="text" id="customerName" placeholder="Customer Name">

<input type="text" id="customerCity" placeholder="Customer City">

<input type="text" id="quotationNo" placeholder="Quotation Number">

<input type="text" id="gstNo" placeholder="GST Number">

<input type="date" id="quotationDate">

<input type="text" id="senderName" placeholder="Sender Name">

<input type="text" id="senderMobile" placeholder="Sender Mobile Number">

<h3>Items Table</h3>

<table id="itemTable">

<thead>

<tr>
    <th>Category</th>
    <th>Product Description</th>
    <th>Image</th>
    <th>Qty</th>
    <th>Price</th>
    <th>GST %</th>
    <th>Action</th>
</tr>

</thead>

<tbody id="itemTableBody">

<tr class="itemRow">

<td>
    <select class="itemCategory">
        <option>Sales</option>
        <option>Service</option>
    </select>
</td>

<td>
    <input type="text" class="productName" placeholder="Product Name">
</td>

<td>
    <input type="file" class="productImage" accept="image/*">
</td>

<td>
    <input type="number" class="qty" min="1">
</td>

<td>
    <input type="number" class="price">
</td>

<td>
    <input type="number" class="gst">
</td>

<td>
    <button class="btn-danger" onclick="removeRow(this)">
        Delete
    </button>
</td>

</tr>

</tbody>

</table>

<br>

<button class="btn-secondary" onclick="addRow()">
+ Add Row
</button>

<button class="btn-primary" onclick="generateQuotation()">
Generate Quotation
</button>

<button class="btn-primary" onclick="window.print()">
Print
</button>

</div>

<!-- QUOTATION PAGE -->

<div class="page">

<div class="watermark">JANAK</div>

<div class="header">

<div>

<div class="company-name">JANAK</div>

<div class="company-title">
Janak Positioning & Surveying Systems Pvt. Ltd.
</div>

<div style="margin-top:15px; line-height:1.8;">
GSTIN: 07AABCJ0148A1Z9,304 B, Pal Mohan Plaza,<br>
Karol Bagh, New Delhi - 110005<br>
Phone: +91 11 23515400
</div>

</div>

<div>

<div class="quote-title">
QUOTATION
</div>

<div class="quote-info">

<b>Quotation No:</b>
<span id="showQuotationNo"></span>

<br>

<b>GST No:</b>
<span id="showGSTNo"></span>

<br>

<b>Date:</b>
<span id="showDate"></span>

</div>

</div>

</div>

<div class="client">

To,<br><br>

<b id="showCustomer"></b><br>

<span id="showCity"></span>

</div>

<div class="content">

Dear Sir/Madam,<br><br>

Thank you for your valuable enquiry of Surveying instrument. We are pleased to submit our quotation as below:

</div>

<!-- OUTPUT TABLE -->

<table>

<thead>

<tr>
    <th>Sr</th>
    <th>Category</th>
    <th>Product</th>
    <th>Image</th>
    <th>Qty</th>
    <th>Price</th>
    <th>GST</th>
    <th>Total</th>
</tr>

</thead>

<tbody id="outputTableBody"></tbody>

</table>

<!-- TOTAL -->

<table class="total-box">

<tr>
    <td>Subtotal</td>
    <td id="showSubtotal">₹0.00</td>
</tr>

<tr>
    <td>GST Amount</td>
    <td id="showGSTAmount">₹0.00</td>
</tr>

<tr class="grand-total">
    <td>Grand Total</td>
    <td id="showGrandTotal">₹0.00</td>
</tr>

</table>

<!-- FOOTER -->

<div class="footer">

We hope our quotation meets your requirements and
look forward to your valuable order.

Please feel free to contact us for any clarification.

<div class="signature">

Best Regards,<br><br>

For Janak Positioning & Surveying Systems Pvt. Ltd.<br><br>

<b id="showSenderName"></b><br>
<span id="showSenderMobile"></span>

</div>

</div>

</div>

<script>

function addRow(){

    let tbody = document.getElementById("itemTableBody");

    let tr = document.createElement("tr");

    tr.className = "itemRow";

    tr.innerHTML = `

    <td>
        <select class="itemCategory">
            <option>Sales</option>
            <option>Service</option>
        </select>
    </td>

    <td>
        <input type="text" class="productName">
    </td>

    <td>
        <input type="file" class="productImage" accept="image/*">
    </td>

    <td>
        <input type="number" class="qty">
    </td>

    <td>
        <input type="number" class="price">
    </td>

    <td>
        <input type="number" class="gst">
    </td>

    <td>
        <button class="btn-danger" onclick="removeRow(this)">
            Delete
        </button>
    </td>
    `;

    tbody.appendChild(tr);
}

function removeRow(button){

    let row = button.parentElement.parentElement;

    let tbody = document.getElementById("itemTableBody");

    if(tbody.rows.length > 1){
        row.remove();
    }
}

function generateQuotation(){

    document.getElementById("showCustomer").innerHTML =
    document.getElementById("customerName").value;

    document.getElementById("showCity").innerHTML =
    document.getElementById("customerCity").value;

    document.getElementById("showQuotationNo").innerHTML =
    document.getElementById("quotationNo").value;

    document.getElementById("showGSTNo").innerHTML =
    document.getElementById("gstNo").value;

    document.getElementById("showDate").innerHTML =
    document.getElementById("quotationDate").value;

    document.getElementById("showSenderName").innerHTML =
    document.getElementById("senderName").value;

    document.getElementById("showSenderMobile").innerHTML =
    document.getElementById("senderMobile").value ? "Mobile: " + document.getElementById("senderMobile").value : "";

    let rows = document.getElementsByClassName("itemRow");

    let output = "";

    let subtotal = 0;
    let gstTotal = 0;
    let grandTotal = 0;

    for(let i=0; i<rows.length; i++){

        let row = rows[i];

        let category = row.querySelector(".itemCategory").value;

        let product = row.querySelector(".productName").value;

        let qty = Number(row.querySelector(".qty").value) || 0;

        let price = Number(row.querySelector(".price").value) || 0;

        let gst = Number(row.querySelector(".gst").value) || 0;

        let imageInput = row.querySelector(".productImage");

        let imageURL = "";

        if(imageInput.files.length > 0){
            imageURL = URL.createObjectURL(imageInput.files[0]);
        }

        let itemSubtotal = qty * price;

        let gstAmount = (itemSubtotal * gst) / 100;

        let itemTotal = itemSubtotal + gstAmount;

        subtotal += itemSubtotal;
        gstTotal += gstAmount;
        grandTotal += itemTotal;

        output += `

        <tr>

        <td>${i+1}</td>

        <td>${category}</td>

        <td style="text-align:left;">
            ${product}
        </td>

        <td>
            ${
                imageURL
                ? `<img src="${imageURL}">`
                : `No Image`
            }
        </td>

        <td>${qty}</td>

        <td>₹${price.toFixed(2)}</td>

        <td>${gst}%</td>

        <td>₹${itemTotal.toFixed(2)}</td>

        </tr>
        `;
    }

    document.getElementById("outputTableBody").innerHTML = output;

    document.getElementById("showSubtotal").innerHTML =
    "₹" + subtotal.toFixed(2);

    document.getElementById("showGSTAmount").innerHTML =
    "₹" + gstTotal.toFixed(2);

    document.getElementById("showGrandTotal").innerHTML =
    "₹" + grandTotal.toFixed(2);
}

</script>

</body>
</html>
