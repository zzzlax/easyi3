<img src="easyi3.svg" width="100%" height="100%">
<h1>Now even easier</h1>
<h2 id="this-script-is-intended-to-be-used-on-a-headless-arch-or-debian-based-distribution.">Run me on any Arch/Debian Distro with any Window Manager!</h2>
<p>The end result being an i3 window manager with all it’s depend’s, network monitoring, work load balancing, an advanced intrusion detection system and general performance enhancements set by default installed alongside your current window manager.</p>
<p>The packages will vary depending on your distro:</p>
<p>Select packages when prompted, only i3 turned on by default</p>
<p>package availability is as follows:</p>
<table>
<thead>
<tr class="header">
<th>Package</th>
<th>Arch</th>
<th>Debian</th>
<th>Syslinked</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>i3 meta</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>lightdm</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>git</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>trash-cli</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>axel</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>fail2ban</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>zsh</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>memcached</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>memlockd</td>
<td>n</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="even">
<td>xfce4-terminal</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>macchanger</td>
<td>n</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="even">
<td>brightnessctl</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>stacer</td>
<td>n</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>tuned</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>ufw</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="even">
<td>auditd</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>thunar</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>curl</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>feh</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>tlp</td>
<td>y</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="odd">
<td>firefox</td>
<td>y</td>
<td>n</td>
<td>n</td>
</tr>
<tr class="even">
<td>unburden-home-dir</td>
<td>n</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>nocache</td>
<td>n</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="even">
<td>network-manager-openvpn-pptp</td>
<td>n</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>network-manager-openvpn-gnome</td>
<td>n</td>
<td>y</td>
<td>n</td>
</tr>
</tbody>
</table>
<p>Lastly, this script will curl/wget two other packages I find highly-useful/essential:</p>
<div>
<html>
<a href="https://github.com/soimort/translate-shell">Translator</a> <a href="https://github.com/sdushantha/tmpmail">Tmpmail</a>
</html>
</div>
<hr />
<h2 id="to-use">To use</h2>
<p>First, download and install a fresh Arch or Debian based distribution then establish a network connection.</p>
<p>Then open type <a href="https://zzzlax.github.io/downloads/ezi3">https://zzzlax.github.io/downloads/ezi3</a> into your web browser and click "save" (no need install git first, clone this repo, or even see a webpage!) then run the script from whatever directory you downloaded it to.</p>
<p>The script should begin with a zenity GUI listing all suggested packages and a series of notifications alerting you of background progress. By default all packages are selected, feel free to remove any you dont want by unchecking them when prompted.</p>
<hr />
<p>If you try to run easy i3 on a distro that doesn’t use apt or pacman the script will fail. Feel free to install the packages listed and let me know which ones are available for your distribution or join the development!</p>
<p>Thanks, hope this helps!</p>
