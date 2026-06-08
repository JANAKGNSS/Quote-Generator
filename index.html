<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Quotation Portal</title>
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
            --success-color: #1e4620;
        }

        body {
            margin: 0;
            padding: 0;
            background: #e9ecef;
            font-family: 'Inter', Arial, sans-serif;
            color: var(--text-main);
        }

        /* UTILITIES */
        .hidden { display: none !important; }
        
        /* AUTH & HOME PAGE PORTAL */
        .portal-container {
            max-width: 500px;
            margin: 80px auto;
            background: #ffffff;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 4px 25px rgba(0,0,0,0.1);
            text-align: center;
        }
        .portal-logo {
            max-width: 220px;
            margin-bottom: 20px;
        }
        .role-btn-group {
            display: flex;
            gap: 15px;
            margin-top: 30px;
        }
        .role-btn {
            flex: 1;
            padding: 15px;
            font-size: 16px;
            font-weight: 600;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.2s;
        }
        .btn-admin-choice { background: var(--primary-dark); color: white; border: none; }
        .btn-staff-choice { background: var(--primary-color); color: white; border: none; }
        
        .login-box {
            margin-top: 25px;
            border-top: 1px solid #eee;
            padding-top: 20px;
        }

        /* DASHBOARD LAYOUT */
        .nav-bar {
            background: var(--primary-dark);
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 10px;
        }
        .nav-brand { font-weight: 700; font-size: 18px; }
        .nav-user { font-size: 14px; display: flex; align-items: center; gap: 15px; }

        .main-layout {
            padding: 30px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        /* APP PANELS */
        .panel {
            background: #ffffff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
            margin-bottom: 30px;
        }
        .panel h2 {
            color: var(--primary-color);
            margin-top: 0;
            margin-bottom: 20px;
            font-size: 22px;
            border-bottom: 2px solid var(--bg-light);
            padding-bottom: 10px;
        }

        /* FORM BOX DESIGN */
        .form-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 15px;
            margin-bottom: 25px;
        }
        label {
            font-size: 13px;
            font-weight: 600;
            display: block;
            margin-bottom: 6px;
            color: var(--text-muted);
        }
        input, select, textarea {
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
        input:disabled, select:disabled {
            background-color: #f1f3f5;
            cursor: not-allowed;
        }

        /* RESPONSIVE TABLE IMPLEMENTATIONS */
        .table-responsive-wrapper {
            width: 100%;
            overflow-x: auto;
            margin-bottom: 20px;
            border: 1px solid #eee;
            border-radius: 4px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th {
            background: var(--text-muted);
            color: #ffffff;
            padding: 12px 10px;
            font-size: 13px;
            text-align: left;
        }
        td {
            padding: 10px;
            border-bottom: 1px solid #eee;
            font-size: 14px;
        }

        /* SYSTEM BUTTONS */
        .button-group {
            margin-top: 25px;
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }
        button {
            padding: 11px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            transition: opacity 0.2s;
        }
        button:hover { opacity: 0.9; }
        .btn-primary { background: var(--primary-color); color: #ffffff; }
        .btn-secondary { background: var(--text-muted); color: #ffffff; }
        .btn-danger { background: var(--accent-color); color: #ffffff; }
        .btn-success { background: var(--success-color); color: #ffffff; }
        .btn-sm { padding: 6px 12px; font-size: 12px; }

        /* DEVICE PREVIEW TOGGLE FRAMING SYSTEM */
        .preview-control-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }
        .preview-frame-container {
            width: 100%;
            transition: all 0.3s ease;
            margin: 0 auto;
        }
        /* Simulated Mobile Device Window Wrap Rules */
        .preview-frame-container.mobile-view {
            max-width: 375px;
            border: 12px solid #222;
            border-radius: 25px;
            padding: 15px 10px !important;
            background: white;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            height: 640px;
            overflow-y: auto;
        }

        /* LIVE OUTPUT QUOTATION COMPONENT VIEW */
        .page {
            width: 100%;
            background: #ffffff;
            padding: 40px;
            position: relative;
            box-shadow: 0 4px 25px rgba(0,0,0,0.05);
            box-sizing: border-box;
            min-height: 297mm;
        }
        .preview-frame-container.mobile-view .page {
            padding: 10px;
            min-height: auto;
            box-shadow: none;
        }
        .watermark {
            position: absolute;
            top: 40%; left: 50%;
            transform: translate(-50%, -50%) rotate(-45deg);
            font-size: 90px;
            color: #000; opacity: 0.02;
            font-weight: 900; pointer-events: none;
        }
        .preview-frame-container.mobile-view .watermark { font-size: 40px; }

        .header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            border-bottom: 3px solid var(--primary-color);
            padding-bottom: 20px;
            margin-bottom: 25px;
        }
        .preview-frame-container.mobile-view .header {
            flex-direction: column;
            gap: 15px;
        }
        .brand-logo-img { max-width: 200px; height: auto; }
        .company-details { margin-top: 8px; line-height: 1.5; font-size: 12px; color: var(--text-muted); }
        .quote-meta-box { text-align: right; }
        .preview-frame-container.mobile-view .quote-meta-box { text-align: left; width: 100%; }
        .quote-title { font-size: 28px; color: var(--primary-color); font-weight: 800; margin-bottom: 10px; }
        .quote-info { line-height: 1.6; font-size: 13px; }

        .client {
            margin-top: 15px; margin-bottom: 20px;
            font-size: 13px; background: var(--bg-light);
            padding: 12px; border-left: 4px solid var(--primary-color);
        }
        table.output-table th {
            background: var(--primary-color); color: white;
            font-size: 11px; text-transform: uppercase; padding: 8px;
        }
        table.output-table td { padding: 8px; text-align: center; font-size: 12px; }
        table.output-table img { width: 45px; height: 45px; object-fit: cover; border-radius: 4px; }

        /* Total calculation block elements */
        .total-box { width: 300px; margin-left: auto; margin-top: 20px; }
        .preview-frame-container.mobile-view .total-box { width: 100%; }
        .total-box td { padding: 8px 12px; font-size: 13px; }
        .grand-total { background: var(--primary-dark); color: white; font-weight: 700; }

        .footer { margin-top: 40px; font-size: 13px; }
        .signature { margin-top: 30px; }

        /* PRINT MEDIA EMULATION DEFINITION */
        @page { size: A4 portrait; margin: 15mm 12mm; }
        @media print {
            .form-box, .nav-bar, .panel, #portalView, .preview-control-header { display: none !important; }
            body { background: #ffffff !important; padding: 0 !important; margin: 0 !important; }
            .main-layout { padding: 0; max-width: 100%; }
            .preview-frame-container.mobile-view { max-width: 100% !important; border: none; padding: 0 !important; height: auto; }
            .page { box-shadow: none !important; padding: 0 !important; width: 100% !important; }
            table.output-table th { background-color: var(--primary-color) !important; -webkit-print-color-adjust: exact; print-color-adjust: exact; }
            .grand-total { background-color: var(--primary-dark) !important; -webkit-print-color-adjust: exact; print-color-adjust: exact; }
        }

        /* SMALL DEVICE SCREEN MEDIA QUERY OVERRIDES */
        @media (max-width: 76EDpx) {
            body { padding: 0; }
            .main-layout { padding: 15px 10px; }
            .panel { padding: 15px; }
            .form-grid { grid-template-columns: 1fr; }
            .header { flex-direction: column; gap: 15px; }
            .quote-meta-box { text-align: left; }
            .total-box { width: 100%; }
            #itemTable th:nth-child(1), #itemTable td:nth-child(1),
            #itemTable th:nth-child(3), #itemTable td:nth-child(3) { display: none; } /* Hide non-critical columns on raw phone forms */
        }
    </style>
</head>
<body>

<div id="portalView" class="portal-container">
    <img src="https://janaksurvey.com/images/front-logo-janak.png" alt="Janak Survey Logo" class="portal-logo">
    <h3>Quotation Management Workspace</h3>
    <p style="color: var(--text-muted); font-size: 14px;">Select your Access Gateway below to get started</p>
    
    <div class="role-btn-group">
        <button class="role-btn btn-admin-choice" onclick="showLoginGate('admin')">Admin Access</button>
        <button class="role-btn btn-staff-choice" onclick="showLoginGate('staff')">Staff Access</button>
    </div>

    <div id="loginFormGate" class="login-box hidden">
        <h4 id="loginGateTitle" style="margin-top:0;">Verify Security Access</h4>
        <div style="margin-bottom:12px; text-align:left;">
            <label>Username PIN</label>
            <input type="text" id="gateUser" placeholder="e.g. admin or staff1">
        </div>
        <div style="margin-bottom:15px; text-align:left;">
            <label>Password</label>
            <input type="password" id="gatePass" value="1245">
        </div>
        <button class="btn-primary" style="width:100%" onclick="processSystemLogin()">Authenticate</button>
    </div>
</div>

<div id="appWorkspace" class="hidden">
    <div class="nav-bar">
        <div class="nav-brand">JANAK SURVEY GATEWAY</div>
        <div class="nav-user">
            <div>Session: <strong id="userBadge" style="text-transform:uppercase;">User</strong> (<span id="roleBadge">Role</span>)</div>
            <button class="btn-danger btn-sm" onclick="logoutWorkspace()">Exit System</button>
        </div>
    </div>

    <div class="main-layout">
        <div id="adminPanelBlock" class="panel hidden">
            <h2>Admin Control Terminal (Staff Directory Profiles)</h2>
            <div class="form-grid">
                <div>
                    <label>Staff ID Name</label>
                    <input type="text" id="newStaffName" placeholder="e.g. Ramesh Kumar">
                </div>
                <div>
                    <label>System Username Tag</label>
                    <input type="text" id="newStaffUser" placeholder="e.g. ramesh12">
                </div>
                <div>
                    <label>Assigned Permission</label>
                    <select id="newStaffRole">
                        <option value="Standard Staff">Standard Staff (Locked Pricing Mode)</option>
                        <option value="Senior Executive">Senior Executive (Full Modifications)</option>
                    </select>
                </div>
                <div style="display:flex; align-items:flex-end;">
                    <button class="btn-success" style="width:100%;" onclick="addNewStaffProfile()">Create New Profile</button>
                </div>
            </div>

            <h4 style="margin-bottom:10px;">Active System Directory Records</h4>
            <div class="table-responsive-wrapper">
                <table>
                    <thead>
                        <tr>
                            <th>Staff Representative Name</th>
                            <th>Username Handle</th>
                            <th>Role Scope</th>
                            <th>Status Control</th>
                            <th>Actions</th>
                        </tr>
                    </thead>
                    <tbody id="directoryTableBody">
                        </tbody>
                </table>
            </div>
        </div>

        <div class="panel form-box">
            <h2>Quotation Builder Setup</h2>
            
            <div class="form-grid">
                <div>
                    <label>Customer Name</label>
                    <input type="text" id="customerName" placeholder="Customer Name">
                </div>
                <div>
                    <label>Customer City</label>
                    <input type="text" id="customerCity" placeholder="Customer City">
                </div>
                <div>
                    <label>Quotation Number</label>
                    <input type="text" id="quotationNo" placeholder="Quotation Number">
                </div>
                <div>
                    <label>GST Number</label>
                    <input type="text" id="gstNo" placeholder="GST Number">
                </div>
                <div>
                    <label>Quotation Date</label>
                    <input type="date" id="quotationDate">
                </div>
                <div>
                    <label>Sender Signatory Name</label>
                    <input type="text" id="senderName" placeholder="Sender Name">
                </div>
                <div>
                    <label>Sender Contact Number</label>
                    <input type="text" id="senderMobile" placeholder="Sender Mobile Number">
                </div>
                <div>
                    <label>Document Layout Engine</label>
                    <select id="pageSizeSetting" onchange="applyPageLayout()">
                        <option value="A4">A4 Standard (210mm × 297mm)</option>
                        <option value="Letter">US Letter Standard (8.5" × 11")</option>
                    </select>
                </div>
            </div>

            <h3>Line Items Configuration Management</h3>
            <div class="table-responsive-wrapper">
                <table id="itemTable">
                    <thead>
                        <tr>
                            <th style="width: 15%;">Category</th>
                            <th style="width: 35%;">Product Description</th>
                            <th style="width: 20%;">Image Asset</th>
                            <th style="width: 8%;">Qty</th>
                            <th style="width: 12%;">Base Price (₹)</th>
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
                                <button class="btn-danger btn-sm" onclick="removeRow(this)">Delete</button>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <div class="button-group">
                <button id="addItemsBtn" class="btn-secondary" onclick="addRow()">+ Add More Item</button>
                <button class="btn-primary" onclick="generateQuotation()">Compile & Sync Preview</button>
                <button class="btn-success" onclick="downloadPDF()">Download / Print System PDF</button>
            </div>
        </div>

        <div class="panel">
            <div class="preview-control-header">
                <h3 style="margin:0; color: var(--text-main);">Live Document Preview Frame</h3>
                <div>
                    <button class="btn-secondary btn-sm" onclick="toggleMobileView(false)">Desktop A4 View</button>
                    <button class="btn-primary btn-sm" style="background:#007bff" onclick="toggleMobileView(true)">Mobile Smartphone View</button>
                </div>
            </div>
            
            <div id="previewWrapper" class="preview-frame-container">
                <div id="quotationPageElement" class="page">
                    <div class="watermark">JANAK</div>

                    <div class="header">
                        <div class="logo-container">
                            <img src="https://janaksurvey.com/images/front-logo-janak.png" alt="Janak Survey Logo" class="brand-logo-img">
                            <div class="company-title" style="font-weight:700; font-size:14px; margin-top:10px; color:var(--accent-color);">Janak Positioning & Surveying Systems Pvt. Ltd.</div>
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
                        <span id="showCustomer" style="font-weight: 600; font-size: 14px;">[Customer Name]</span><br>
                        <span id="showCity">[Customer City]</span>
                    </div>

                    <div style="font-size:13px; margin-bottom:15px;">
                        Dear Sir/Madam,<br>
                        Thank you for your valuable enquiry. We are pleased to submit our quotation parameters as mapped down:
                    </div>

                    <div class="table-responsive-wrapper" style="border:none;">
                        <table class="output-table">
                            <thead>
                                <tr>
                                    <th style="width: 5%;">Sr.</th>
                                    <th style="width: 15%;">Category</th>
                                    <th style="width: 35%;">Product Description</th>
                                    <th style="width: 15%;">Image</th>
                                    <th style="width: 7%;">Qty</th>
                                    <th style="width: 13%;">Price</th>
                                    <th style="width: 10%;">GST</th>
                                    <th style="width: 15%;">Total</th>
                                </tr>
                            </thead>
                            <tbody id="outputTableBody">
                                <tr>
                                    <td colspan="8" style="color: #999; padding: 20px; text-align:center;">No items compiled. Fill in details above and execution tracking will follow.</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>

                    <table class="total-box">
                        <tr>
                            <td style="text-align:right; color:var(--text-muted);">Subtotal</td>
                            <td id="showSubtotal" style="text-align:right; font-weight:600;">₹0.00</td>
                        </tr>
                        <tr>
                            <td style="text-align:right; color:var(--text-muted);">GST Tax Amount</td>
                            <td id="showGSTAmount" style="text-align:right; font-weight:600;">₹0.00</td>
                        </tr>
                        <tr class="grand-total">
                            <td style="text-align:right;">Grand Total Value</td>
                            <td id="showGrandTotal" style="text-align:right;">₹0.00</td>
                        </tr>
                    </table>

                    <div class="footer">
                        We hope our metrics meet validation. Looking forward to transaction confirmation processing.<br>
                        
                        <div class="signature">
                            Best Regards,<br><br>
                            <strong>For Janak Positioning & Surveying Systems Pvt. Ltd.</strong><br><br><br>
                            <span id="showSenderName" style="font-weight: 600; text-decoration: underline;">[Authorized Signatory]</span><br>
                            <span id="showSenderMobile"></span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<script>
// Mock Memory Persistence State for App Engine demo runtime tracking
let currentActiveSession = { user: "", role: "", status: "Active" };
let selectedGateRole = "";

let staffDirectoryDb = [
    { name: "Amit Sharma", username: "amit1", role: "Standard Staff", status: "Active" },
    { name: "Priya Nair", username: "priya2", role: "Senior Executive", status: "Active" }
];

function showLoginGate(role) {
    selectedGateRole = role;
    document.getElementById("loginFormGate").classList.remove("hidden");
    document.getElementById("loginGateTitle").innerText = role === 'admin' ? "Admin Central Passcode Verification" : "Staff Directory Login Gateway";
    document.getElementById("gateUser").value = role === 'admin' ? "admin" : "amit1";
}

function processSystemLogin() {
    let uInput = document.getElementById("gateUser").value;
    let pInput = document.getElementById("gatePass").value;

    if(pInput !== "1245") {
        alert("Incorrect security PIN profile provided.");
        return;
    }

    if(selectedGateRole === 'admin' && uInput === 'admin') {
        currentActiveSession = { user: "Administrator Manager", role: "Admin", status: "Unrestricted" };
    } else {
        let profile = staffDirectoryDb.find(x => x.username === uInput);
        if(!profile) {
            alert("No registered account found mapping this handle tag.");
            return;
        }
        if(profile.status === 'Blocked') {
            alert("This user profile account has been suspended by Administration.");
            return;
        }
        currentActiveSession = { user: profile.name, role: profile.role, status: "Active" };
    }

    initializeWorkspaceSession();
}

function initializeWorkspaceSession() {
    document.getElementById("portalView").classList.add("hidden");
    document.getElementById("appWorkspace").classList.remove("hidden");
    
    document.getElementById("userBadge").innerText = currentActiveSession.user;
    document.getElementById("roleBadge").innerText = currentActiveSession.role;

    if(currentActiveSession.role === 'Admin') {
        document.getElementById("adminPanelBlock").classList.remove("hidden");
        setFormInputsRestriction(false);
    } else {
        document.getElementById("adminPanelBlock").classList.add("hidden");
        // Staff validation tracking rules
        if(currentActiveSession.role === 'Standard Staff') {
            setFormInputsRestriction(true); // Locks pricing modifications 
        } else {
            setFormInputsRestriction(false); // Senior Staff can configure pricing structures
        }
    }
    renderDirectoryTable();
}

function setFormInputsRestriction(restrict) {
    // If restricted, workers cannot manipulate the foundational base price matrix tags
    let elements = document.querySelectorAll(".price, .gst, .itemCategory, #addItemsBtn");
    elements.forEach(el => {
        if(restrict) {
            el.setAttribute("disabled", "true");
            if(el.tagName === 'BUTTON') el.style.display = "none";
        } else {
            el.removeAttribute("disabled");
            if(el.tagName === 'BUTTON') el.style.display = "inline-block";
        }
    });
}

function logoutWorkspace() {
    document.getElementById("appWorkspace").classList.add("hidden");
    document.getElementById("loginFormGate").classList.add("hidden");
    document.getElementById("portalView").classList.remove("hidden");
}

/* ADMIN MATRIX MANAGEMENT OPERATIONS */
function renderDirectoryTable() {
    let html = "";
    staffDirectoryDb.forEach((staff, index) => {
        html += `<tr>
            <td><strong>${staff.name}</strong></td>
            <td>@${staff.username}</td>
            <td><span style="font-size:12px; font-weight:600; padding:2px 6px; border-radius:3px; background:#e9ecef;">${staff.role}</span></td>
            <td><span style="color: ${staff.status === 'Active' ? 'green':'red'}; font-weight:700;">${staff.status}</span></td>
            <td>
                <button class="btn-secondary btn-sm" onclick="toggleStaffStatus(${index})">Toggle Hold</button>
                <button class="btn-danger btn-sm" onclick="purgeStaffProfile(${index})">Purge</button>
            </td>
        </tr>`;
    });
    document.getElementById("directoryTableBody").innerHTML = html || `<tr><td colspan="5" style="text-align:center; color:#999;">No personnel profiles registered.</td></tr>`;
}

function addNewStaffProfile() {
    let name = document.getElementById("newStaffName").value;
    let user = document.getElementById("newStaffUser").value;
    let role = document.getElementById("newStaffRole").value;

    if(!name || !user) { alert("Complete standard credentials setup first."); return; }
    staffDirectoryDb.push({ name: name, username: user, role: role, status: "Active" });
    
    document.getElementById("newStaffName").value = "";
    document.getElementById("newStaffUser").value = "";
    renderDirectoryTable();
}

function toggleStaffStatus(idx) {
    staffDirectoryDb[idx].status = staffDirectoryDb[idx].status === 'Active' ? 'Blocked' : 'Active';
    renderDirectoryTable();
}

function purgeStaffProfile(idx) {
    if(confirm("Confirm profile wipe context removal?")) {
        staffDirectoryDb.splice(idx, 1);
        renderDirectoryTable();
    }
}

/* WORKSPACE RESPONSIVE FRAMING OPERATIONS */
function toggleMobileView(isMobile) {
    let wrapper = document.getElementById("previewWrapper");
    if(isMobile) {
        wrapper.classList.add("mobile-view");
    } else {
        wrapper.classList.remove("mobile-view");
    }
}

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
        <button class="btn-danger btn-sm" onclick="removeRow(this)">Delete</button>
    </td>`;
    tbody.appendChild(tr);
    if(currentActiveSession.role === 'Standard Staff') setFormInputsRestriction(true);
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
        document.getElementById("outputTableBody").innerHTML = `<tr><td colspan="8" style="color: #999; padding: 20px; text-align:center;">No items configured.</td></tr>`;
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
                    <td>${item.imageURL ? `<img src="${item.imageURL}">` : `<span style="color:#999; font-size:11px;">No Image</span>`}</td>
                    <td>${item.qty}</td>
                    <td>₹${item.price.toLocaleString('en-IN', {minimumFractionDigits: 2})}</td>
                    <td>${item.gst}%</td>
                    <td style="font-weight:600;">₹${item.itemTotal.toLocaleString('en-IN', {minimumFractionDigits: 2})}</td>
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
    generateQuotation();
    applyPageLayout();
    window.print();
}
</script>
</body>
</html>
