<!doctype html><html lang="en"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1"><title>README | King of Kings Portal</title>
<style>body{font:16px/1.65 system-ui,Segoe UI,Arial,sans-serif;background:#f3fbf5;color:#0f2a1d;margin:0;padding:32px 18px}main{max-width:760px;margin:auto;background:#fff;border:1px solid #e0eee5;border-radius:20px;padding:32px}h1{font-size:1.8rem;line-height:1.2;color:#145233;margin-top:0}h2{font-size:1.2rem;color:#1d6e44;margin-top:1.8em;border-bottom:2px solid #fbd0dd;padding-bottom:6px}p{margin:.7em 0;color:#2d4a3b}li{margin:.35em 0}a{color:#1d6e44;font-weight:600}</style></head><body><main>
<h1>King of Kings International School: Website and Portal Prototype</h1>
<p>A clickable prototype of the school website with portals for parents, students, teachers and school leadership. It runs fully in the browser. All data shown is sample data kept in your own browser.</p>
<h2>How to open it on a laptop (Windows)</h2>
<p>Easiest way:</p>
<ol>
<li>Extract the zip file so you can see this README and the file called index.html.</li>
<li>Double click start.bat. A black window opens and your browser loads the site at <a href="http://localhost:8080">http://localhost:8080</a>.</li>
<li>Leave the black window open while you use the site. Press Ctrl and C in it, or close it, to stop.</li>
</ol>
<p>If start.bat does not work, do it by hand:</p>
<ol>
<li>Open the extracted folder in File Explorer, click the address bar, type cmd and press Enter.</li>
<li>Type: py -m http.server 8080 (if that fails, try: python -m http.server 8080).</li>
<li>Open Chrome and go to <a href="http://localhost:8080">http://localhost:8080</a></li>
</ol>
<p>Python must be installed. Get it from python.org if needed. Node users can run: npx serve -l 8080</p>
<p>Double clicking index.html also shows the pages, but use the steps above for the best result.</p>
<h2>How to open it on a phone</h2>
<ol>
<li>Keep the laptop server running and connect the phone to the same wifi.</li>
<li>On the laptop, open a command window and type ipconfig. Note the IPv4 Address, for example 192.168.1.5.</li>
<li>On the phone, open Chrome or Safari and go to <a href="http://192.168.1.5:8080">http://192.168.1.5:8080</a> using your own number.</li>
<li>If it will not load, allow Python through the Windows firewall on private networks.</li>
</ol>
<h2>Demo logins</h2>
<p>Open portal.html (the Portal Login button). Pick Primary School or College, then a role. The password for every account is demo123.</p>
<p>Parent: par1 (two children), par2, par3</p>
<p>Student: KKI/P/001 (Primary 4), KKI/C/001 (JSS 2)</p>
<p>Teacher: T001 (Primary), T003 (College)</p>
<p>Leadership: HT01 Head Teacher, PR01 Principal, BU01 Bursar, PO01 Proprietor</p>
<h2>What to try</h2>
<ol>
<li>Parent: sign in as par1, open Pay School Fees, choose items, pay by card, and see the receipt.</li>
<li>Leadership: sign in as BU01 and open Fees and Payments. The payment from step 1 appears there.</li>
<li>Teacher: sign in as T001, open Score Entry, change a score and save.</li>
<li>Leadership: open Results Control to publish or hide results. Students and parents only see published results.</li>
<li>Website: submit the Admissions form, then see it under Applications in the leadership dashboard.</li>
</ol>
<p>Use Reset demo data on the login page to return to the starting sample data.</p>
<h2>Folder guide</h2>
<p>index.html, about.html, academics.html, admissions.html, gallery.html, news.html, contact.html: public website</p>
<p>portal.html: login page for all portals</p>
<p>student.html, parent.html, teacher.html, admin.html: dashboards</p>
<p>assets/css/style.css: all styling (light green with soft pink)</p>
<p>assets/js/app.js: shared navigation, sample data and storage</p>
<p>assets/js/portal.js: dashboard screens and logic</p>
<p>assets/img: school photos and crest</p>
<p>manifest.webmanifest and sw.js: let the portal be installed as a phone app (works when served from a web address)</p>
<h2>Important notes</h2>
<p>This is a prototype. Payments are simulated and no money moves. Data is stored only in the browser being used, so a payment made on one device does not appear on another. A live version needs a real database, secure sign in, and a payment gateway such as Paystack or Flutterwave.</p>
<p>Fees, staff names, student names and scores are sample data and should be replaced with the school's real records.</p>
<p>This copy uses the school's real name and photos. Keep it on your own devices and show it in person. Publish the final site only on hosting the school owns or has approved.</p>
<p>Prototype designed by GloxadX.</p>
</main></body></html>
