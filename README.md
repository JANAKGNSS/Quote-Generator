<html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@800&family=Caveat:wght@700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary-color: #7b1113;
            --primary-dark: #410c0d;
            --accent-color: #c00000;
            --text-main: #333333;
            --text-muted: #555555;
            --border-color: #cccccc;
            --bg-light: #f8f9fa;
        }

        body {
            margin: 0;
            padding: 40px 20px;
            background: #e9ecef;
            font-family: 'Inter', Arial, sans-serif;
            color: var(--text-main);
        }

        /* FORM SECTION UI */
        .form-box {
            width: 100%;
            max-width: 1100px;
            margin: 0 auto 40px auto;
            background: #ffffff;
            padding: 35px;
            border-radius: 8px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            box-sizing: border-box;
        }

        .form-box h2 {
            color: var(--primary-color);
            margin-top: 0;
            margin-bottom: 25px;
            font-size: 24px;
            border-bottom: 2px solid var(--bg-light);
            padding-bottom: 10px;
        }

        .form-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 15px;
            margin-bottom: 25px;
        }

        .form-box h3 {
            margin-top: 35px;
            margin-bottom: 15px;
            color: var(--text-main);
            font-size: 18px;
        }

        input, select {
            width: 100%;
            padding: 10px 12px;
            border: 1px solid var(--border-color);
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
            transition: border-color 0.2s;
        }

        input:focus, select:focus {
            outline: none;
            border-color: var(--primary-color);
        }

        .button-group {
            margin-top: 25px;
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        button {
            padding: 12px 24px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            transition: opacity 0.2s;
        }

        button:hover {
            opacity: 0.9;
        }

        .btn-primary { background: var(--primary-color); color: #ffffff; }
        .btn-secondary { background: var(--text-muted); color: #ffffff; }
        .btn-danger { background: var(--accent-color); color: #ffffff; padding: 8px 14px; font-size: 13px; }

        /* INPUT TABLE SPECIFIC */
        #itemTable {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        #itemTable th {
            background: var(--text-muted);
            color: #ffffff;
            padding: 10px;
            font-size: 13px;
            text-align: left;
        }
        #itemTable td {
            padding: 8px;
            border-bottom: 1px solid #eee;
        }

        /* QUOTATION OUTPUT PAGE PRESENTATION */
        .page {
            width: 100%;
            max-width: 1100px;
            margin: 0 auto;
            background: #ffffff;
            padding: 50px;
            position: relative;
            box-shadow: 0 4px 25px rgba(0,0,0,0.1);
            box-sizing: border-box;
            min-height: 297mm; /* Proportional Layout Bounds */
        }

        .watermark {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) rotate(-45deg);
            font-size: 130px;
            color: #000000;
            opacity: 0.03;
            font-weight: 900;
            pointer-events: none;
            letter-spacing: 10px;
        }

        /* LOGO & BRANDING INTERNAL SUB-LAYOUT */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            border-bottom: 3px solid var(--primary-color);
            padding-bottom: 25px;
            margin-bottom: 30px;
        }

        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            width: fit-content;
        }

        .logo-top {
            display: flex;
            align-items: flex-end;
            gap: 16px;
        }

        /* Image-based Logo adjustments */
        .brand-logo-img {
            max-width: 280px;
            height: auto;
            display: block;
        }

        .divider {
            width: 100%;
            height: 5px;
            background: #8B2626;
            margin-top: 8px;
            margin-bottom: 4px;
            clip-path: polygon(0% 40%, 5% 20%, 95% 10%, 100% 50%, 98% 85%, 85% 70%, 15% 90%, 0% 60%);
        }

        .slogan {
            font-family: 'Caveat', cursive;
            font-size: 28px;
            color: #2b2b2b;
            margin-left: 5px;
            letter-spacing: -0.5px;
            margin-top: 2px;
        }

        .slogan span.pride-text {
            color: #8B2626;
            font-weight: 700;
            padding-left: 5px;
        }

        .company-title {
            color: var(--accent-color);
            font-size: 18px;
            margin-top: 15px;
            font-weight: 700;
            letter-spacing: 0.5px;
        }

        .company-details {
            margin-top: 8px;
            line-height: 1.6;
            font-size: 13px;
            color: var(--text-muted);
        }

        /* UPPER RIGHT DETAILS */
        .quote-meta-box {
            text-align: right;
        }

        .quote-title {
            font-size: 36px;
            color: var(--primary-color);
            font-weight: 800;
            letter-spacing: 2px;
            margin-bottom: 15px;
        }

        .quote-info {
            line-height: 1.8;
            font-size: 14px;
            text-align: right;
        }

        /* CLIENT & CONTENT ENTRIES */
        .client {
            margin-top: 20px;
            margin-bottom: 25px;
            line-height: 1.6;
            font-size: 14px;
            background: var(--bg-light);
            padding: 15px;
            border-left: 4px solid var(--primary-color);
            border-radius: 0 4px 4px 0;
        }

        .content {
            margin-bottom: 25px;
            line-height: 1.6;
            font-size: 14px;
        }

        /* FINAL OUTPUT SYSTEM TABLE */
        table.output-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            font-size: 14px;
        }

        table.output-table th {
            background: var(--primary-color);
            color: #ffffff;
            padding: 12px 10px;
            font-weight: 600;
            border: 1px solid #b56c6d;
            font-size: 13px;
            text-transform: uppercase;
        }

        table.output-table td {
            border: 1px solid #e0e0e0;
            padding: 12px 10px;
            text-align: center;
            vertical-align: middle;
        }

        table.output-table img {
            width: 65px;
            height: 65px;
            object-fit: cover;
            border-radius: 4px;
            border: 1px solid #dddddd;
        }

        /* PRICING TOTAL SECTION */
        .total-box {
            width: 350px;
            margin-left: auto;
            margin-top: 30px;
            border-collapse: collapse;
            font-size: 14px;
        }

        .total-box td {
            padding: 10px 15px;
            border: 1px solid #e0e0e0;
        }
        
        .total-box td:first-child {
            font-weight: 500;
            color: var(--text-muted);
            text-align: right;
        }

        .total-box td:last-child {
            text-align: right;
            font-weight: 600;
            width: 130px;
        }

        .grand-total {
            background: var(--primary-dark);
            color: #ffffff !important;
        }

        .grand-total td {
            color: #ffffff !important;
            font-weight: 700 !important;
            font-size: 15px;
            border-color: var(--primary-dark);
        }

        /* CLOSING TERMS & SIGNATURES */
        .footer {
            margin-top: 50px;
            line-height: 1.6;
            font-size: 14px;
            page-break-inside: avoid;
        }

        .signature {
            margin-top: 45px;
            line-height: 1.6;
        }

        /* STRICT DOCUMENT PAGE SETTING INSTRUCTIONS (A4 / LETTER REGULATION) */
        @page {
            size: A4 portrait; /* Dynamically auto-switches or processes to Letter uniformly depending on client system defaults */
            margin: 15mm 12mm 15mm 12mm;
        }

        @media print {
            .form-box {
                display: none !important;
            }
            body {
                background: #ffffff !important;
                padding: 0 !important;
                margin: 0 !important;
            }
            .page {
                box-shadow: none !important;
                width: 100% !important;
                max-width: 100% !important;
                padding: 0 !important;
                min-height: auto !important;
            }
            table.output-table th {
                background-color: var(--primary-color) !important;
                -webkit-print-color-adjust: exact;
                print-color-adjust: exact;
            }
            .grand-total {
                background-color: var(--primary-dark) !important;
                -webkit-print-color-adjust: exact;
                print-color-adjust: exact;
            }
        }
    </style>
</head>
<body>

<div class="form-box">
    <h2>Quotation From</h2>
    
    <div class="form-grid">
        <input type="text" id="customerName" placeholder="Customer Name">
        <input type="text" id="customerCity" placeholder="Customer City">
        <input type="text" id="quotationNo" placeholder="Quotation Number">
        <input type="text" id="gstNo" placeholder="GST Number">
        <input type="date" id="quotationDate">
        <input type="text" id="senderName" placeholder="Sender Name">
        <input type="text" id="senderMobile" placeholder="Sender Mobile Number">
    </div>

    <div class="form-grid" style="grid-template-columns: 1fr 1fr; max-width: 500px; margin-bottom: 20px;">
        <div>
            <label style="font-size: 13px; font-weight: 600; display: block; margin-bottom: 5px;">Document Layout Setting</label>
            <select id="pageSizeSetting" onchange="applyPageLayout()">
                <option value="A4">A4 Standard (210mm × 297mm)</option>
                <option value="Letter">US Letter Standard (8.5" × 11")</option>
            </select>
        </div>
    </div>

    <h3>Line Items Management</h3>
    <table id="itemTable">
        <thead>
            <tr>
                <th style="width: 12%;">Category</th>
                <th style="width: 35%;">Product Description</th>
                <th style="width: 20%;">Image Asset</th>
                <th style="width: 8%;">Qty</th>
                <th style="width: 12%;">Base Price</th>
                <th style="width: 8%;">GST %</th>
                <th style="width: 5%;">Action</th>
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
                    <input type="text" class="productName" placeholder="e.g. Total Station Model X">
                </td>
                <td>
                    <input type="file" class="productImage" accept="image/*">
                </td>
                <td>
                    <input type="number" class="qty" min="1" value="1">
                </td>
                <td>
                    <input type="number" class="price" placeholder="0.00">
                </td>
                <td>
                    <input type="number" class="gst" placeholder="18" value="18">
                </td>
                <td>
                    <button class="btn-danger" onclick="removeRow(this)">Delete</button>
                </td>
            </tr>
        </tbody>
    </table>

    <div class="button-group">
        <button class="btn-secondary" onclick="addRow()">+ Add More Item</button>
        <button class="btn-primary" onclick="generateQuotation()">Get Quotation</button>
        <button class="btn-primary" style="background-color: #1e4620;" onclick="downloadPDF()">Download/Print</button>
    </div>
</div>

<div id="quotationPageElement" class="page">
    <div class="watermark">JANAK</div>

    <div class="header">
        <div class="logo-container">
            <div class="logo-top">
                <img src="https://janaksurvey.com/images/front-logo-janak.png" alt="Janak Survey Logo" class="brand-logo-img">
            </div>
         <div class="company-title">Janak Positioning & Surveying Systems Pvt. Ltd.</div>
            <div class="company-details">
                GSTIN: 07AABCJ0148A1Z9<br>
                304 B, Pal Mohan Plaza, Karol Bagh, New Delhi - 110005<br>
                Phone: +91 11 23515400
            </div>
        </div>

        <div class="quote-meta-box">
            <div class="quote-title">QUOTATION</div>
            <div class="quote-info">
                <b>Quotation No:</b> <span id="showQuotationNo">—</span><br>
                <b>GST No:</b> <span id="showGSTNo">—</span><br>
                <b>Date:</b> <span id="showDate">—</span>
            </div>
        </div>
    </div>

    <div class="client">
        <strong>To,</strong><br>
        <span id="showCustomer" style="font-weight: 600; font-size: 15px;">[Customer Name]</span><br>
        <span id="showCity">[Customer City]</span>
    </div>

    <div class="content">
        Dear Sir/Madam,<br><br>
        Thank you for your valuable enquiry of Surveying instrument. We are pleased to submit our quotation as below:
    </div>

    <table class="output-table">
        <thead>
            <tr>
                <th style="width: 5%;">Sr.</th>
                <th style="width: 12%;">Category</th>
                <th style="width: 38%;">Product Description</th>
                <th style="width: 15%;">Image</th>
                <th style="width: 6%;">Qty</th>
                <th style="width: 12%;">Price</th>
                <th style="width: 7%;">GST</th>
                <th style="width: 15%;">Total</th>
            </tr>
        </thead>
        <tbody id="outputTableBody">
            <tr>
                <td colspan="8" style="color: #999; padding: 20px;">No items compiled. Fill in details above and click 'Compile Quotation'.</td>
            </tr>
        </tbody>
    </table>

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

    <div class="footer">
        We hope our quotation meets your requirements and look forward to your valuable order.<br>
        Please feel free to contact us for any clarification.

        <div class="signature">
            Best Regards,<br><br>
            <strong>For Janak Positioning & Surveying Systems Pvt. Ltd.</strong><br><br><br>
            <span id="showSenderName" style="font-weight: 600; text-decoration: underline;">[Authorized Signatory]</span><br>
            <span id="showSenderMobile"></span>
        </div>
    </div>
</div>

<script>
function applyPageLayout() {
    let sizeSelected = document.getElementById("pageSizeSetting").value;
    let styleTag = document.getElementById("dynamicPageSizeRule");
    
    if(!styleTag) {
        styleTag = document.createElement("style");
        styleTag.id = "dynamicPageSizeRule";
        document.head.appendChild(styleTag);
    }
    
    if(sizeSelected === "Letter") {
        styleTag.innerHTML = `@page { size: letter portrait; margin: 15mm 12mm; }`;
    } else {
        styleTag.innerHTML = `@page { size: A4 portrait; margin: 15mm 12mm; }`;
    }
}

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
        <input type="text" class="productName" placeholder="Product Name">
    </td>
    <td>
        <input type="file" class="productImage" accept="image/*">
    </td>
    <td>
        <input type="number" class="qty" min="1" value="1">
    </td>
    <td>
        <input type="number" class="price" placeholder="0.00">
    </td>
    <td>
        <input type="number" class="gst" placeholder="18" value="18">
    </td>
    <td>
        <button class="btn-danger" onclick="removeRow(this)">Delete</button>
    </td>`;
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
    document.getElementById("showCustomer").innerHTML = document.getElementById("customerName").value || "[Customer Name]";
    document.getElementById("showCity").innerHTML = document.getElementById("customerCity").value || "[Customer City]";
    document.getElementById("showQuotationNo").innerHTML = document.getElementById("quotationNo").value || "—";
    document.getElementById("showGSTNo").innerHTML = document.getElementById("gstNo").value || "—";
    
    let rawDate = document.getElementById("quotationDate").value;
    if(rawDate) {
        let dateObj = new Date(rawDate);
        document.getElementById("showDate").innerHTML = dateObj.toLocaleDateString('en-IN', {day: '2-digit', month: '2-digit', year: 'numeric'});
    } else {
        document.getElementById("showDate").innerHTML = "—";
    }

    document.getElementById("showSenderName").innerHTML = document.getElementById("senderName").value || "[Authorized Signatory]";
    document.getElementById("showSenderMobile").innerHTML = document.getElementById("senderMobile").value ? "Mobile: " + document.getElementById("senderMobile").value : "";

    let rows = document.getElementsByClassName("itemRow");
    let output = "";
    let subtotal = 0;
    let gstTotal = 0;
    let grandTotal = 0;
    let loadedImagesCount = 0;

    function renderTableHTML() {
        document.getElementById("outputTableBody").innerHTML = output;
        document.getElementById("showSubtotal").innerHTML = "₹" + subtotal.toLocaleString('en-IN', {minimumFractionDigits: 2, maximumFractionDigits: 2});
        document.getElementById("showGSTAmount").innerHTML = "₹" + gstTotal.toLocaleString('en-IN', {minimumFractionDigits: 2, maximumFractionDigits: 2});
        document.getElementById("showGrandTotal").innerHTML = "₹" + grandTotal.toLocaleString('en-IN', {minimumFractionDigits: 2, maximumFractionDigits: 2});
    }

    if(rows.length === 0 || (rows.length === 1 && rows[0].querySelector(".productName").value === "")) {
        document.getElementById("outputTableBody").innerHTML = `<tr><td colspan="8" style="color: #999; padding: 20px;">No items configured.</td></tr>`;
        return;
    }

    let rowDataArray = [];

    for(let i=0; i<rows.length; i++){
        let row = rows[i];
        let category = row.querySelector(".itemCategory").value;
        let product = row.querySelector(".productName").value || "Unspecified Product";
        let qty = Number(row.querySelector(".qty").value) || 0;
        let price = Number(row.querySelector(".price").value) || 0;
        let gst = Number(row.querySelector(".gst").value) || 0;
        let imageInput = row.querySelector(".productImage");

        let itemSubtotal = qty * price;
        let gstAmount = (itemSubtotal * gst) / 100;
        let itemTotal = itemSubtotal + gstAmount;

        subtotal += itemSubtotal;
        gstTotal += gstAmount;
        grandTotal += itemTotal;

        rowDataArray.push({
            sr: i + 1,
            category: category,
            product: product,
            qty: qty,
            price: price,
            gst: gst,
            itemTotal: itemTotal,
            fileInput: imageInput,
            imageURL: ""
        });
    }

    let checkAndRender = () => {
        loadedImagesCount++;
        if(loadedImagesCount === rowDataArray.length) {
            rowDataArray.forEach(item => {
                output += `
                <tr>
                    <td>${item.sr}</td>
                    <td>${item.category}</td>
                    <td style="text-align: left; font-weight: 500;">${item.product}</td>
                    <td>${item.imageURL ? `<img src="${item.imageURL}">` : `<span style="color:#999; font-size:12px;">No Image</span>`}</td>
                    <td>${item.qty}</td>
                    <td>₹${item.price.toLocaleString('en-IN', {minimumFractionDigits: 2, maximumFractionDigits: 2})}</td>
                    <td>${item.gst}%</td>
                    <td style="font-weight:600;">₹${item.itemTotal.toLocaleString('en-IN', {minimumFractionDigits: 2, maximumFractionDigits: 2})}</td>
                </tr>`;
            });
            renderTableHTML();
        }
    };

    rowDataArray.forEach((item) => {
        if(item.fileInput && item.fileInput.files.length > 0) {
            let reader = new FileReader();
            reader.onload = function(e) {
                item.imageURL = e.target.result;
                checkAndRender();
            };
            reader.readAsDataURL(item.fileInput.files[0]);
        } else {
            item.imageURL = "";
            checkAndRender();
        }
    });
}

function downloadPDF() {
    // Generate latest data state before processing download
    generateQuotation();
    applyPageLayout();
    
    // Calls standard client system print loop mapped into native PDF download vectors cleanly
    window.print();
}
</script>
</body>
</html>
