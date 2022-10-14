<img src="ezi3.svg" width="100%" height="100%">

<h2 id="this-script-is-intended-to-be-used-on-a-headless-arch-or-debian-based-distribution.">This script is intended to be used on a headless Arch or Debian-based distribution.</h2>
<h6 id="this-includes-ubuntu-server-manjaro-linux-mint-endeavour-os-kali-linux-arch4arm-and-more">This includes Ubuntu Server, Manjaro, Linux Mint, Endeavour Os, Kali Linux, Arch4Arm and more</h6>
<p>The end result being an i3 window manager with all it’s depend’s, a torrified ZSH shell, network monitoring, work load balancing, an advanced intrusion detection system and general performance enhancements set by default.</p>
<p>Alias’s are preconfigured for bleachbit and system matinence:</p>
<p>Bleachbit as user:</p>
<div class="sourceCode" id="cb1"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb1-1"><a href="#cb1-1" aria-hidden="true"></a><span class="ex">clean</span></span></code></pre></div>
<p>Bleachbit as root:</p>
<div class="sourceCode" id="cb2"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb2-1"><a href="#cb2-1" aria-hidden="true"></a><span class="ex">deep-clean</span></span></code></pre></div>
<p>Update package manager cache, upgrade all pkgs and remove unused packages:</p>
<div class="sourceCode" id="cb3"><pre class="sourceCode bash"><code class="sourceCode bash"><span id="cb3-1"><a href="#cb3-1" aria-hidden="true"></a><span class="ex">rolling</span></span></code></pre></div>
<p>Aswell as global alias’s for:</p>
<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Alias</th>
<th>Command</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>p</td>
<td>python3</td>
<td>Call .py scripts quickly</td>
</tr>
<tr class="even">
<td>b</td>
<td>bash</td>
<td>Call Bash scripts quickly</td>
</tr>
<tr class="odd">
<td>tab</td>
<td>xfce4-terminal –tab</td>
<td>Open a new tab in the active terminal</td>
</tr>
<tr class="even">
<td>c</td>
<td>clear &amp;&amp;</td>
<td>A global prefix to clear the screen</td>
</tr>
<tr class="odd">
<td>x</td>
<td>rm -rf ~/zsh_history ; history -c</td>
<td>A global prefix to remove shell history</td>
</tr>
<tr class="even">
<td>cx</td>
<td>rm -rf ~/zsh_history ; history -c ; rm - rf .local/share/recently-used.xbel &amp;&amp; clear</td>
<td>Remove history and recently used history as well as clearing the terminal</td>
</tr>
</tbody>
</table>
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
<td>tor</td>
<td>y</td>
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
<tr class="odd">
<td>macchanger</td>
<td>n</td>
<td>y</td>
<td>y</td>
</tr>
<tr class="even">
<td>apt-transport-tor</td>
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
<h2 id="recommends">Recommends</h2>
<p>Either ohmyzsh, fizsh or cloning zsh plugins and adding them by source to your zshrc. Fizsh has the fastest load time in terminal.</p>
<hr />
<div>
<html>
<a href="https://github.com/ohmyzsh/ohmyzsh">Ohmyzsh</a> <a href="https://github.com/zsh-users/fizsh">Fizsh</a> <a href="https://github.com/topics/zsh-plugins">ZSH Plugins</a>
</html>
</div>
<hr />
<p>Using MEGAovpn located in the ZZZlax git repo with a free protonvpn account to set up all the free server configs in 1 script then setting your primary connection to connect to a VPN upon boot.</p>
<p>Using .Pyrate Browser to access the tor network on a server-side cookie proof (you read that correctly) web browser. Some of its features include automated launching of django webservers, script injection, a customizeable homescreen writen in Html5/CSS/JS, and a GUI for youtube-dl that is capiable of scraping band and album information from wikipedia and many more security and networking features.</p>
<p>And/Or Showing love to my Pinephone repo &lt;3.</p>
<hr />
<div>
<html>
<a href="https://github.com/ZZZlax/.Pyrate">.Pyrate</a> <a href="https://github.com/ZZZlax/MEGAvpn">MEGAovpn</a> <a href="https://github.com/ZZZlax/Pinephone">ZZZ’s Pinephone Repo</a> <br>
</html>
</div>
<hr />
<p>If you try to run easy i3 on a distro that doesn’t use apt or pacman the script will fail. Feel free to install the packages listed one by one and list which ones are available for your distribution and join the development!</p>
<p>Thanks, hope this helps!</p>
