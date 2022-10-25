<img src="easyi3.svg" width="100%" height="100%">

<h2 id="this-script-is-intended-to-be-used-on-a-headless-arch-or-debian-based-distribution.">This script is intended to be used on a headless Arch or Debian. Not for Ubuntu do to "sane" locked root.</h2>
<h6 id="this-includes-ubuntu-server-manjaro-linux-mint-endeavour-os-kali-linux-arch4arm-and-more">This includes Ubuntu Server, Manjaro, Linux Mint, Endeavour Os, Kali Linux, Arch4Arm and more</h6>
<p>The end result being an i3 window manager with all it’s depend’s, network monitoring, work load balancing, an advanced intrusion detection system and general performance enhancements set by default.</p>
<p>Wallpapers are sourced from your ~/Pictures folder making it quick and easy and Rofi was made transparent and full screen to maximize screen space.</p>
<p>The packages will vary depending on your distro:</p>
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
<td>rofi</td>
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
<td>curl</td>
<td>y</td>
<td>y</td>
<td>n</td>
</tr>
<tr class="odd">
<td>network-manager-openvpn-gnome</td>
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

</tbody>
</table>
<p>A desktop item will be created in ‘/etc/xdg/autostart/’ that automatically sets your CPU Frequency Governor to ‘Performance’ mode.</p>
<p>Lastly, this script will curl/wget two other packages I find highly-useful/essential:</p>
<div>
<html>
<a href="https://github.com/soimort/translate-shell">Translator</a> <a href="https://github.com/sdushantha/tmpmail">Tmpmail</a>
</html>
</div>
<hr />
<h2 id="on-debian">On Debian</h2>
<p>When the install script is run it authors a second script in your home folder called ‘root.’ When this script is run as root it will compress your bootloader using lz4 and z3fold- which makes for faster boot times. It is not necessary to run this script. However, easyi3 will attempt to. This function is still in testing and <em>might</em> not work. If so simply terminate the program- all of the heavy work will be done by then- then run:</p>
<div class="sourceCode" id="cb4"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb4-1"><a href="#cb4-1" aria-hidden="true"></a><span class="fu">su</span> root</span>
<span id="cb4-2"><a href="#cb4-2" aria-hidden="true"></a><span class="fu">bash</span> root</span></code></pre></div>
<h2 id="on-arch">On Arch</h2>
<p>There is no root script. I’m assuming if you are on Arch you can manage your own kernel.</p>
<hr />
<h2 id="to-use">To use</h2>
<p>First, download and install of any Headless Arch or Debian based distribution then establish a network connection. Install git by running</p>
<div class="sourceCode" id="cb5"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb5-1"><a href="#cb5-1" aria-hidden="true"></a><span class="fu">sudo</span> pacman -Ss git <span class="kw">||</span> <span class="fu">sudo</span> apt install git</span></code></pre></div>
<p>Then run:</p>
<div class="sourceCode" id="cb6"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb6-1"><a href="#cb6-1" aria-hidden="true"></a><span class="fu">git</span> clone https://www.github.com/ZZZlax/easyi3 <span class="kw">&amp;&amp;</span> <span class="bu">cd</span> easyi3 <span class="kw">&amp;&amp;</span> <span class="fu">bash</span> easyi3</span></code></pre></div>
<p>The script should begin with either</p>
<blockquote>
<p>Setting up keyring</p>
</blockquote>
<p>or</p>
<blockquote>
<p>Updating apt cache</p>
</blockquote>
<hr />
<div>
<html>
<a href="https://github.com/ohmyzsh/ohmyzsh">Ohmyzsh</a> <a href="https://github.com/zsh-users/fizsh">Fizsh</a> <a href="https://github.com/topics/zsh-plugins">ZSH Plugins</a>
</html>
</div>
<hr />
<p>If you try to run easy i3 on a distro that doesn’t use apt or pacman the script will fail. Feel free to install the packages listed one by one and list which ones are available for your distribution and join the development!</p>
<p>Thanks, hope this helps!</p>
