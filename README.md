<article>

<h1>VEHICLE</h1>
<h2>Viewstate Hidden Event Enumerator!</h2>
<h3>An advanced toolset for testing modern web application frameworks and rich internet applications.</h3>

<p>
VEHICLE (formerly known as ria-scip) is a pentest platform with advanced testing features for modern web application frameworks (MWAF) and rich internet applications (RIA).<br><br>
It enables testers to <b>affect various server control properties</b> and <b>enumerate & execute dormant events of invisible</b>, visible, disabled and commented server web controls 
(currently supported for <b>ASP.net</b> and <b>Mono</b>).<br><br>

These features are implemeted by abusing application mis-configurations and framework-specific programming flaws, and by manipulating proprietary input formats.<br>

The project is implemented as an extension to the <a href="http://code.google.com/p/zaproxy/" target="_blank">OWASP Zed Attack Proxy (ZAP)</a> project.
</p>

<p>Developed by <a href="http://www.hacktics.com" target="_blank">Hacktics ASC</a><br>
<a href="http://www.hacktics.com" target="_blank"><img src="http://diviner.googlecode.com/files/hacktics_logo.jpg" /></a></p>

<p>
<h2>Requirements:</h2>
<ul>
<li> VEHICLE requires Java <u>1.7.x</u>, and was tested with ZAP <u>v.2.x</u>.</li>
<li> Verify that ZAP proxy is executed using Java 1.7.x, prior to running the installer.</li>
</ul>
</p>

<p><h2>How Does it Work?</h2>
VEHICLE can locate insecure ASP.net configuration, as well as locate traces of invisible, disabled and commented controls and events. It can then be used to enumerate invisible controls, and execute dormant events of server controls by forging a valid postback call (invisible controls without event validation or disabled & commented controls in any scenario), or by reconstructing the viewstate and eventvalidation fields of invisible controls (in case the eventvalidation is on but the MAC is off).<br>
<br>
VEHICLE also provides a manual interface for performing additional RIA/ASP.net targeted attacks such as reusing hijacked viewstate/eventvalidation fields, reconstructing viewstate fields after content alteration/parameter tampering, etc.<br>
<hr/>
<a href="http://ria-scip.googlecode.com/svn/wiki/images/SCIP-RIA%20Event%20Enumerator.png">VEHICLE in action - Image</a><br>
<a href="http://www.youtube.com/watch?v=0c8Y7TlXcWs">VEHICLE (a.k.a ria-scip) in action - Demo Video</a>
<br>
</p>

<p>
<h2>Quickstart</h2>
VEHICLE can currently be used by right-clicking on any ASP.net page in ZAP's treeview. <br>
Currently supports ASP.net, while the next release will support mono and additional technologies.
</p>

<p>
<h2>Developers</h2>
VEHICLE is developed and maintained by <a href="https://twitter.com/nashcontrol" rel="nofollow">Alex Mor</a>, <a href="https://twitter.com/sectooladdict" rel="nofollow">Shay Chen</a> and <a href="https://twitter.com/nivselatwit" rel="nofollow">Niv Sela</a>.<br>
The development team also includes <a href="https://twitter.com/michal_golds">Michal Goldstein</a> and Alon Friedman.
</p>

<p>
<h2>Features</h2>

<table border="0">
<tr><td><b><u>Event Execution Features</u></b></td></tr>
<tr><td valign="top">
<ul>
<li><I>Event Execution of Disabled / Commented Controls</I></li>
<li><I>Event Execution of Invisible Controls (When the Event Validation is OFF)</I></li>
<li><I>Event Execution of Invisible Controls (When the Viewstate MAC is OFF)</I></li>
<li><I>Manual Event Execution of Optional Events (MAC/Validation is OFF)</I></li>
<li><I>Event Execution of Invisible Controls using Cached EventValidation from Wayback Machine (Even when the MAC and Validation are ON)</I></li>
<li><I>Server Control Property Injection / Override (When the Viewstate MAC is OFF)</I></li>
<li><I>Edit the Viewstate Field (When the Viewstate MAC is OFF)</I></li>
<li><I>Property Override using Cached Viewstate from Wayback Machine (Even when the MAC and Validation are ON)</I></li>
</ul>
</td></tr>

<tr><td><b><u>Additional Features</u></b></td></tr>
<tr><td valign="top">
<ul>
<li><I>Error-Based Control Name Enumeration</I></li>
<li><I>Blind Control Name Enumeration</I></li>
<li><I>Viewstate/EventValidation Reconstruction (Assist in Control Value Manipulation)</I></li>
<li><I>Obtain, Compare and Reuse Snapshots of Previous Viewstate/EventValidation fields from Wayback Machine</I></li>
</ul>
</td></tr>

<tr><td><b><u>Technology Support</u></b></td></tr>
<tr><td valign="top">
<ul>
<li><I>ASP.net postbacks / Viewstate 2</I></li>
<li><I>Upcoming: Support for Mono / Callbacks / Viewstate 1</I></li>
</ul>
</td></tr>

<tr><td><b><u>Integration Support</u></b></td></tr>
<tr><td valign="top">
<ul>
<li><I>Integration With ZAP's 'Resend Request' Feature</I></li>
<li><I>Integration With the Page Resurrection features of the DejaVu ZAP extension</I></li>
</ul>
</td></tr>

</table>
</p>

<p>
<h2>Copyright</h2>
</p>
<p>VEHICLE - An advanced toolset for testing modern web application frameworks and rich internet applications.</p>

<p>Copyright (C) 2013, Hacktics ASC, Ernst & Young.</p>

<p>This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.</p>

<p>This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.</p>

<p>You should have received a copy of the GNU General Public License along with this program.  If not, see <a href="http://www.gnu.org/licenses/">http://www.gnu.org/licenses</a>.</p>

</article>