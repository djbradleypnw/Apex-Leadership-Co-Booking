
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#102d50">
<meta name="description" content="Inland Apex Leadership Co. — School Event Agreement and Reservation Deposit">
<title>Inland Apex Leadership Co. | School Onboarding</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>

<style>
:root {
  --navy:#102d50;
  --blue:#1769aa;
  --orange:#f58220;
  --light:#f4f7fb;
  --ink:#172638;
  --muted:#64748b;
  --line:#dce4ed;
}
* {box-sizing:border-box}
body {
  margin:0;
  font-family:Inter,Arial,sans-serif;
  background:var(--light);
  color:var(--ink);
  line-height:1.55;
}
header {
  background:var(--navy);
  color:white;
  padding:22px 20px;
  border-bottom:5px solid var(--orange);
}
.header-inner {
  max-width:1050px;
  margin:auto;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:20px;
}
.brand {
  font-size:19px;
  font-weight:900;
  letter-spacing:.4px;
  line-height:1.2;
}
.brand span {color:var(--orange)}
.header-tag {
  font-size:12px;
  color:#dce8f5;
  text-align:right;
  font-weight:600;
}
main {
  width:min(920px, calc(100% - 28px));
  margin:36px auto 70px;
}
.panel {
  background:white;
  border:1px solid var(--line);
  border-radius:18px;
  padding:clamp(20px,4vw,38px);
  box-shadow:0 12px 35px rgba(16,45,80,.07);
}
.hidden {display:none!important}
h1 {
  color:var(--navy);
  font-size:clamp(27px,4vw,38px);
  line-height:1.15;
  margin:0 0 12px;
}
h2 {color:var(--navy);margin-top:0}
p {color:#475569}
.eyebrow {
  color:var(--orange);
  font-size:12px;
  font-weight:900;
  letter-spacing:1.5px;
  text-transform:uppercase;
  margin-bottom:10px;
}
.intro {font-size:16px;max-width:680px}
.steps {
  display:flex;
  gap:8px;
  flex-wrap:wrap;
  margin:24px 0;
}
.step {
  border-radius:30px;
  padding:8px 13px;
  background:#edf2f7;
  color:#53657a;
  font-size:12px;
  font-weight:800;
}
.step.active {background:#fff0e3;color:#a94d00}
label {
  display:block;
  color:var(--navy);
  font-weight:750;
  font-size:13px;
  margin:17px 0 7px;
}
input,textarea {
  width:100%;
  border:1px solid #cbd5e1;
  border-radius:9px;
  padding:13px 14px;
  font:inherit;
  font-size:15px;
  color:var(--ink);
  background:white;
}
input:focus,textarea:focus {
  outline:3px solid rgba(23,105,170,.13);
  border-color:var(--blue);
}
.grid {
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:0 18px;
}
button,.button {
  border:0;
  border-radius:9px;
  padding:14px 19px;
  font:inherit;
  font-weight:850;
  cursor:pointer;
  text-decoration:none;
  display:inline-flex;
  align-items:center;
  justify-content:center;
  gap:8px;
  transition:.15s ease;
}
button:hover,.button:hover {transform:translateY(-1px);filter:brightness(1.04)}
.primary {background:var(--orange);color:#fff}
.secondary {background:var(--navy);color:#fff}
.outline {background:white;color:var(--navy);border:1px solid #cbd5e1}
.button-row {display:flex;gap:12px;flex-wrap:wrap;margin-top:25px}
.button-row button {flex:1}
.small-note {font-size:12px;color:var(--muted)}
.signature-wrap {
  border:1px solid #cbd5e1;
  border-radius:12px;
  overflow:hidden;
  background:#fff;
}
#signatureCanvas {
  display:block;
  width:100%;
  height:170px;
  touch-action:none;
  cursor:crosshair;
}
.signature-tools {
  border-top:1px solid var(--line);
  padding:9px 12px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:10px;
}
.signature-tools button {
  padding:7px 12px;
  font-size:12px;
}
.error {color:#b42318;font-size:13px;font-weight:700;margin-top:10px}
.success {color:#167044;font-size:14px;font-weight:700}
.payment-option {
  border:1px solid var(--line);
  border-radius:12px;
  padding:18px;
  margin:13px 0;
}
.payment-option h3 {margin:0 0 5px;color:var(--navy)}
.payment-option p {margin:0 0 12px;font-size:14px}
.deposit-amount {
  font-size:38px;
  font-weight:900;
  color:var(--navy);
  margin:8px 0;
}
footer {
  text-align:center;
  color:#718096;
  font-size:12px;
  padding:0 20px 35px;
}
.agreement-preview {
  background:white;
  border:1px solid var(--line);
  border-radius:10px;
  padding:24px;
  margin-top:20px;
  max-height:650px;
  overflow:auto;
}
#agreementDocument {
  font-family:Arial,sans-serif;
  color:#111;
  font-size:10.5pt;
  line-height:1.38;
  background:white;
}
#agreementDocument h2 {
  color:#111;
  font-family:Arial,sans-serif;
  font-size:14pt;
  text-align:center;
  margin:0 0 20px;
}
#agreementDocument h3 {
  color:#111;
  font-family:Arial,sans-serif;
  font-size:11pt;
  margin:15px 0 4px;
}
#agreementDocument p {color:#111;margin:7px 0}
#agreementDocument .field {
  display:inline-block;
  border-bottom:1px solid #111;
  min-width:140px;
  padding:0 3px 2px;
  font-weight:600;
}
#agreementDocument .signature-image {
  max-width:230px;
  max-height:75px;
  object-fit:contain;
  display:block;
  margin:3px 0;
}
#agreementDocument table {
  width:100%;
  border-collapse:collapse;
  margin-top:8px;
  font-size:9.5pt;
}
#agreementDocument th,#agreementDocument td {
  border:1px solid #555;
  padding:5px;
  text-align:left;
}
#agreementDocument .signature-section {margin-top:25px}
#agreementDocument .legal {white-space:normal}
@media(max-width:620px) {
  .grid {grid-template-columns:1fr}
  .header-inner {align-items:flex-start}
  .header-tag {max-width:120px}
  .button-row {flex-direction:column}
  .button-row button {width:100%}
  .panel {padding:22px 18px}
}
@media print {
  body {background:white}
  header,footer,main {display:none!important}
}
</style>
</head>

<body>
<header>
  <div class="header-inner">
    <div class="brand">INLAND <span>APEX</span><br>LEADERSHIP CO.</div>
    <div class="header-tag">SCHOOL EVENT<br>ONBOARDING</div>
  </div>
</header>

<main>
  <!-- HOME -->
  <section id="home" class="panel">
    <div class="eyebrow">Let's get your event on the calendar</div>
    <h1>Let's make this a great year.</h1>
    <p class="intro">We're excited to partner with your school! Complete your event agreement below, keep a copy for your records, and take care of your Reservation Deposit.</p>
    <div class="steps">
      <span class="step active">1. Agreement</span>
      <span class="step">2. Reservation Deposit</span>
      <span class="step">3. You're all set</span>
    </div>
    <h2>First up: your event agreement</h2>
    <p>We'll use the information you provide to fill in your Apex Event Agreement. You'll be able to review it, sign it, download a PDF copy, and submit it to our team.</p>
    <button class="primary" onclick="showPage('formPage')">Complete Event Agreement →</button>
  </section>

  <!-- FORM -->
  <section id="formPage" class="panel hidden">
    <div class="eyebrow">Step 1 of 3</div>
    <h1>School & Event Information</h1>
    <p>Enter your contact and event details below. Please double-check your email address so we can send you a copy of the completed agreement.</p>

    <form id="schoolForm" onsubmit="return false">
      <label for="customerName">School / Customer Name *</label>
      <input id="customerName" required placeholder="Example: Riverside Elementary">

      <div class="grid">
        <div>
          <label for="eventStart">Event Start Date *</label>
          <input id="eventStart" type="date" required>
        </div>
        <div>
          <label for="eventEnd">Event End Date *</label>
          <input id="eventEnd" type="date" required>
        </div>
      </div>

      <label for="eventLocation">Event Location *</label>
      <input id="eventLocation" required placeholder="School address or event location">

      <label for="customerTitle">Your Title / Position *</label>
      <input id="customerTitle" required placeholder="Example: Principal, PTO President">

      <div class="grid">
        <div>
          <label for="customerPhone">Phone Number *</label>
          <input id="customerPhone" type="tel" required placeholder="(509) 555-1234">
        </div>
        <div>
          <label for="customerEmail">Email Address *</label>
          <input id="customerEmail" type="email" required placeholder="you@school.org">
        </div>
      </div>

      <label>Customer Signature *</label>
      <p class="small-note">Use your mouse, trackpad, finger, or stylus to sign in the box below.</p>
      <div class="signature-wrap">
        <canvas id="signatureCanvas"></canvas>
        <div class="signature-tools">
          <span class="small-note">Draw your signature above</span>
          <button type="button" class="outline" onclick="clearSignature()">Clear / Redraw</button>
        </div>
      </div>

      <div id="formError" class="error" role="alert"></div>

      <div class="button-row">
        <button type="button" class="outline" onclick="showPage('home')">Back</button>
        <button type="button" class="primary" onclick="prepareAgreement()">Review Agreement →</button>
      </div>
    </form>
  </section>

  <!-- AGREEMENT -->
  <section id="agreementPage" class="panel hidden">
    <div class="eyebrow">Step 1 of 3 · Review & Submit</div>
    <h1>Your Apex Event Agreement</h1>
    <p>Review the agreement below. Your information and drawn signature have been added to the customer fields. You can download a PDF copy for your records and submit the signed agreement to our team.</p>

    <div class="agreement-preview">
      <div id="agreementDocument"></div>
    </div>

    <div id="submitStatus" class="small-note" style="margin-top:15px"></div>
    <div class="button-row">
      <button class="outline" onclick="showPage('formPage')">Back to Edit</button>
      <button class="secondary" onclick="downloadAgreement()">Download PDF</button>
      <button class="primary" id="submitButton" onclick="submitAgreement()">Submit Agreement →</button>
    </div>
    <p class="small-note">Please download your copy before leaving this page. The submission process will also email a copy to Inland Apex Leadership Co.</p>
  </section>

  <!-- PAYMENT -->
  <section id="paymentPage" class="panel hidden">
    <div class="eyebrow">Step 2 of 3</div>
    <h1>Reservation Deposit</h1>
    <p>Thanks for completing your agreement! The next step is your $750 Reservation Deposit, which reserves your event with Inland Apex Leadership Co.</p>
    <div class="deposit-amount">$750</div>

    <div class="payment-option">
      <h3>Credit / Debit Card</h3>
      <p>Pay securely through Square using a credit or debit card.</p>
      <a class="button primary" href="https://square.link/u/h1gP4Q8f" target="_blank" rel="noopener">Pay Reservation Deposit →</a>
    </div>

    <div class="payment-option">
      <h3>ACH Direct Deposit</h3>
      <p>Prefer to pay by ACH? Contact Bradley and we'll provide the direct deposit instructions securely.</p>
      <a class="button secondary" href="mailto:Bradley@apexleadershipco.com?subject=ACH%20Instructions%20-%20Reservation%20Deposit">Request ACH Instructions</a>
    </div>

    <div class="payment-option">
      <h3>Check</h3>
      <p>Checks can be made payable to:</p>
      <strong>Inland Apex Leadership Co. LLC</strong>
    </div>

    <p class="small-note">The Reservation Deposit is the $750 Booking Fee described in the Event Agreement and is applied as provided in that agreement.</p>
    <div class="button-row">
      <button class="outline" onclick="showPage('agreementPage')">Back to Agreement</button>
      <button class="primary" onclick="showPage('thankYouPage')">Continue →</button>
    </div>
  </section>

  <!-- THANK YOU -->
  <section id="thankYouPage" class="panel hidden">
    <div class="eyebrow">Step 3 of 3 · Thank You</div>
    <h1>We're excited to work with you!</h1>
    <p class="intro">Thank you for taking the time to complete your Apex Event Agreement. Our team is looking forward to serving your school and making this a great event!</p>
    <p>If you haven't already, please complete your $750 Reservation Deposit using the payment options above.</p>
    <p>Questions? Reach out to Bradley at <a href="mailto:Bradley@apexleadershipco.com">Bradley@apexleadershipco.com</a>.</p>
    <button class="secondary" onclick="showPage('paymentPage')">View Payment Options</button>
  </section>
</main>

<footer>
  Inland Apex Leadership Co. LLC · Spokane Valley, Washington<br>
  Questions? Bradley@apexleadershipco.com
</footer>

<!-- Hidden iframe receives the Apps Script response -->
<iframe name="submissionFrame" id="submissionFrame" title="Agreement submission" style="display:none"></iframe>

<script>
/*
  IMPORTANT:
  After deploying Google Apps Script, paste its Web App URL below.
*/
const GOOGLE_SCRIPT_URL = "PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE";

const APEX_AGREEMENT_TEXT = `
<p>This Apex Event Agreement Traditional (the “Agreement”) is entered into effective as of the <span class="field">{{EFFECTIVE_DATE}}</span> (“Effective Date”), by and between Inland Apex Leadership Co. LLC (hereinafter “Apex”) and <span class="field">{{CUSTOMER}}</span> (“Customer”). Customer’s profile: Grades ________ Population _________________.</p>

<p>WHEREAS, Customer desires to organize an event and conduct related promotional and educational activities as set forth below (collectively, the “Event”), in order to promote Customer as well as raise funds for Customer’s desired needs or purposes;</p>

<p>WHEREAS, Apex is in the business of organizing, marketing, and putting on fundraising events such as the Event.</p>

<p>NOW, THEREFORE, for and in consideration of the terms and conditions hereof, the parties hereto do hereby agree as follows:</p>

<h3>Apex Services.</h3>
<p>Apex agrees to plan, organize, market, promote, and conduct the Event based on the following Event details:</p>
<p>Event Name: _______________</p>
<p>Event Date: <span class="field">{{EVENT_DATE}}</span></p>
<p>Event Location: <span class="field">{{EVENT_LOCATION}}</span></p>
<p>Such services shall include the following: (i) marketing and promotional activities in connection with the Event in order to increase participation including presentations to students and teachers, including hosting a webpage for the Event within Apex’s website; (ii) contracting with sponsors; (iii) coordinate the Event course design/layout, water stations, starting lines, and finish lines; (iv) provide participant lap markers and coordinate any prizes, awards, or any special recognitions; and (v) maintain commercial general liability insurance with minimum policy limits of $1,000,000 per occurrence to cover liability for bodily injury or property damage arising out of Apex’s activities in connection with the Event.</p>

<h3>Customer Cooperation.</h3>
<p>Customer agrees to cooperate with Apex in the performance of Apex’s activities pursuant to this Agreement. Customer agrees to provide Apex with reasonable access to administrators, teachers and staff in order to promote the Event and increase participation as well as to provide leads to Apex for other marketing and sponsorship activities in order to increase total revenue for the Event. Customer grants to Apex the right to use its Brand (defined below) during the term of the Agreement solely for purposes of conducting, marketing and promoting the Event. Customer agrees to use Apex’s online system following the terms and conditions, and agrees subject to applicable law, to provide Apex directory information of student names and grade level. Any funds received directly by Apex staff in connection with the Event will be promptly remitted to Customer and will be paid in accordance with Paragraph 3 below.</p>

<h3>Fees.</h3>
<p>Upon execution of this Agreement, Customer shall pay to Apex a booking fee of $750.00 (the “Booking Fee”). Upon any cancellation of the Agreement by Customer (other than due to default by Apex), Apex shall be entitled to retain the Booking Fee as its liquidated damages and not as a penalty. Otherwise, the Booking Fee shall be applicable to, and applied to, the Apex Share of fees payable to Apex as described herein. Customer shall pay to Apex a late cancellation fee of $2,500 for any cancellation by Customer of an Event with notice less than 30 days’ prior to the Event date. All entry fees and sponsorship fees earned in connection with the Event (the “Event Revenue”) shall be paid directly by participants’ parents, guardians, and sponsors via HeritagePay as set forth in Section 5 through the Event website hosted by Apex. The percentage of total collected that will be split between Apex and Customer according to the sliding scale designated at the end of this agreement. Payment shall be made no later than 30 calendar days following the conclusion of the Event. For avoidance of doubt, if Customer elects to remit a percentage of the Event Revenue back to teachers or other school personnel, such amount may not reduce the Apex Share, which shall be calculated prior to any such remittances.</p>

<h3>HeritagePay.</h3>
<p>Customer agrees that HeritagePay will be the exclusive payment processor for all transactions related to the Event. Donors may be given the opportunity to make an additional optional donation to help defray the cost of credit card processing.</p>

<h3>Data.</h3>
<p>Customers shall only disclose to Apex those student records that qualify as “directory information” under the Family Educational Rights and Privacy Act (FERPA), 20 U.S.C. § 1232g, and its implementing regulations. Customer represents and warrants that it has designated such information as directory information in accordance with FERPA and has provided appropriate notice to parents, guardians and eligible students. Apex may use directory information received from Customer, as well as de-identified metadata and other aggregated, non-personally identifiable information derived from the use of its services, for its own internal business, research, and product development purposes, provided such use complies with applicable law. Customers shall provide parents, guardians and eligible students with the opportunity to opt out of the disclosure of directory information to Apex, in accordance with FERPA requirements. The customer is solely responsible for managing and honoring such opt-out requests. Additionally, customers shall be responsible for obtaining any required verifiable parental consent under the Children’s Online Privacy Protection Act (COPPA), 15 U.S.C. §§ 6501–6506. Customer acknowledges and agrees that it is acting as the agent for the parents for purposes of COPPA compliance and assumes full responsibility for ensuring such compliance. Notwithstanding the foregoing, the parties do not intend for Apex to collect personally identifiable information directly from children under the age of 13. Customer acknowledges and agrees that Apex may collect, use and disclose personally identifiable information as set forth in Apex’s privacy policy located at [myapexevent.com/home/privacy]. Customer further acknowledges and agrees that HeritagePay has its own privacy policy located at [https://heritagepay.myapexevent.com/terms] which shall govern information collected and/or used by HeritagePay.</p>

<h3>Term and Termination.</h3>
<p>This Agreement shall commence on the Effective Date and will terminate one year from the date of Customer’s Event or when there are no further payment questions outstanding from sponsors, whichever is later (the “Closing Date”). Either party may terminate this Agreement before the “Closing Date” upon the material breach of the other party, which breach is not cured upon ten (10) days written notice from the non-breaching party. In the event of termination, all services shall terminate except that, Apex may elect in its sole discretion to continue providing one or more of its online marketing and promotional services through the Closing Date in order to help Customer complete its fundraising efforts.</p>

<h3>Limitations of Liability.</h3>
<h3>Disclaimer of Damages.</h3>
<p>EXCEPT FOR CUSTOMER'S INDEMNITY OBLIGATIONS, NEITHER PARTY WILL BE LIABLE TO THE OTHER PARTY FOR ANY LOST REVENUE, LOST PROFITS, REPLACEMENT GOODS, LOSS OF TECHNOLOGY, RIGHTS OR SERVICES, INCIDENTAL SPECIAL, PUNITIVE, INDIRECT OR CONSEQUENTIAL DAMAGES, LOSS OF DATA, OR INTERRUPTION OF EITHER PARTY'S BUSINESS, EVEN IF THE PARTIES ARE ADVISED OF THE POSSIBILITY OF SUCH DAMAGES, WHETHER UNDER THEORY OF CONTRACT, TORT (INCLUDING NEGLIGENCE), STRICT LIABILITY OR OTHERWISE, OR DAMAGES RELATING TO ANY CLAIM.</p>

<h3>Maximum Liability.</h3>
<p>EXCEPT FOR CUSTOMER'S INDEMNITY OBLIGATIONS, EACH PARTY'S MAXIMUM AGGREGATE LIABILITY TO THE OTHER PARTY RELATED TO OR IN CONNECTION WITH THIS AGREEMENT, WHETHER BASED UPON WARRANTY, CONTRACT, NEGLIGENCE, TORT, STRICT LIABILITY OR OTHERWISE WILL NOT EXCEED IN THE AGGREGATE THE TOTAL AMOUNT OF FEES PAID AND PAYABLE BY THE CUSTOMER TO APEX UNDER THIS AGREEMENT FOR THE TWELVE-MONTH PERIOD PRIOR TO THE TIME SUCH LIABILITY AROSE.</p>

<h3>Disclaimer of Warranties.</h3>
<p>APEX DISCLAIMS ALL REPRESENTATIONS, GUARANTEES, AND WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, ANY IMPLIED WARRANTY OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, WARRANTY OF NON-INFRINGEMENT, OR IMPLIED WARRANTY ARISING OUT OF THE COURSE OF PERFORMANCE, COURSE OF DEALING, OR USAGE OF TRADE.</p>

<h3>Indemnity.</h3>
<p>Customer will indemnify, defend, and hold harmless Apex, its affiliates and their respective officers, directors, employees, agents, successors, and assigns, from and against all claims, damages and losses resulting from: (a) any violation of law by Customer, whether before, on or after the Effective Date; (b) Customer’s negligence, gross negligence or willful misconduct, including without limitation, that of its employees and agents; (c) any use by Apex of the Brand in accordance with this Agreement.</p>

<h3>Governing Law; Jurisdiction.</h3>
<p>The validity, interpretation, construction, and performance of this Agreement shall be governed by the laws of the State of Texas, without giving effect to the principles of conflict of laws. Customer and Apex irrevocably and unconditionally consent to the exclusive jurisdiction of the federal and state courts located in Harris County, Texas for all proceedings arising out of this contract or related to the parties’ relationship, and Customer and Apex agree to only institute such proceedings in those courts. Customer and Apex also waive any objection to venue in those courts based on improper venue. Customer and Apex agree that a final judgment (subject to appeals) in any such proceeding is conclusive and may be enforced in other jurisdictions by suit on the judgment or in another lawful manner. In any action or proceeding to enforce rights under this Agreement, the prevailing party will be entitled to recover costs and attorneys’ fees.</p>

<h3>Severability.</h3>
<p>In the event any provision of this Agreement is held by a tribunal of competent jurisdiction to be contrary to the law, the remaining provisions of this Agreement will remain in full force and effect.</p>

<h3>Waiver.</h3>
<p>The waiver of any breach or default of this Agreement will not constitute a waiver of any subsequent breach or default and will not act to amend or negate the rights of the waiving party.</p>

<h3>Assignment.</h3>
<p>Neither party may assign its rights or delegate its duties under this Agreement in whole or in part without the prior written consent of the other party, except that on written notice to the other party this Agreement may be assigned in whole as part of a corporate reorganization, consolidation, merger, or sale of substantially all of its assets. Any other attempted assignment or delegation will be void unless the non-assigning party consents to the assignment. This Agreement will bind and insure to the benefit of each party's successors and permitted assigns.</p>

<h3>Relationship of Parties.</h3>
<p>Apex and Customer are independent contractors, and this Agreement will not establish any relationship of partnership, joint venture, employment, franchise or agency between Apex and Customer. Neither Apex nor Customer will have the power to bind the other or incur obligations on the other's behalf without the other's prior written consent, except as otherwise expressly provided herein.</p>

<h3>Entire Agreement; Counterparts.</h3>
<p>This Agreement, including all documents incorporated herein by reference, constitute the complete and exclusive agreement between the parties with respect to the subject matter hereof, and supersedes and replaces any and all prior or contemporaneous discussions, negotiations, understandings, and agreements, written and oral, regarding such subject matter, including previously executed confidentiality agreements. This Agreement may be executed in two or more counterparts, each of which will be deemed an original, but all of which together will constitute one and the same instrument. No modifications are effective under this Agreement unless evidenced in writing and signed by both parties.</p>

<h3>Headings.</h3>
<p>The headings to the clauses of this Agreement are for ease of reference only and will not affect the interpretation or construction of this Agreement.</p>

<h3>Force Majeure.</h3>
<p>Apex will use its good faith efforts to conduct the Event on the scheduled day for the Event; provided, however, that Apex shall not be responsible for damages that result from delays or postponements of the Event due to circumstances beyond its reasonable control, including, without limitation, acts of God, weather, terrorism, pandemic, epidemic, war or government actions.</p>

<h3>Notice.</h3>
<p>Any notice hereunder shall be in writing and shall be effective: (i) the next business day following deposit with a reputable courier service for overnight delivery; or (ii) three (3) business days following deposit in the United States Mail, postage prepaid, when sent by certified mail. All notices shall be forwarded to the address below:</p>
<p>Inland Apex Leadership Co: &nbsp;&nbsp; Event Location (1a)<br>12608 E. Nora Ave,<br>Spokane Valley, WA, 99216</p>

<h3>Counterparts.</h3>
<p>This Agreement may be executed in two (2) or more counterparts, each of which shall be considered an original instrument.</p>

<h3>Exclusivity.</h3>
<p>Customer agrees that the Event shall be the only major fundraising activity for the School and PTA/O for the semester in which the Event occurs. Failing to ensure exclusivity as the major fundraiser of the semester could severely impact the success of the Event.</p>

<div class="signature-section">
<p>________________________________________________________________________________</p>
<p><strong>APEX:</strong></p>
<p>Signature: ____________________________________</p>
<p>Name: Bradley Trancygier</p>
<p>Title: Owner</p>
<br>
<p><strong>CUSTOMER:</strong></p>
<p>Signature:</p>
<img class="signature-image" src="{{SIGNATURE}}" alt="Customer drawn signature">
<p>Name: <span class="field">{{CUSTOMER}}</span></p>
<p>Title: <span class="field">{{TITLE}}</span></p>
<p>Phone: <span class="field">{{PHONE}}</span></p>
<p>Email: <span class="field">{{EMAIL}}</span></p>
</div>

<br><br>
<h3 style="text-align:center">Apex Price Scale</h3>
<table>
<tr><th>Min Collected</th><th>Max Collected</th><th>School %</th><th>Apex %</th></tr>
<tr><td>$100,001</td><td>+</td><td>60%</td><td>40%</td></tr>
<tr><td>$90,001</td><td>$100,000</td><td>59%</td><td>41%</td></tr>
<tr><td>$80,001</td><td>$90,000</td><td>58%</td><td>42%</td></tr>
<tr><td>$70,001</td><td>$80,000</td><td>57%</td><td>43%</td></tr>
<tr><td>$60,001</td><td>$70,000</td><td>56%</td><td>44%</td></tr>
<tr><td>$50,001</td><td>$60,000</td><td>55%</td><td>45%</td></tr>
<tr><td>$45,001</td><td>$50,000</td><td>54%</td><td>46%</td></tr>
<tr><td>$40,001</td><td>$45,000</td><td>53%</td><td>47%</td></tr>
<tr><td>$35,001</td><td>$40,000</td><td>52%</td><td>48%</td></tr>
<tr><td>$30,001</td><td>$35,000</td><td>51%</td><td>49%</td></tr>
<tr><td>$0</td><td>$30,000</td><td>50%</td><td>50%</td></tr>
</table>
<p style="margin-top:20px">Customer Initials: ______ (this confirms you have seen this portion)</p>
`;

let currentSignature = "";
let signatureDrawing = false;
let signatureHasInk = false;
let canvas, ctx;

function showPage(id) {
  document.querySelectorAll("main > section").forEach(s => s.classList.add("hidden"));
  document.getElementById(id).classList.remove("hidden");
  window.scrollTo({top:0,behavior:"smooth"});
}

function setupSignature() {
  canvas = document.getElementById("signatureCanvas");
  ctx = canvas.getContext("2d");
  resizeSignatureCanvas();

  canvas.addEventListener("pointerdown", startSignature);
  canvas.addEventListener("pointermove", drawSignature);
  canvas.addEventListener("pointerup", stopSignature);
  canvas.addEventListener("pointercancel", stopSignature);
  canvas.addEventListener("pointerleave", stopSignature);
}

function resizeSignatureCanvas() {
  const rect = canvas.getBoundingClientRect();
  const ratio = window.devicePixelRatio || 1;
  const previous = signatureHasInk ? canvas.toDataURL() : null;
  canvas.width = Math.max(1, Math.floor(rect.width * ratio));
  canvas.height = Math.max(1, Math.floor(rect.height * ratio));
  ctx = canvas.getContext("2d");
  ctx.scale(ratio, ratio);
  ctx.lineWidth = 2.3;
  ctx.lineCap = "round";
  ctx.lineJoin = "round";
  ctx.strokeStyle = "#102d50";
  if (previous) {
    const img = new Image();
    img.onload = () => ctx.drawImage(img,0,0,rect.width,rect.height);
    img.src = previous;
  }
}

function pointerPosition(e) {
  const r = canvas.getBoundingClientRect();
  return {x:e.clientX-r.left,y:e.clientY-r.top};
}
function startSignature(e) {
  e.preventDefault();
  signatureDrawing = true;
  canvas.setPointerCapture(e.pointerId);
  const p = pointerPosition(e);
  ctx.beginPath();
  ctx.moveTo(p.x,p.y);
  ctx.lineTo(p.x+.1,p.y+.1);
  ctx.stroke();
  signatureHasInk = true;
}
function drawSignature(e) {
  if (!signatureDrawing) return;
  e.preventDefault();
  const p = pointerPosition(e);
  ctx.lineTo(p.x,p.y);
  ctx.stroke();
}
function stopSignature() {
  signatureDrawing = false;
}
function clearSignature() {
  ctx.clearRect(0,0,canvas.width,canvas.height);
  signatureHasInk = false;
  currentSignature = "";
}
window.addEventListener("resize", () => {
  if (canvas) resizeSignatureCanvas();
});

function escapeHtml(value) {
  return String(value).replace(/[&<>"']/g, c => ({
    "&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"
  }[c]));
}
function formatDate(value) {
  if (!value) return "";
  const d = new Date(value + "T12:00:00");
  return d.toLocaleDateString("en-US",{month:"long",day:"numeric",year:"numeric"});
}
function getFormData() {
  return {
    customer:document.getElementById("customerName").value.trim(),
    start:document.getElementById("eventStart").value,
    end:document.getElementById("eventEnd").value,
    location:document.getElementById("eventLocation").value.trim(),
    title:document.getElementById("customerTitle").value.trim(),
    phone:document.getElementById("customerPhone").value.trim(),
    email:document.getElementById("customerEmail").value.trim()
  };
}
function prepareAgreement() {
  const form = document.getElementById("schoolForm");
  const error = document.getElementById("formError");
  error.textContent = "";
  if (!form.reportValidity()) return;
  if (!signatureHasInk) {
    error.textContent = "Please draw your signature before continuing.";
    return;
  }
  const data = getFormData();
  if (data.end < data.start) {
    error.textContent = "The event end date cannot be before the start date.";
    return;
  }
  currentSignature = canvas.toDataURL("image/png");
  let eventDate = formatDate(data.start);
  if (data.end !== data.start) eventDate += " – " + formatDate(data.end);

  let html = APEX_AGREEMENT_TEXT
    .replaceAll("{{EFFECTIVE_DATE}}",escapeHtml(formatDate(new Date().toISOString().slice(0,10))))
    .replaceAll("{{CUSTOMER}}",escapeHtml(data.customer))
    .replaceAll("{{EVENT_DATE}}",escapeHtml(eventDate))
    .replaceAll("{{EVENT_LOCATION}}",escapeHtml(data.location))
    .replaceAll("{{TITLE}}",escapeHtml(data.title))
    .replaceAll("{{PHONE}}",escapeHtml(data.phone))
    .replaceAll("{{EMAIL}}",escapeHtml(data.email))
    .replaceAll("{{SIGNATURE}}",currentSignature);

  document.getElementById("agreementDocument").innerHTML = html;
  document.getElementById("submitStatus").textContent = "";
  showPage("agreementPage");
}

async function makePdfBlob() {
  const element = document.getElementById("agreementDocument");
  const data = getFormData();
  const filename = "Apex-Event-Agreement-" + data.customer.replace(/[^a-z0-9]+/gi,"-") + ".pdf";
  const options = {
    margin:[12,12,12,12],
    filename,
    image:{type:"jpeg",quality:0.97},
    html2canvas:{scale:2,useCORS:true,backgroundColor:"#ffffff"},
    jsPDF:{unit:"mm",format:"letter",orientation:"portrait"},
    pagebreak:{mode:["css","legacy"]}
  };
  return await html2pdf().set(options).from(element).outputPdf("blob");
}

async function downloadAgreement() {
  const status = document.getElementById("submitStatus");
  status.textContent = "Preparing your PDF...";
  try {
    const blob = await makePdfBlob();
    const data = getFormData();
    const url = URL.createObjectURL(blob);
    const a = document.createElement("a");
    a.href = url;
    a.download = "Apex-Event-Agreement-" + data.customer.replace(/[^a-z0-9]+/gi,"-") + ".pdf";
    document.body.appendChild(a);
    a.click();
    a.remove();
    setTimeout(()=>URL.revokeObjectURL(url),30000);
    status.textContent = "Your PDF download should begin automatically.";
  } catch(err) {
    console.error(err);
    status.textContent = "We couldn't create the PDF. Please try again or print this page.";
  }
}

function submitAgreement() {
  const status = document.getElementById("submitStatus");
  const button = document.getElementById("submitButton");
  if (!GOOGLE_SCRIPT_URL.startsWith("https://script.google.com/")) {
    status.innerHTML = '<span class="error">The submission service has not been connected yet. Please contact Bradley.</span>';
    return;
  }
  if (!currentSignature) {
    status.innerHTML = '<span class="error">Your signature is missing. Please go back and sign again.</span>';
    return;
  }
  button.disabled = true;
  button.textContent = "Preparing PDF...";
  status.textContent = "Preparing your signed agreement for secure submission...";

  makePdfBlob().then(blob => {
    const reader = new FileReader();
    reader.onloadend = () => {
      const base64 = String(reader.result).split(",")[1];
      const data = getFormData();
      const frame = document.getElementById("submissionFrame");
      let gotResponse = false;

      const onFrameLoad = () => {
        if (gotResponse) return;
        gotResponse = true;
        status.innerHTML = '<span class="success">Your agreement has been submitted. Please check your email for a copy, and keep the PDF you downloaded for your records.</span>';
        button.disabled = false;
        button.textContent = "Continue to Reservation Deposit →";
        button.onclick = () => showPage("paymentPage");
      };

      frame.addEventListener("load",onFrameLoad,{once:true});

      const form = document.createElement("form");
      form.method = "POST";
      form.action = GOOGLE_SCRIPT_URL;
      form.target = "submissionFrame";
      form.style.display = "none";

      const fields = {
        pdfBase64:base64,
        filename:"Apex-Event-Agreement-" + data.customer.replace(/[^a-z0-9]+/gi,"-") + ".pdf",
        customerName:data.customer,
        customerEmail:data.email,
        eventDate:formatDate(data.start) + (data.end !== data.start ? " – " + formatDate(data.end) : ""),
        website:"Inland Apex Leadership Co. website",
        websiteEmail:"Bradley@apexleadershipco.com",
        websitePhone:data.phone,
        websiteTitle:data.title,
        websiteLocation:data.location,
        websiteHoneypot:""
      };
      Object.entries(fields).forEach(([name,value]) => {
        const input = document.createElement("input");
        input.type = "hidden";
        input.name = name;
        input.value = value;
        form.appendChild(input);
      });
      document.body.appendChild(form);
      form.submit();
      form.remove();

      status.textContent = "Submitting... Please keep this page open while the agreement is sent.";
      setTimeout(() => {
        if (!gotResponse) {
          status.innerHTML = '<span class="error">We have not received a confirmation from the submission service yet. Please keep your downloaded PDF and contact Bradley to confirm receipt.</span>';
          button.disabled = false;
          button.textContent = "Try Submission Again";
        }
      },20000);
    };
    reader.readAsDataURL(blob);
  }).catch(err => {
    console.error(err);
    status.textContent = "PDF creation failed. Please try again.";
    button.disabled = false;
    button.textContent = "Submit Agreement →";
  });
}

document.addEventListener("DOMContentLoaded",setupSignature);
</script>
</body>
</html>
