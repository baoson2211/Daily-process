# INSTALLATION UBUNTU SERVER 14.04

## 2016-01-18
1. LXDE installation 

  * Run Instruction:<br />
		```$ sudo apt-get install lxde-core```
	
  * Packages had been installed:<br />
	acl at-spi2-core colord consolekit dbus-x11 dconf-gsettings-backend
	dconf-service desktop-file-utils dictionaries-common fontconfig
	fontconfig-config fonts-dejavu-core gconf-service gconf-service-backend
	gconf2 gconf2-common gcr gdisk gksu glib-networking glib-networking-common
	glib-networking-services gnome-keyring gsettings-desktop-schemas gvfs
	gvfs-backends gvfs-common gvfs-daemons gvfs-fuse gvfs-libs
	hicolor-icon-theme libarchive13 libasound2 libasound2-data libatasmart4
	libatk-bridge2.0-0 libatk1.0-0 libatk1.0-data libatspi2.0-0
	libauthen-sasl-perl libavahi-client3 libavahi-common-data libavahi-common3
	libavahi-glib1 libbluetooth3 libcairo-gobject2 libcairo2 libcdio-cdda1
	libcdio-paranoia1 libcdio13 libcolord1 libcolorhug1 libcroco3 libcups2
	libdatrie1 libdconf1 libdrm-intel1 libdrm-nouveau2 libdrm-radeon1
	libencode-locale-perl libexif12 libfile-listing-perl libfm-data libfm-extra4
	libfm-gtk-data libfm-gtk4 libfm-modules libfm4 libfont-afm-perl
	libfontconfig1 libfontenc1 libgconf-2-4 libgcr-ui-3-1 libgd3
	libgdk-pixbuf2.0-0 libgdk-pixbuf2.0-common libgif4 libgksu2-0
	libgl1-mesa-dri libgl1-mesa-glx libglade2-0 libglapi-mesa
	libgnome-keyring-common libgnome-keyring0 libgphoto2-6 libgphoto2-l10n
	libgphoto2-port10 libgraphite2-3 libgtk-3-0 libgtk-3-bin libgtk-3-common
	libgtk2.0-0 libgtk2.0-bin libgtk2.0-common libgtop2-7 libgtop2-common
	libgudev-1.0-0 libgusb2 libharfbuzz0b libhtml-form-perl libhtml-format-perl
	libhtml-parser-perl libhtml-tagset-perl libhtml-tree-perl
	libhttp-cookies-perl libhttp-daemon-perl libhttp-message-perl
	libhttp-negotiate-perl libice6 libicu52 libid3tag0 libieee1284-3 libimlib2
	libimobiledevice4 libio-html-perl libio-socket-inet6-perl
	libio-socket-ssl-perl libjasper1 libjbig0 libjpeg-progs libjpeg-turbo-progs
	libjpeg-turbo8 libjpeg8 liblcms2-2 libldb1 libllvm3.4 libltdl7
	liblwp-mediatypes-perl liblwp-protocol-https-perl liblzo2-2
	libmailtools-perl libmenu-cache-bin libmenu-cache3 libmtp-common
	libmtp-runtime libmtp9 libnet-http-perl libnet-smtp-ssl-perl
	libnet-ssleay-perl libnettle4 libntdb1 libobrender29 libobt2
	libp11-kit-gnome-keyring libpam-ck-connector libpam-gnome-keyring
	libpango-1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 libpangoxft-1.0-0
	libpciaccess0 libpixman-1-0 libplist1 libproxy1 librsvg2-2 librsvg2-common
	libsane libsane-common libsecret-1-0 libsecret-common libsm6 libsmbclient
	libsocket6-perl libsoup2.4-1 libstartup-notification0 libtalloc2 libtdb1
	libtevent0 libthai-data libthai0 libtiff5 libtxc-dxtn-s2tc0 libudisks2-0
	liburi-perl libusbmuxd2 libutempter0 libv4l-0 libv4lconvert0 libvpx1
	libwayland-client0 libwayland-cursor0 libwbclient0 libwnck-common libwnck22
	libwww-perl libwww-robotrules-perl libx11-xcb1 libxaw7 libxcb-dri2-0
	libxcb-dri3-0 libxcb-glx0 libxcb-present0 libxcb-render0 libxcb-shape0
	libxcb-shm0 libxcb-sync1 libxcb-util0 libxcomposite1 libxcursor1 libxdamage1
	libxfixes3 libxft2 libxi6 libxinerama1 libxkbcommon0 libxmu6 libxpm4
	libxrandr2 libxrender1 libxres1 libxshmfence1 libxt6 libxtst6 libxv1
	libxxf86dga1 libxxf86vm1 lxde-common lxde-core lxde-icon-theme lxmenu-data
	lxpanel lxsession lxsession-data lxsession-logout miscfiles obconf openbox
	p11-kit p11-kit-modules pcmanfm python-talloc python-xdg samba-libs udisks2
	usbmuxd x11-common x11-utils xbitmaps xscreensaver xscreensaver-data xterm

  * Issue:<br />
	locale: Cannot set LC_ALL to default locale: No such file or directory

  * Solution:<br />
	Add variable LC_ALL='en_US.utf8' in /etc/environment

  * State:<br />
	Purged and be instead by ubuntu-desktop

2. xinit installation

  *	Run Instruction:<br />
		```$ sudo apt-get install xinit```

  *	Packages had been installed:<br />
	libegl1-mesa libegl1-mesa-drivers libgbm1 libglamor0 libmtdev1
	libopenvg1-mesa libwayland-egl1-mesa libwayland-server0 libxatracker2
	libxcb-xfixes0 libxfont1 libxkbfile1 libxvmc1 x11-xkb-utils xfonts-base
	xfonts-encodings xfonts-utils xinit xserver-common xserver-xorg
	xserver-xorg-core xserver-xorg-input-all xserver-xorg-input-evdev
	xserver-xorg-input-mouse xserver-xorg-input-synaptics
	xserver-xorg-input-vmmouse xserver-xorg-input-wacom xserver-xorg-video-all
	xserver-xorg-video-ati xserver-xorg-video-cirrus xserver-xorg-video-fbdev
	xserver-xorg-video-glamoregl xserver-xorg-video-intel
	xserver-xorg-video-mach64 xserver-xorg-video-mga
	xserver-xorg-video-modesetting xserver-xorg-video-neomagic
	xserver-xorg-video-nouveau xserver-xorg-video-openchrome
	xserver-xorg-video-qxl xserver-xorg-video-r128 xserver-xorg-video-radeon
	xserver-xorg-video-s3 xserver-xorg-video-savage
	xserver-xorg-video-siliconmotion xserver-xorg-video-sis
	xserver-xorg-video-sisusb xserver-xorg-video-tdfx xserver-xorg-video-trident
	xserver-xorg-video-vesa xserver-xorg-video-vmware

  * Issue:<br />

  * Solution:<br />

  * Modify:<br />

  * State:<br />
	Purged

3. Ubuntu desktop intallation

  *	Run Instruction:<br />
		```$ sudo apt-get install ubuntu-desktop```

  *	Packages had been installed:<br />
	account-plugin-aim account-plugin-facebook account-plugin-flickr
	account-plugin-google account-plugin-jabber account-plugin-salut 
	account-plugin-twitter account-plugin-yahoo acl acpi-support 
	activity-log-manager activity-log-manager-control-center adium-theme-ubuntu 
	aisleriot alsa-base alsa-utils anacron apg app-install-data 
	app-install-data-partner appmenu-qt appmenu-qt5 apport-gtk aptdaemon 
	aptdaemon-data apturl apturl-common aspell aspell-en at-spi2-core 
	avahi-autoipd avahi-daemon avahi-utils bamfdaemon baobab bluez bluez-alsa 
	bluez-cups branding-ubuntu brasero brasero-cdrkit brasero-common brltty 
	checkbox-gui checkbox-ng checkbox-ng-service cheese cheese-common colord 
	compiz compiz-core compiz-gnome compiz-plugins-default cpp cpp-4.8 
	cracklib-runtime cups cups-browsed cups-bsd cups-client cups-common 
	cups-core-drivers cups-daemon cups-filters cups-filters-core-drivers 
	cups-pk-helper cups-ppdc cups-server-common dbus-x11 dc dconf-cli 
	dconf-gsettings-backend dconf-service deja-dup deja-dup-backend-gvfs 
	desktop-file-utils dialog dictionaries-common diffstat dmz-cursor-theme 
	dnsmasq-base doc-base duplicity dvd+rw-tools empathy empathy-common enchant 
	eog espeak-data evince evince-common evolution-data-server 
	evolution-data-server-common evolution-data-server-online-accounts 
	example-content file-roller firefox folks-common fontconfig 
	fontconfig-config fonts-dejavu-core fonts-droid fonts-freefont-ttf 
	fonts-kacst fonts-kacst-one fonts-khmeros-core fonts-lao fonts-liberation 
	fonts-lklug-sinhala fonts-nanum fonts-opensymbol fonts-sil-abyssinica 
	fonts-sil-padauk fonts-takao-pgothic fonts-thai-tlwg fonts-tibetan-machine 
	fonts-tlwg-garuda fonts-tlwg-kinnari fonts-tlwg-loma fonts-tlwg-mono 
	fonts-tlwg-norasi fonts-tlwg-purisa fonts-tlwg-sawasdee 
	fonts-tlwg-typewriter fonts-tlwg-typist fonts-tlwg-typo fonts-tlwg-umpush 
	fonts-tlwg-waree foomatic-db-compressed-ppds friends friends-dispatcher 
	friends-facebook friends-twitter gcc gcc-4.8 gconf-service 
	gconf-service-backend gconf2 gconf2-common gcr gdb gdisk gedit gedit-common 
	genisoimage geoclue geoclue-ubuntu-geoip gettext ghostscript ghostscript-x 
	gir1.2-accounts-1.0 gir1.2-appindicator3-0.1 gir1.2-atk-1.0 gir1.2-atspi-2.0 
	gir1.2-dbusmenu-glib-0.4 gir1.2-dee-1.0 gir1.2-ebook-1.2 
	gir1.2-ebookcontacts-1.2 gir1.2-edataserver-1.2 gir1.2-freedesktop 
	gir1.2-gdata-0.0 gir1.2-gdkpixbuf-2.0 gir1.2-gmenu-3.0 
	gir1.2-gnomebluetooth-1.0 gir1.2-gnomekeyring-1.0 gir1.2-goa-1.0 
	gir1.2-gst-plugins-base-1.0 gir1.2-gstreamer-1.0 gir1.2-gtk-3.0 
	gir1.2-gtksource-3.0 gir1.2-gudev-1.0 gir1.2-ibus-1.0 
	gir1.2-javascriptcoregtk-3.0 gir1.2-messagingmenu-1.0 
	gir1.2-networkmanager-1.0 gir1.2-notify-0.7 gir1.2-packagekitglib-1.0 
	gir1.2-pango-1.0 gir1.2-peas-1.0 gir1.2-rb-3.0 gir1.2-secret-1 
	gir1.2-signon-1.0 gir1.2-soup-2.4 gir1.2-totem-1.0 gir1.2-totem-plparser-1.0 
	gir1.2-udisks-2.0 gir1.2-unity-5.0 gir1.2-vte-2.90 gir1.2-webkit-3.0 
	gir1.2-wnck-3.0 gkbd-capplet glib-networking glib-networking-common 
	glib-networking-services gnome-accessibility-themes gnome-bluetooth 
	gnome-calculator gnome-contacts gnome-control-center-shared-data 
	gnome-desktop3-data gnome-disk-utility gnome-font-viewer gnome-icon-theme 
	gnome-icon-theme-symbolic gnome-keyring gnome-mahjongg gnome-menus 
	gnome-mines gnome-orca gnome-power-manager gnome-screensaver 
	gnome-screenshot gnome-session-bin gnome-session-canberra 
	gnome-session-common gnome-settings-daemon-schemas gnome-sudoku 
	gnome-system-log gnome-system-monitor gnome-terminal gnome-terminal-data 
	gnome-user-guide gnome-user-share gnome-video-effects gnomine growisofs 
	gsettings-desktop-schemas gsettings-ubuntu-schemas gsfonts 
	gstreamer0.10-alsa gstreamer0.10-nice gstreamer0.10-plugins-base 
	gstreamer0.10-plugins-base-apps gstreamer0.10-plugins-good 
	gstreamer0.10-pulseaudio gstreamer0.10-tools gstreamer0.10-x 
	gstreamer1.0-alsa gstreamer1.0-clutter gstreamer1.0-nice 
	gstreamer1.0-plugins-base gstreamer1.0-plugins-base-apps 
	gstreamer1.0-plugins-good gstreamer1.0-pulseaudio gstreamer1.0-tools 
	gstreamer1.0-x gtk2-engines-murrine gtk3-engines-unico gucharmap 
	guile-2.0-libs gvfs gvfs-backends gvfs-bin gvfs-common gvfs-daemons 
	gvfs-fuse gvfs-libs hardening-includes hicolor-icon-theme hplip hplip-data 
	hud humanity-icon-theme hunspell-en-us hwdata ibus ibus-gtk ibus-gtk3 
	ibus-pinyin ibus-table im-config indicator-applet indicator-application 
	indicator-appmenu indicator-bluetooth indicator-datetime indicator-keyboard 
	indicator-messages indicator-power indicator-printers indicator-session 
	indicator-sound inputattach intel-gpu-tools intltool-debian iproute 
	iputils-arping kerneloops-daemon landscape-client-ui-install 
	language-selector-gnome libaa1 libaccount-plugin-1.0-0 
	libaccount-plugin-generic-oauth libaccount-plugin-google libaccounts-glib0 
	libaccounts-qt5-1 libappindicator3-1 libapt-pkg-perl libarchive-zip-perl 
	libarchive13 libart-2.0-2 libasan0 libasound2 libasound2-data 
	libasound2-plugins libaspell15 libasprintf-dev libassuan0 libasyncns0 
	libatasmart4 libatk-adaptor libatk-bridge2.0-0 libatk1.0-0 libatk1.0-data 
	libatkmm-1.6-1 libatomic1 libatspi2.0-0 libaudio2 libauthen-sasl-perl 
	libautodie-perl libavahi-client3 libavahi-common-data libavahi-common3 
	libavahi-core7 libavahi-glib1 libavahi-gobject0 libavc1394-0 libbamf3-2 
	libbluetooth3 libboost-date-time1.54.0 libboost-system1.54.0 
	libbrasero-media3-1 libbrlapi0.6 libburn4 libc-dev-bin libc6-dbg libc6-dev 
	libcaca0 libcairo-gobject2 libcairo2 libcairomm-1.0-1 libcamel-1.2-45 
	libcanberra-gtk-module libcanberra-gtk0 libcanberra-gtk3-0 
	libcanberra-gtk3-module libcanberra-pulse libcanberra0 libcdio-cdda1 
	libcdio-paranoia1 libcdio13 libcdparanoia0 libcdr-0.0-0 libcheese-gtk23 
	libcheese7 libclone-perl libcloog-isl4 libclucene-contribs1 libclucene-core1 
	libclutter-1.0-0 libclutter-1.0-common libclutter-gst-2.0-0 
	libclutter-gtk-1.0-0 libcmis-0.4-4 libcogl-common libcogl-pango15 libcogl15 
	libcolamd2.8.0 libcolord1 libcolorhug1 libcolumbus1 libcolumbus1-common 
	libcompizconfig0 libcrack2 libcroco3 libcrypt-passwdmd5-perl libcups2 
	libcupscgi1 libcupsfilters1 libcupsimage2 libcupsmime1 libcupsppdc1 
	libdaemon0 libdatrie1 libdbusmenu-glib4 libdbusmenu-gtk3-4 libdbusmenu-gtk4 
	libdbusmenu-qt2 libdbusmenu-qt5 libdconf1 libdecoration0 libdee-1.0-4 
	libdigest-hmac-perl libdjvulibre-text libdjvulibre21 libdmapsharing-3.0-2 
	libdotconf0 libdpkg-perl libdrm-intel1 libdrm-nouveau2 libdrm-radeon1 libdv4 
	libebackend-1.2-7 libebook-1.2-14 libebook-contacts-1.2-0 libecal-1.2-16 
	libedata-book-1.2-20 libedata-cal-1.2-23 libedataserver-1.2-18 libegl1-mesa 
	libegl1-mesa-drivers libelfg0 libemail-valid-perl libenchant1c2a libespeak1 
	libevdocument3-4 libevview3-3 libexempi3 libexif12 libexiv2-12 
	libexttextcat-2.0-0 libexttextcat-data libfarstream-0.1-0 libfarstream-0.2-2 
	libfftw3-single3 libfile-basedir-perl libfile-copy-recursive-perl 
	libfile-desktopentry-perl libfile-fcntllock-perl libfile-mimeinfo-perl 
	libflac8 libfolks-eds25 libfolks-telepathy25 libfolks25 libfontconfig1 
	libfontembed1 libfontenc1 libframe6 libfreerdp-plugins-standard libfreerdp1 
	libfriends0 libfs6 libgail-3-0 libgail-common libgail18 libgbm1 
	libgcc-4.8-dev libgconf-2-4 libgcr-ui-3-1 libgd3 libgdata-common libgdata13 
	libgdk-pixbuf2.0-0 libgdk-pixbuf2.0-common libgee-0.8-2 libgee2 libgeis1 
	libgeoclue0 libgettextpo-dev libgettextpo0 libgexiv2-2 libgl1-mesa-dri 
	libgl1-mesa-glx libglamor0 libglapi-mesa libgles2-mesa libglew1.10 
	libglewmx1.10 libglib2.0-bin libglibmm-2.4-1c2a libglu1-mesa libgmime-2.6-0 
	libgmp10 libgnome-bluetooth11 libgnome-control-center1 libgnome-desktop-3-7 
	libgnome-keyring-common libgnome-keyring0 libgnome-menu-3-0 
	libgnomekbd-common libgnomekbd8 libgoa-1.0-0b libgoa-1.0-common libgomp1 
	libgpgme11 libgphoto2-6 libgphoto2-l10n libgphoto2-port10 libgpod-common 
	libgpod4 libgrail6 libgraphite2-3 libgrip0 libgs9 libgs9-common 
	libgsettings-qt1 libgssdp-1.0-3 libgstreamer-plugins-base0.10-0 
	libgstreamer-plugins-base1.0-0 libgstreamer-plugins-good1.0-0 
	libgstreamer0.10-0 libgstreamer1.0-0 libgtk-3-0 libgtk-3-bin libgtk-3-common 
	libgtk2.0-0 libgtk2.0-bin libgtk2.0-common libgtkmm-3.0-1 
	libgtksourceview-3.0-1 libgtksourceview-3.0-common libgtop2-7 
	libgtop2-common libgucharmap-2-90-7 libgudev-1.0-0 libgupnp-1.0-4 
	libgupnp-igd-1.0-4 libgusb2 libgutenprint2 libgweather-3-6 
	libgweather-common libgxps2 libharfbuzz-icu0 libharfbuzz0b libhpmud0 libhud2 
	libhunspell-1.3-0 libhyphen0 libibus-1.0-5 libical1 libice6 libicu52 
	libido3-0.1-0 libiec61883-0 libieee1284-3 libijs-0.35 libimobiledevice4 
	libindicator3-7 libio-pty-perl libio-socket-inet6-perl libio-socket-ssl-perl 
	libipc-run-perl libipc-system-simple-perl libisl10 libisofs6 libitm1 
	libjack-jackd2-0 libjasper1 libjavascriptcoregtk-3.0-0 libjbig0 libjbig2dec0 
	libjpeg-turbo8 libjpeg8 libjson-glib-1.0-0 libjson-glib-1.0-common libjte1 
	libkpathsea6 liblangtag-common liblangtag1 liblcms2-2 libldb1 
	liblightdm-gobject-1-0 liblircclient0 liblist-moreutils-perl libllvm3.4 
	liblouis-data liblouis2 libltdl7 liblua5.2-0 liblzo2-2 libmailtools-perl 
	libmbim-glib0 libmeanwhile1 libmessaging-menu0 libmetacity-private0a 
	libmhash2 libminiupnpc8 libmission-control-plugins0 libmm-glib0 libmnl0 
	libmpc3 libmpfr4 libmspub-0.0-0 libmtp-common libmtp-runtime libmtp9 
	libmythes-1.2-0 libnatpmp1 libnautilus-extension1a libneon27-gnutls 
	libnet-dns-perl libnet-domain-tld-perl libnet-ip-perl libnet-libidn-perl 
	libnet-smtp-ssl-perl libnet-ssleay-perl libnetfilter-conntrack3 libnettle4 
	libnice10 libnl-route-3-200 libnm-glib-vpn1 libnm-glib4 libnm-gtk-common 
	libnm-gtk0 libnm-util2 libnotify-bin libnotify4 libnspr4 libnss-mdns libnss3 
	libnss3-nssdb libntdb1 libnux-4.0-0 libnux-4.0-common liboauth0 libogg0 
	libopencc1 libopenobex1 liborc-0.4-0 liborcus-0.6-0 liboxideqt-qmlplugin 
	liboxideqtcore0 liboxideqtquick0 libp11-kit-gnome-keyring 
	libpackagekit-glib2-16 libpam-gnome-keyring libpanel-applet-4-0 
	libpango-1.0-0 libpango1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 
	libpangomm-1.4-1 libpangox-1.0-0 libpangoxft-1.0-0 libpaper-utils libpaper1 
	libpciaccess0 libpeas-1.0-0 libpeas-common libperl5.18 libperlio-gzip-perl 
	libpixman-1-0 libplist1 libpocketsphinx1 libpoppler-glib8 libpoppler44 
	libportaudio2 libprotobuf8 libproxy1 libproxy1-plugin-gsettings 
	libproxy1-plugin-networkmanager libpulse-mainloop-glib0 libpulse0 
	libpulsedsp libpurple-bin libpurple0 libpwquality-common libpwquality1 
	libpython3.4 libpyzy-1.0-0 libqmi-glib0 libqpdf13 libqt4-dbus 
	libqt4-declarative libqt4-designer libqt4-help libqt4-network libqt4-opengl 
	libqt4-script libqt4-scripttools libqt4-sql libqt4-sql-mysql 
	libqt4-sql-sqlite libqt4-svg libqt4-test libqt4-xml libqt4-xmlpatterns 
	libqt5core5a libqt5dbus5 libqt5feedback5 libqt5gui5 libqt5multimedia5 
	libqt5network5 libqt5opengl5 libqt5organizer5 libqt5positioning5 
	libqt5printsupport5 libqt5qml-graphicaleffects libqt5qml5 libqt5quick5 
	libqt5sensors5 libqt5sql5 libqt5sql5-sqlite libqt5svg5 libqt5test5 
	libqt5webkit5 libqt5webkit5-qmlwebkitplugin libqt5widgets5 libqt5xml5 
	libqtassistantclient4 libqtcore4 libqtdbus4 libqtgui4 libqtwebkit4 
	libquadmath0 libraptor2-0 librasqal3 libraw1394-11 libraw9 librdf0 
	libreoffice-avmedia-backend-gstreamer libreoffice-base-core libreoffice-calc 
	libreoffice-common libreoffice-core libreoffice-draw libreoffice-gnome 
	libreoffice-gtk libreoffice-impress libreoffice-math libreoffice-ogltrans 
	libreoffice-pdfimport libreoffice-presentation-minimizer 
	libreoffice-style-galaxy libreoffice-style-human libreoffice-writer 
	librest-0.7-0 librhythmbox-core8 librsvg2-2 librsvg2-common librsync1 
	libsamplerate0 libsane libsane-common libsane-hpaio libsbc1 libsecret-1-0 
	libsecret-common libsgutils2-2 libshout3 libsignon-extension1 
	libsignon-glib1 libsignon-plugins-common1 libsignon-qt5-1 libsm6 
	libsmbclient libsndfile1 libsnmp-base libsnmp30 libsocket6-perl libsonic0 
	libsoup-gnome2.4-1 libsoup2.4-1 libspectre1 libspeechd2 libspeex1 
	libspeexdsp1 libsphinxbase1 libssh-4 libstartup-notification0 
	libsub-identify-perl libsystemd-journal0 libt1-5 libtag1-vanilla libtag1c2a 
	libtalloc2 libtcl8.6 libtdb1 libtelepathy-farstream3 libtelepathy-glib0 
	libtelepathy-logger3 libtevent0 libtext-levenshtein-perl libthai-data 
	libthai0 libtheora0 libthumbnailer0 libtiff5 libtimezonemap1 libtk8.6 
	libtotem-plparser18 libtotem0 libtxc-dxtn-s2tc0 libudisks2-0 
	libufe-xidgetter0 libunistring0 libunity-action-qt1 libunity-control-center1 
	libunity-core-6.0-9 libunity-gtk2-parser0 libunity-gtk3-parser0 
	libunity-misc4 libunity-protocol-private0 libunity-scopes-json-def-desktop 
	libunity-webapps0 libunity9 libunityvoice1 libupower-glib1 liburi-perl 
	liburl-dispatcher1 libusbmuxd2 libutempter0 libuuid-perl libv4l-0 
	libv4lconvert0 libvisio-0.0-0 libvisual-0.4-0 libvisual-0.4-plugins 
	libvncserver0 libvorbis0a libvorbisenc2 libvorbisfile3 libvpx1 libvte-2.90-9 
	libvte-2.90-common libwacom-common libwacom2 libwavpack1 libwayland-client0 
	libwayland-cursor0 libwayland-egl1-mesa libwbclient0 libwebkitgtk-3.0-0 
	libwebkitgtk-3.0-common libwebp5 libwebpmux1 libwhoopsie-preferences0 
	libwhoopsie0 libwmf0.2-7 libwmf0.2-7-gtk libwnck-3-0 libwnck-3-common 
	libwnck-common libwnck22 libwpd-0.9-9 libwpg-0.2-2 libwps-0.2-2 libx11-xcb1 
	libx86-1 libxatracker2 libxaw7 libxcb-dri2-0 libxcb-dri3-0 libxcb-glx0 
	libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-present0 libxcb-randr0 
	libxcb-render-util0 libxcb-render0 libxcb-shape0 libxcb-shm0 libxcb-sync1 
	libxcb-util0 libxcb-xkb1 libxcomposite1 libxcursor1 libxdamage1 libxfixes3 
	libxfont1 libxft2 libxi6 libxinerama1 libxkbcommon-x11-0 libxkbcommon0 
	libxklavier16 libxmu6 libxp6 libxpm4 libxrandr2 libxrender1 libxres1 
	libxshmfence1 libxss1 libxt6 libxtst6 libxv1 libxvmc1 libxxf86dga1 
	libxxf86vm1 libyajl2 libyaml-tiny-perl libyelp0 libzeitgeist-1.0-1 
	libzeitgeist-2.0-0 libzephyr4 light-themes lightdm lintian linux-libc-dev 
	linux-sound-base lp-solve make manpages-dev mcp-account-manager-uoa 
	media-player-info metacity-common mobile-broadband-provider-info 
	modemmanager mousetweaks mscompress mtools nautilus nautilus-data 
	nautilus-sendto nautilus-sendto-empathy nautilus-share network-manager 
	network-manager-gnome network-manager-pptp network-manager-pptp-gnome 
	notification-daemon notify-osd notify-osd-icons nux-tools obex-data-server 
	obexd-client onboard onboard-data oneconf oneconf-common openprinting-ppds 
	overlay-scrollbar overlay-scrollbar-gtk2 overlay-scrollbar-gtk3 
	oxideqt-codecs p11-kit p11-kit-modules patchutils pcmciautils pkg-config 
	plainbox-provider-checkbox plainbox-provider-resource-generic 
	plainbox-secure-policy plymouth-label plymouth-theme-ubuntu-logo pm-utils 
	policykit-1-gnome policykit-desktop-privileges poppler-data poppler-utils 
	pptp-linux printer-driver-c2esp printer-driver-foo2zjs 
	printer-driver-foo2zjs-common printer-driver-gutenprint 
	printer-driver-hpcups printer-driver-min12xxw printer-driver-pnm2ppa 
	printer-driver-postscript-hp printer-driver-ptouch printer-driver-pxljr 
	printer-driver-sag-gdi printer-driver-splix pulseaudio 
	pulseaudio-module-bluetooth pulseaudio-module-x11 pulseaudio-utils 
	python-aptdaemon python-aptdaemon.gtk3widgets python-cairo 
	python-commandnotfound python-crypto python-cups python-cupshelpers 
	python-dbus python-dbus-dev python-debtagshw python-defer python-dirspec 
	python-gconf python-gi python-gi-cairo python-gnomekeyring python-gobject 
	python-gobject-2 python-gtk2 python-httplib2 python-ibus python-imaging 
	python-ldb python-libxml2 python-lockfile python-lxml python-notify 
	python-ntdb python-oauthlib python-oneconf python-pexpect python-pil 
	python-piston-mini-client python-qt4 python-qt4-dbus python-renderpm 
	python-reportlab python-reportlab-accel python-samba python-sip python-smbc 
	python-talloc python-tdb python-twisted-web python-ubuntu-sso-client 
	python-xdg python-zeitgeist python3-aptdaemon python3-aptdaemon.gtk3widgets 
	python3-aptdaemon.pkcompat python3-brlapi python3-cairo python3-chardet 
	python3-checkbox-ng python3-checkbox-support python3-crypto python3-debian 
	python3-defer python3-feedparser python3-gi-cairo python3-httplib2 
	python3-louis python3-lxml python3-mako python3-markupsafe python3-oauthlib 
	python3-oneconf python3-piston-mini-client python3-pkg-resources 
	python3-plainbox python3-pyatspi python3-pyparsing python3-requests 
	python3-six python3-speechd python3-uno python3-urllib3 python3-xdg 
	python3-xkit qdbus qpdf qt-at-spi qtchooser qtcore4-l10n 
	qtdeclarative5-accounts-plugin qtdeclarative5-dialogs-plugin 
	qtdeclarative5-localstorage-plugin qtdeclarative5-privatewidgets-plugin 
	qtdeclarative5-qtfeedback-plugin qtdeclarative5-qtquick2-plugin 
	qtdeclarative5-ubuntu-ui-extras-browser-plugin 
	qtdeclarative5-ubuntu-ui-extras-browser-plugin-assets 
	qtdeclarative5-ubuntu-ui-toolkit-plugin qtdeclarative5-unity-action-plugin 
	qtdeclarative5-window-plugin remmina remmina-common remmina-plugin-rdp 
	remmina-plugin-vnc rfkill rhythmbox rhythmbox-data rhythmbox-mozilla 
	rhythmbox-plugin-cdrecorder rhythmbox-plugin-magnatune 
	rhythmbox-plugin-zeitgeist rhythmbox-plugins rtkit samba-common 
	samba-common-bin samba-libs sane-utils seahorse session-migration 
	sessioninstaller shotwell shotwell-common signon-keyring-extension 
	signon-plugin-oauth2 signon-plugin-password signon-ui signond simple-scan 
	smbclient sni-qt software-center software-center-aptdaemon-plugins 
	software-properties-gtk sound-theme-freedesktop speech-dispatcher 
	speech-dispatcher-audio-plugins sphinx-voxforge-hmm-en sphinx-voxforge-lm-en 
	ssh-askpass-gnome syslinux syslinux-common syslinux-legacy 
	system-config-printer-common system-config-printer-gnome 
	system-config-printer-udev t1utils tcl tcl8.6 telepathy-gabble 
	telepathy-haze telepathy-idle telepathy-indicator telepathy-logger 
	telepathy-mission-control-5 telepathy-salut thunderbird 
	thunderbird-gnome-support tk tk8.6 toshset totem totem-common totem-mozilla 
	totem-plugins transmission-common transmission-gtk ttf-indic-fonts-core 
	ttf-punjabi-fonts ttf-ubuntu-font-family ubuntu-artwork ubuntu-desktop 
	ubuntu-docs ubuntu-drivers-common ubuntu-extras-keyring ubuntu-mono 
	ubuntu-release-upgrader-gtk ubuntu-session ubuntu-settings ubuntu-sounds 
	ubuntu-sso-client ubuntu-sso-client-qt ubuntu-system-service 
	ubuntu-ui-toolkit-theme ubuntu-wallpapers ubuntu-wallpapers-trusty 
	ubuntuone-client-data udisks2 unity unity-asset-pool unity-control-center 
	unity-control-center-signon unity-greeter unity-gtk-module-common 
	unity-gtk2-module unity-gtk3-module unity-lens-applications unity-lens-files 
	unity-lens-friends unity-lens-music unity-lens-photos unity-lens-video 
	unity-scope-audacious unity-scope-calculator unity-scope-chromiumbookmarks 
	unity-scope-clementine unity-scope-colourlovers unity-scope-devhelp 
	unity-scope-firefoxbookmarks unity-scope-gdrive unity-scope-gmusicbrowser 
	unity-scope-gourmet unity-scope-guayadeque unity-scope-home 
	unity-scope-manpages unity-scope-musicstores unity-scope-musique 
	unity-scope-openclipart unity-scope-texdoc unity-scope-tomboy 
	unity-scope-video-remote unity-scope-virtualbox unity-scope-yelp 
	unity-scope-zotero unity-scopes-master-default unity-scopes-runner 
	unity-services unity-settings-daemon unity-voice-service 
	unity-webapps-common unity-webapps-qml unity-webapps-service uno-libs3 unzip 
	update-inetd update-manager update-notifier upower ure usb-creator-common 
	usb-creator-gtk usb-modeswitch usb-modeswitch-data usbmuxd vbetool vino 
	wamerican webaccounts-extension-common webapp-container webbrowser-app 
	whoopsie whoopsie-preferences wodim x11-apps x11-common x11-session-utils 
	x11-utils x11-xfs-utils x11-xkb-utils x11-xserver-utils xbitmaps 
	xcursor-themes xdg-user-dirs xdg-user-dirs-gtk xdg-utils xdiagnose 
	xfonts-base xfonts-encodings xfonts-mathml xfonts-scalable xfonts-utils 
	xinit xinput xorg xorg-docs-core xserver-common xserver-xorg 
	xserver-xorg-core xserver-xorg-input-all xserver-xorg-input-evdev
	xserver-xorg-input-mouse xserver-xorg-input-synaptics
	xserver-xorg-input-vmmouse xserver-xorg-input-wacom xserver-xorg-video-all
	xserver-xorg-video-ati xserver-xorg-video-cirrus xserver-xorg-video-fbdev
	xserver-xorg-video-glamoregl xserver-xorg-video-intel
	xserver-xorg-video-mach64 xserver-xorg-video-mga
	xserver-xorg-video-modesetting xserver-xorg-video-neomagic
	xserver-xorg-video-nouveau xserver-xorg-video-openchrome
	xserver-xorg-video-qxl xserver-xorg-video-r128 xserver-xorg-video-radeon
	xserver-xorg-video-s3 xserver-xorg-video-savage
	xserver-xorg-video-siliconmotion xserver-xorg-video-sis
	xserver-xorg-video-sisusb xserver-xorg-video-tdfx xserver-xorg-video-trident
	xserver-xorg-video-vesa xserver-xorg-video-vmware xterm xul-ext-ubufox
	xul-ext-unity xul-ext-webaccounts xul-ext-websites-integration xvt yelp
	yelp-xsl zeitgeist zeitgeist-core zeitgeist-datahub zenity zenity-common zip

  * Issue:<br />

  * Solution:<br />

  * Modify:<br />
	Remove brltty gnome-sudoku gnome-mines gnome-mines rhythmbox network-manager
	totem eog

  * State:<br />
	Purged

4. Lubuntu desktop intallation

  *	Run Instruction:<br />
		```$ sudo apt-get install lubuntu-desktop```

  *	Packages had been installed:<br />
	abiword abiword-common abiword-plugin-grammar abiword-plugin-mathview acl
	acpi-support alsa-base alsa-utils anacron apg app-install-data apport-gtk
	aptdaemon aptdaemon-data apturl apturl-common aspell aspell-en at-spi2-core
	audacious audacious-plugins audacious-plugins-data avahi-daemon avahi-utils
	blueman bluez bluez-alsa bluez-cups cheese-common colord consolekit cpp
	cpp-4.8 cracklib-runtime cups cups-browsed cups-bsd cups-client cups-common
	cups-core-drivers cups-daemon cups-driver-gutenprint cups-filters
	cups-filters-core-drivers cups-pk-helper cups-ppdc cups-server-common
	dbus-x11 dc dconf-cli dconf-gsettings-backend dconf-service desktop-base
	desktop-file-utils dialog dictionaries-common diffstat dmz-cursor-theme
	dnsmasq-base docbook-xml enchant evince evince-common evolution-data-server
	evolution-data-server-common evolution-data-server-online-accounts
	ffmpegthumbnailer file-roller firefox fontconfig fontconfig-config
	fonts-dejavu-core fonts-droid fonts-freefont-ttf fonts-kacst fonts-kacst-one
	fonts-khmeros-core fonts-lao fonts-liberation fonts-lklug-sinhala fonts-lyx
	fonts-nanum fonts-sil-abyssinica fonts-sil-padauk fonts-takao-pgothic
	fonts-thai-tlwg fonts-tibetan-machine fonts-tlwg-garuda fonts-tlwg-kinnari
	fonts-tlwg-loma fonts-tlwg-mono fonts-tlwg-norasi fonts-tlwg-purisa
	fonts-tlwg-sawasdee fonts-tlwg-typewriter fonts-tlwg-typist fonts-tlwg-typo
	fonts-tlwg-umpush fonts-tlwg-waree foomatic-db-compressed-ppds galculator
	gconf-service gconf-service-backend gconf2 gconf2-common gcr gdb gdebi
	gdebi-core gdisk gecko-mediaplayer genisoimage geoclue geoclue-ubuntu-geoip
	gettext ghostscript ghostscript-x giblib1 gir1.2-atk-1.0
	gir1.2-dbusmenu-glib-0.4 gir1.2-dee-1.0 gir1.2-freedesktop
	gir1.2-gdkpixbuf-2.0 gir1.2-gnomebluetooth-1.0 gir1.2-gstreamer-1.0
	gir1.2-gtk-3.0 gir1.2-gudev-1.0 gir1.2-ibus-1.0 gir1.2-javascriptcoregtk-3.0
	gir1.2-notify-0.7 gir1.2-packagekitglib-1.0 gir1.2-pango-1.0 gir1.2-soup-2.4
	gir1.2-udisks-2.0 gir1.2-unity-5.0 gir1.2-vte-2.90 gir1.2-webkit-3.0
	gir1.2-wnck-3.0 gkbd-capplet gksu glib-networking glib-networking-common
	glib-networking-services gnome-accessibility-themes gnome-bluetooth
	gnome-control-center-shared-data gnome-desktop-data gnome-desktop3-data
	gnome-disk-utility gnome-icon-theme gnome-icon-theme-full
	gnome-icon-theme-symbolic gnome-keyring gnome-menus gnome-mplayer
	gnome-power-manager gnome-screensaver gnome-session-bin
	gnome-settings-daemon-schemas gnome-system-tools gnome-themes-standard
	gnome-themes-standard-data gnome-user-guide gnome-user-share gnumeric
	gnumeric-common gnumeric-doc gpicview gsettings-desktop-schemas
	gsettings-ubuntu-schemas gsfonts gstreamer0.10-nice
	gstreamer0.10-plugins-base gstreamer0.10-plugins-good
	gstreamer0.10-pulseaudio gstreamer0.10-x gstreamer1.0-clutter
	gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-x
	gtk2-engines gtk2-engines-murrine gtk2-engines-pixbuf gtk3-engines-unico
	gucharmap guvcview gvfs gvfs-backends gvfs-common gvfs-daemons gvfs-fuse
	gvfs-libs hardening-includes hardinfo hicolor-icon-theme hplip hplip-data
	humanity-icon-theme hunspell-en-us hwdata ibus ibus-gtk ibus-gtk3 im-config
	indicator-applet indicator-application indicator-application-gtk2
	indicator-bluetooth indicator-datetime indicator-keyboard indicator-messages
	indicator-power indicator-session indicator-sound inputattach
	intltool-debian iputils-arping kerneloops-daemon language-selector-gnome
	leafpad liba52-0.7.4 libaa1 libaacs0 libabiword-3.0 libaccount-plugin-1.0-0
	libaccount-plugin-generic-oauth libaccount-plugin-google libaccounts-glib0
	libaccounts-qt5-1 libappindicator3-1 libapt-pkg-perl libarchive-zip-perl
	libarchive13 libart-2.0-2 libasound2 libasound2-data libasound2-plugins
	libaspell15 libasprintf-dev libass4 libassuan0 libasyncns0 libatasmart4
	libatk-bridge2.0-0 libatk1.0-0 libatk1.0-data libatspi2.0-0 libaudclient2
	libaudcore1 libauthen-sasl-perl libautodie-perl libavahi-client3
	libavahi-common-data libavahi-common3 libavahi-core7 libavahi-glib1
	libavc1394-0 libavcodec54 libavformat54 libavresample1 libavutil52
	libbinio1ldbl libbluetooth3 libbluray1 libbs2b0 libburn4 libc6-dbg libcaca0
	libcairo-gobject2 libcairo-perl libcairo2 libcamel-1.2-45 libcanberra-gtk3-0
	libcanberra-gtk3-module libcanberra-pulse libcanberra0 libcddb2
	libcdio-cdda1 libcdio-paranoia1 libcdio13 libcdparanoia0 libchamplain-0.12-0
	libchamplain-gtk-0.12-0 libcheese-gtk23 libcheese7 libclone-perl
	libcloog-isl4 libclutter-1.0-0 libclutter-1.0-common libclutter-gst-2.0-0
	libclutter-gtk-1.0-0 libcogl-common libcogl-pango15 libcogl15 libcolamd2.8.0
	libcolord1 libcolorhug1 libcompfaceg1 libcrack2 libcroco3
	libcrypt-passwdmd5-perl libcue1 libcups2 libcupscgi1 libcupsfilters1
	libcupsimage2 libcupsmime1 libcupsppdc1 libdaemon0 libdatrie1
	libdbusmenu-glib4 libdbusmenu-gtk3-4 libdbusmenu-gtk4 libdca0 libdconf1
	libdee-1.0-4 libdigest-hmac-perl libdirectfb-1.2-9 libdiscid0
	libdjvulibre-text libdjvulibre21 libdpkg-perl libdrm-intel1 libdrm-nouveau2
	libdrm-radeon1 libdv4 libdvdnav4 libdvdread4 libebackend-1.2-7
	libebook-1.2-14 libebook-contacts-1.2-0 libecal-1.2-16 libedata-book-1.2-20
	libedata-cal-1.2-23 libedataserver-1.2-18 libegl1-mesa libegl1-mesa-drivers
	libelfg0 libemail-valid-perl libenca0 libenchant1c2a libencode-locale-perl
	libevdocument3-4 libevview3-3 libexif12 libexo-1-0 libexo-common
	libexo-helpers libfaad2 libfarstream-0.1-0 libffmpegthumbnailer4
	libfftw3-single3 libfile-basedir-perl libfile-copy-recursive-perl
	libfile-desktopentry-perl libfile-fcntllock-perl libfile-listing-perl
	libfile-mimeinfo-perl libflac8 libfluidsynth1 libfm-data libfm-extra4
	libfm-gtk-data libfm-gtk4 libfm-modules libfm4 libfont-afm-perl
	libfontconfig1 libfontembed1 libfontenc1 libframe6 libfs6 libgail-3-0
	libgbm1 libgconf-2-4 libgcr-ui-3-1 libgd3 libgda-5.0-4 libgda-5.0-common
	libgdata-common libgdata13 libgdk-pixbuf2.0-0 libgdk-pixbuf2.0-common
	libgdome2-0 libgdome2-cpp-smart0c2a libgee2 libgeis1 libgeoclue0
	libgettextpo-dev libgettextpo0 libgif4 libgksu2-0 libgl1-mesa-dri
	libgl1-mesa-glx libglamor0 libglapi-mesa libgles2-mesa libglib-perl
	libglib2.0-bin libglu1-mesa libgmlib1 libgmp10 libgmtk1 libgmtk1-data
	libgnome-bluetooth11 libgnome-desktop-3-7 libgnome-keyring-common
	libgnome-keyring0 libgnome-menu-3-0 libgnomekbd-common libgnomekbd8
	libgoa-1.0-0b libgoa-1.0-common libgoffice-0.10-10 libgoffice-0.10-10-common
	libgomp1 libgpgme11 libgphoto2-6 libgphoto2-l10n libgphoto2-port10
	libgpod-common libgpod4 libgrail6 libgraphite2-3 libgrip0 libgs9
	libgs9-common libgsf-1-114 libgsf-1-common libgsm1 libgssdp-1.0-3
	libgstreamer-plugins-base0.10-0 libgstreamer-plugins-base1.0-0
	libgstreamer-plugins-good1.0-0 libgstreamer0.10-0 libgstreamer1.0-0
	libgtk-3-0 libgtk-3-bin libgtk-3-common libgtk2-perl libgtk2.0-0
	libgtk2.0-bin libgtk2.0-common libgtkmathview0c2a libgtkspell0 libgtop2-7
	libgtop2-common libgucharmap-2-90-7 libgudev-1.0-0 libguess1 libgupnp-1.0-4
	libgupnp-igd-1.0-4 libgusb2 libgutenprint2 libgweather-3-6
	libgweather-common libgxps2 libharfbuzz-icu0 libharfbuzz0b libhpmud0
	libhtml-form-perl libhtml-format-perl libhtml-parser-perl
	libhtml-tagset-perl libhtml-tree-perl libhttp-cookies-perl
	libhttp-daemon-perl libhttp-message-perl libhttp-negotiate-perl
	libhunspell-1.3-0 libibus-1.0-5 libical1 libice6 libicu52 libid3tag0
	libido3-0.1-0 libiec61883-0 libieee1284-3 libijs-0.35 libimlib2
	libimobiledevice4 libindicator3-7 libindicator7 libio-html-perl
	libio-pty-perl libio-socket-inet6-perl libio-socket-ssl-perl libipc-run-perl
	libipc-system-simple-perl libisl10 libisofs6 libjack-jackd2-0 libjasper1
	libjavascriptcoregtk-3.0-0 libjbig0 libjbig2dec0 libjpeg-turbo8 libjpeg8
	libjs-jquery libjson-glib-1.0-0 libjson-glib-1.0-common libjte1 libkpathsea6
	liblcms2-2 libldb1 liblightdm-gobject-1-0 liblink-grammar4 liblircclient0
	liblist-moreutils-perl libllvm3.4 libloudmouth1-0 libltdl7 liblua5.2-0
	liblwp-mediatypes-perl liblwp-protocol-https-perl liblzo2-2 libmad0
	libmailtools-perl libmbim-glib0 libmeanwhile1 libmenu-cache-bin
	libmenu-cache3 libmessaging-menu0 libmhash2 libminiupnpc8 libmm-glib0
	libmms0 libmnl0 libmodplug1 libmowgli2 libmp3lame0 libmpc3 libmpfr4
	libmpg123-0 libmtp-common libmtp-runtime libmtp9 libmusicbrainz3-6
	libnatpmp1 libnautilus-extension1a libneon27-gnutls libnet-dbus-perl
	libnet-dns-perl libnet-domain-tld-perl libnet-http-perl libnet-ip-perl
	libnet-libidn-perl libnet-smtp-ssl-perl libnet-ssleay-perl
	libnetfilter-conntrack3 libnettle4 libnice10 libnl-route-3-200
	libnm-glib-vpn1 libnm-glib4 libnm-gtk-common libnm-gtk0 libnm-util2
	libnotify-bin libnotify4 libnspr4 libnss-mdns libnss3 libnss3-nssdb libntdb1
	liboauth0 libobrender29 libobt2 libogg0 libonig2 liboobs-1-5 libopenjpeg2
	libopenobex1 libopts25 libopus0 liborc-0.4-0 libots0
	libp11-kit-gnome-keyring libpackagekit-glib2-16 libpam-ck-connector
	libpam-gnome-keyring libpanel-applet-4-0 libpango-1.0-0 libpango-perl
	libpango1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 libpangox-1.0-0
	libpangoxft-1.0-0 libpaper-utils libpaper1 libpciaccess0 libperl5.18
	libperlio-gzip-perl libpisock9 libpixman-1-0 libplist1 libpoppler-glib8
	libpoppler44 libportaudio2 libpostproc52 libproxy1 libpulse-mainloop-glib0
	libpulse0 libpulsedsp libpurple-bin libpurple0 libpwquality-common
	libpwquality1 libpython3.4 libqmi-glib0 libqpdf13 libqt5core5a libqt5dbus5
	libqt5gui5 libqt5network5 libqt5opengl5 libqt5positioning5
	libqt5printsupport5 libqt5qml5 libqt5quick5 libqt5sensors5 libqt5sql5
	libqt5sql5-sqlite libqt5test5 libqt5webkit5 libqt5widgets5 libqt5xml5
	libquadmath0 libquvi-scripts libquvi7 libraptor2-0 librarian0 librasqal3
	libraw1394-11 librdf0 librest-0.7-0 librsvg2-2 librsvg2-common
	libsamplerate0 libsane libsane-common libsane-hpaio libschroedinger-1.0-0
	libsdl1.2debian libsecret-1-0 libsecret-common libsgutils2-2 libshout3
	libsidplayfp libsignon-extension1 libsignon-glib1 libsignon-plugins-common1
	libsignon-qt5-1 libsm6 libsmbclient libsndfile1 libsnmp-base libsnmp30
	libsocket6-perl libsoup-gnome2.4-1 libsoup2.4-1 libspectre1 libspeex1
	libspeexdsp1 libstartup-notification0 libsub-identify-perl libswscale2
	libsystemd-journal0 libt1-5 libtag1-vanilla libtag1c2a libtalloc2 libtcl8.6
	libtdb1 libtelepathy-glib0 libtevent0 libtext-levenshtein-perl libthai-data
	libthai0 libtheora0 libtidy-0.99-0 libtie-ixhash-perl libtiff5
	libtimezonemap1 libtk8.6 libts-0.0-0 libtxc-dxtn-s2tc0 libudisks2-0
	libuniconf4.6 libunistring0 libunity-control-center1
	libunity-protocol-private0 libunity-scopes-json-def-desktop libunity9
	libupower-glib1 liburi-perl liburl-dispatcher1 libusbmuxd2 libutempter0
	libv4l-0 libv4lconvert0 libva1 libvdpau1 libvisual-0.4-0
	libvisual-0.4-plugins libvorbis0a libvorbisenc2 libvorbisfile3 libvpx1
	libvte-2.90-9 libvte-2.90-common libvte-common libvte9 libwacom-common
	libwacom2 libwavpack1 libwayland-client0 libwayland-cursor0
	libwayland-egl1-mesa libwbclient0 libwebcam0 libwebkitgtk-3.0-0
	libwebkitgtk-3.0-common libwebp5 libwebpmux1 libwhoopsie0 libwmf0.2-7
	libwnck-3-0 libwnck-3-common libwnck-common libwnck22 libwpd-0.9-9
	libwpg-0.2-2 libwps-0.2-2 libwv-1.2-4 libwvstreams4.6-base
	libwvstreams4.6-extras libwww-perl libwww-robotrules-perl libx11-xcb1
	libx264-142 libx86-1 libxatracker2 libxaw7 libxcb-dri2-0 libxcb-dri3-0
	libxcb-glx0 libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-present0
	libxcb-randr0 libxcb-render-util0 libxcb-render0 libxcb-shape0 libxcb-shm0
	libxcb-sync1 libxcb-util0 libxcb-xkb1 libxcomposite1 libxcursor1 libxdamage1
	libxfce4ui-1-0 libxfce4ui-common libxfce4util-bin libxfce4util-common
	libxfce4util6 libxfconf-0-2 libxfixes3 libxfont1 libxft2 libxi6 libxinerama1
	libxkbcommon-x11-0 libxkbcommon0 libxklavier16 libxml-parser-perl
	libxml-twig-perl libxml-xpathengine-perl libxmu6 libxp6 libxpm4 libxrandr2
	libxrender1 libxres1 libxshmfence1 libxss1 libxt6 libxtst6 libxv1
	libxvidcore4 libxvmc1 libxxf86dga1 libxxf86vm1 libyajl2 libyelp0 libzephyr4
	light-locker light-locker-settings lightdm lightdm-gtk-greeter
	link-grammar-dictionaries-en lintian linux-sound-base lp-solve
	lubuntu-artwork lubuntu-artwork-14-04 lubuntu-core lubuntu-default-session
	lubuntu-default-settings lubuntu-desktop lubuntu-icon-theme
	lubuntu-lxpanel-icons lubuntu-software-center lxappearance
	lxappearance-obconf lxinput lxlauncher lxmenu-data lxpanel
	lxpanel-indicator-applet-plugin lxrandr lxsession lxsession-data
	lxsession-default-apps lxsession-logout lxshortcut lxtask lxterminal make
	mobile-broadband-provider-info modemmanager mousetweaks mplayer2 mscompress
	mtools mtpaint nautilus-data network-manager network-manager-gnome
	network-manager-pptp network-manager-pptp-gnome notification-daemon ntp
	obconf obex-data-server obexd-client openbox openprinting-ppds p11-kit
	p11-kit-modules patchutils pcmanfm pcmciautils pidgin pidgin-data
	pidgin-libnotify plymouth-label plymouth-theme-lubuntu-logo
	plymouth-theme-lubuntu-text pm-utils policykit-1-gnome
	policykit-desktop-privileges poppler-data poppler-utils pptp-linux
	printer-driver-c2esp printer-driver-foo2zjs printer-driver-foo2zjs-common
	printer-driver-gutenprint printer-driver-hpcups printer-driver-min12xxw
	printer-driver-pnm2ppa printer-driver-postscript-hp printer-driver-ptouch
	printer-driver-pxljr printer-driver-sag-gdi printer-driver-splix pulseaudio
	pulseaudio-module-x11 pulseaudio-utils python-aptdaemon
	python-aptdaemon.gtk3widgets python-cairo python-commandnotfound
	python-crypto python-cups python-cupshelpers python-dbus python-dbus-dev
	python-defer python-gconf python-gi python-gnomekeyring python-gobject
	python-gobject-2 python-gtk2 python-gudev python-imaging python-ldb
	python-libxml2 python-notify python-ntdb python-pexpect python-pil
	python-psutil python-pysqlite2 python-renderpm python-reportlab
	python-reportlab-accel python-samba python-smbc python-talloc python-tdb
	python-xdg python3-aptdaemon python3-aptdaemon.gtk3widgets
	python3-aptdaemon.pkcompat python3-chardet python3-debian python3-defer
	python3-pkg-resources python3-six python3-xdg python3-xkit qpdf
	rarian-compat rfkill rtkit samba-common samba-common-bin samba-libs
	sane-utils scrot session-migration sessioninstaller sgml-data
	signon-keyring-extension signon-plugin-oauth2 signon-ui signond simple-scan
	smbclient software-properties-gtk sound-theme-freedesktop sylpheed
	sylpheed-doc sylpheed-i18n sylpheed-plugins synaptic syslinux
	syslinux-common syslinux-legacy system-config-printer-common
	system-config-printer-gnome system-config-printer-udev system-tools-backends
	t1utils tcl tcl8.6 tk tk8.6 toshset transmission transmission-common
	transmission-gtk tsconf ttf-indic-fonts-core ttf-punjabi-fonts
	ttf-ubuntu-font-family ubuntu-drivers-common ubuntu-extras-keyring
	ubuntu-release-upgrader-gtk ubuntu-system-service udisks2
	unity-control-center unity-control-center-signon unity-greeter
	unity-settings-daemon unzip update-inetd update-manager update-notifier
	upower usb-creator-common usb-creator-gtk usb-modeswitch usb-modeswitch-data
	usbmuxd uvcdynctrl uvcdynctrl-data vbetool wamerican whoopsie wvdial
	x11-apps x11-common x11-session-utils x11-utils x11-xfs-utils x11-xkb-utils
	x11-xserver-utils xbitmaps xdg-user-dirs xdg-user-dirs-gtk xdg-utils xfburn
	xfce4-notifyd xfce4-power-manager xfce4-power-manager-data xfconf
	xfonts-100dpi xfonts-base xfonts-encodings xfonts-scalable xfonts-utils
	xinit xinput xorg xorg-docs-core xpad xserver-common xserver-xorg
	xserver-xorg-core xserver-xorg-input-all xserver-xorg-input-evdev
	xserver-xorg-input-mouse xserver-xorg-input-synaptics
	xserver-xorg-input-vmmouse xserver-xorg-input-wacom xserver-xorg-video-all
	xserver-xorg-video-ati xserver-xorg-video-cirrus xserver-xorg-video-fbdev 
	xserver-xorg-video-glamoregl xserver-xorg-video-intel
	xserver-xorg-video-mach64 xserver-xorg-video-mga
	xserver-xorg-video-modesetting xserver-xorg-video-neomagic
	xserver-xorg-video-nouveau xserver-xorg-video-openchrome
	xserver-xorg-video-qxl xserver-xorg-video-r128 xserver-xorg-video-radeon
	xserver-xorg-video-s3 xserver-xorg-video-savage
	xserver-xorg-video-siliconmotion xserver-xorg-video-sis
	xserver-xorg-video-sisusb xserver-xorg-video-tdfx xserver-xorg-video-trident
	xserver-xorg-video-vesa xserver-xorg-video-vmware xterm xul-ext-ubufox xvt
	yelp yelp-xsl zenity zenity-common zip

  * Issue:<br />

  * Solution:<br />

  * Modify:<br />

  * State:<br />

	Purge except the several packages:<br />
	dconf-gsettings-backend:i386 dconf-service libdconf1:i386 libdrm-intel1:i386
	libdrm-nouveau2:i386 libdrm-radeon1:i386 libegl1-mesa:i386 libfontconfig1:i386
	libgbm1:i386 libgdk-pixbuf2.0-0:i386 libgdk-pixbuf2.0-common
	libgl1-mesa-dri:i386 libglamor0:i386 libglapi-mesa:i386 libgtk-3-0:i386
	libgtk-3-common libice6:i386 libjasper1:i386 libjpeg8:i386 libllvm3.4:i386
	libnotify4:i386 libpango-1.0-0:i386	libpangocairo-1.0-0:i386
	libpangoft2-1.0-0:i386 libpciaccess0:i386 libpixman-1-0:i386 libthai0:i386
	libtiff5:i386 libutempter0 libwayland-client0:i386	libwayland-cursor0:i386
	libwebkitgtk-3.0-0:i386	libwebkitgtk-3.0-common libwebp5:i386	libx11-xcb1:i386
	libxatracker2:i386 libxaw7:i386 libxcb-dri2-0:i386 libxcb-util0:i386
	libxcomposite1:i386	libxcursor1:i386 libxdamage1:i386 libxfixes3:i386
	libxft2:i386 libxi6:i386 libxinerama1:i386	libxkbcommon0:i386
	libxmu6:i386 libxpm4:i386	libxrandr2:i386	libxrender1:i386

5. Webmin Installation
	
  * Run Instruction:<br />
	Reference [Webmin Installing on Debian](http://www.webmin.com/deb.html)

  * Packages had been installed:<br />
	apt-show-versions libauthen-pam-perl webmin

  * Issue:<br />
	The Web Server is running in SSL mode. Try the URL https://SERVER IP ADDRESS:10000/ instead.

  * Solution:<br />
	Reference to:	[Webmin SSL Solution Link](http://eitwebguru.com/webmin-error-the-web-server-is-running-in-ssl-mode/)

  * Modify:<br />

  * State:<br />
	Complete!!! :+1:
	
	You can now loging to [Remote link control](https://url:10000/) as root with
	your root password, or as any user who can use ```sudo``` to commands as root

## 2016-01-19
1. Gitweb Installation:
	
  * Run Instruction:<br />
		```$ sudo apt-get install gitweb```

  * Packages had been installed:<br />
	gitweb
	
  * Issue:<br />
	
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />	
	Complete!!!
	
2. Lighttpd Installation:
	
  * Run Instruction:<br />
		```$ sudo apt-get install lighttpd```

  * Packages had been installed:<br />
	gamin libgamin0 libterm-readline-perl-perl lighttpd spawn-fcgi
	
  * Issue:<br />
	2016-01-19 11:16:59: (network.c.405) can't bind to port:  80 Address already in use same port Apache2.
		
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />
	Complete!!!

3. Uninstall lightdm
	
  * Run Instruction:<br />
		```$ sudo apt-get purge lightdm```

  * Packages had been installed:<br />
	lightdm* lubuntu-core* lubuntu-default-session* lubuntu-default-settings*
	
  * Issue:<br />
		
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />	
	Complete!!!

4. Gitolite3 Installation
	
  * Run Instruction:<br />
		```$ sudo apt-get install gitolite3```
	
  * Packages had been installed:<br />
	apg bluez cheese-common gir1.2-gnomebluetooth-1.0 gkbd-capplet
  gnome-bluetooth gnome-desktop3-data gnome-menus
  gnome-settings-daemon-schemas gsettings-ubuntu-schemas gstreamer1.0-clutter
  indicator-bluetooth indicator-datetime indicator-keyboard indicator-power
  indicator-sound libcheese-gtk23 libcheese7 libclutter-gst-2.0-0 libcrack2
  libecal-1.2-16 libelfg0 libgee2 libglib2.0-bin libgnome-bluetooth11
  libgnome-desktop-3-7 libgnome-keyring-common libgnome-keyring0
  libgnome-menu-3-0 libgnomekbd-common libgnomekbd8 libgtop2-7 libgtop2-common
  libnm-gtk-common libnm-gtk0 libopenobex1 libpulse-mainloop-glib0
  libpwquality-common libpwquality1 libtimezonemap1 libunity-control-center1
  liburl-dispatcher1 libwacom-common libwacom2 lubuntu-icon-theme mousetweaks
  nautilus-data obex-data-server obexd-client policykit-desktop-privileges
  python-cups python-cupshelpers python-gnomekeyring python-libxml2
  python-smbc session-migration system-config-printer-common
  system-config-printer-gnome system-config-printer-udev ubuntu-system-service
  unity-control-center unity-greeter unity-settings-daemon
	
  * Issue:<br />
		
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />
	No adminkey given - not setting up gitolite. Do a dpkg-reconfigure to setup.

## 2016-01-20
1. Auto startup gitweb when server booting:
	
  * Run Instruction:<br />
	Create a file named instaweb with the following content:<br />
	```
	### BEGIN INIT INFO
	# Provides:          git
	# Required-Start:    $local_fs $remote_fs $network $syslog
	# Required-Stop:     $local_fs $remote_fs $network $syslog
	# Should-Start:      fam
	# Should-Stop:       fam
	# Default-Start:     2 3 4 5
	# Default-Stop:      0 1 6
	# Short-Description: Start the lighttpd git server.
	# Description:       Fast and smalle webserver with minimal memory footprint
	#                    developed with security in mind HTTP/1.1 compliant caching
	#                    proxy server.
	### END INIT INFO


	PATH=/sbin:/bin:/usr/sbin:/usr/bin
	DAEMON=/usr/bin/git
	NAME=instaweb
	DESC="git server"
	PIDFILE=/var/run/$NAME.pid
	SCRIPTNAME=/etc/init.d/$NAME

	DAEMON_OPTS="instaweb --port=1234"

	sudo -H -u git bash -c "cd /home/git/repositories/gitolite-admin.git && $DAEMON $DAEMON_OPTS"

	exit 0
	```
	Then move this file into ```/etc/init.d/```

  * Packages had been installed:<br />
	
  * Issue:<br />
	
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />
	Complete!!! :+1:

2. Remove unused packages
	
  * Run Instruction:<br />
		```$ sudo apt-get autoremove --purge```
	
  * Packages had been remove:<br />

  apg* bluez* cheese-common* gir1.2-gnomebluetooth-1.0* gir1.2-notify-0.7*
  gkbd-capplet* gnome-bluetooth* gnome-desktop3-data* gnome-menus*
  gnome-settings-daemon-schemas* gsettings-ubuntu-schemas*
  gstreamer1.0-clutter* gtk2-engines-murrine* gtk2-engines-pixbuf*
  gtk3-engines-unico* indicator-bluetooth* indicator-datetime*
  indicator-keyboard* indicator-power* indicator-sound* libcheese-gtk23*
  libcheese7* libclutter-gst-2.0-0* libcrack2* libecal-1.2-16* libelfg0*
  libgee2* libglib2.0-bin* libgnome-bluetooth11* libgnome-desktop-3-7*
  libgnome-keyring-common* libgnome-keyring0* libgnome-menu-3-0*
  libgnomekbd-common* libgnomekbd8* libgtop2-7* libgtop2-common*
  libnm-gtk-common* libnm-gtk0* libopenobex1* libpulse-mainloop-glib0*
  libpwquality-common* libpwquality1* libtimezonemap1*
  libunity-control-center1* liburl-dispatcher1* libwacom-common* libwacom2*
  linux-headers-3.19.0-25* linux-headers-3.19.0-25-generic*
  linux-image-3.19.0-25-generic* linux-image-extra-3.19.0-25-generic*
  mousetweaks* nautilus-data* obex-data-server* obexd-client* plymouth-label*
  policykit-desktop-privileges* python-cups* python-cupshelpers*
  python-gnomekeyring* python-libxml2* python-pysqlite2* python-smbc*
  session-migration* system-config-printer-common*
  system-config-printer-gnome* system-config-printer-udev*
  ubuntu-system-service* unity-control-center* unity-greeter*
  unity-settings-daemon*

  * Issue:<br />
	
  * Solution:<br />
	
  * Modify:<br />

  * State:<br />
	Complete!!! :+1:

3. Disable auto startup gitweb when server booting and auto startup when login
	
  * Run Instruction:<br />
	copy /etc/init.d/instaweb into /home/git/:<br />
	```$ sudo cp /etc/init.d/instaweb /home/git/instaweb.sh```<br />
	Edit in file just be copied:<br />
	```sudo -H -u git bash -c "cd /home/git/repositories/gitolite-admin.git && $DAEMON $DAEMON_OPTS"```<br />
	to:<br />
	```sudo -H bash -c "cd /home/git/repositories/gitolite-admin.git && $DAEMON $DAEMON_OPTS"```<br />
	change file owner and group:<br />
	```sudo chown root:root instaweb.sh```<br />
	remove instaweb into /etc/init.d/:<br />
	```$ sudo update-rc.d instaweb remove```<br />
	adding the following lines into .profile of each:<br />
	```
	# statup git instaweb
	if [ -f "path-to-file/instaweb.sh" ]; then
		path-to-file/instaweb.sh```
	fi
	```	
	finally, approve the change:<br />
	```	$ source ~/.profile	```

  * Packages had been changed:<br />

  * Issue:<br />
	w3m (or lynx) automatic startup
	
  * Solution:<br />
  Open and edit /usr/lib/git-core/git-instaweb:<br />
	```sudo nano /usr/lib/git-core/git-instaweb```<br />
	You comment 5 last lines and save this file.<br />
	So, if You did not wanna edit that file above, You'd get ```w3m``` (or ```lynx```) out by press ```q``` then press ```y``` on your keyboard.<br />
	Another, you can remove ```w3m``` (or ```lynx```) too (not recommend):<br />
		```$ sudo apt-get remove w3m lynx```
	
  * Modify:<br />

  * State:<br />
	Complete!!! :+1:

## 2016-01-21
1. Vsftpd Installation:
	
  * Run Instruction:<br />
	```$ sudo apt-get install vsftpd```
	
  * Packages had been changed:<br />
	vsftpd
	
  * Issue:<br />
		
  * Solution:<br />
	
  * Modify:<br />
	
  * State:<br />
	Complete!!! :+1:
	
2. Create an user account not sudoer
	
  * Run Instruction:<br />
	Create an user account not sudoer named vsftpd: <br />
	```sudo useradd --shell /bin/bash -u 1002 -b /var/www -m vsftpd```<br />
	Change the name of $HOME user directory:<br />
	```sudo mv /var/www/vsftpd /var/www/ftp```<br />
	Set passwd for new account:<br />
	```sudo passwd vsftpd```<br />
	Type and retype password which you want. Password is NOT appear.<br />
	
	Create a new group named vsftpd:<br />
	```sudo addgroup --gid 1002 vsftpd```<br />
	Modify /etc/passwd as root:<br />
	```sudo nano /etc/passwd```<br />	
	Switch to the line beginning with ```vsftpd``` and changed as follows:<br />
	```vsftpd:x:1002:1002:vsftpd,,,:/var/www/ftp:/bin/bash```<br />
	Then save and quit nano.
	
	Make symbolic link between one of directories in /var/www/ftp and /svr/ftp:<br />
	```sudo ln -s /var/www/ftp/name_of_directory /svr/ftp```
	
  * Packages had been changed:<br />
	
  * Issue:<br />
		
  * Solution:<br />
	
  * Modify:<br />
	
  * State:<br />
	Complete!!! :+1:
	
3. Reconfigure vsftpd, allow anonymous and local users to log in:

  * Run Instruction:<br />
	Log in with sudoer user<br />
	Create an user account not sudoer named vsftpd:<br />
	```sudo nano /etc/vsftpd.conf```<br />
	Type present user's password . Password is NOT appear.
	
	Delete all content and copy the following lines:<br />
	```
	# Example config file /etc/vsftpd.conf
	#
	# The default compiled in settings are fairly paranoid. This sample file
	# loosens things up a bit, to make the ftp daemon more usable.
	# Please see vsftpd.conf.5 for all compiled in defaults.
	#
	# READ THIS: This example file is NOT an exhaustive list of vsftpd options.
	# Please read the vsftpd.conf.5 manual page to get a full idea of vsftpd's
	# capabilities.
	#
	#
	# Run standalone?  vsftpd can run either from an inetd or as a standalone
	# daemon started from an initscript.
	listen=YES
	#
	# Run standalone with IPv6?
	# Like the listen parameter, except vsftpd will listen on an IPv6 socket
	# instead of an IPv4 one. This parameter and the listen parameter are mutually
	# exclusive.
	#listen_ipv6=YES
	#
	# Allow anonymous FTP? (Disabled by default)
	anonymous_enable=YES
	#
	# Uncomment this to allow local users to log in.
	local_enable=YES
	#
	# Uncomment this to enable any form of FTP write command.
	write_enable=YES
	#
	# Default umask for local users is 077. You may wish to change this to 022,
	# if your users expect that (022 is used by most other ftpd's)
	#local_umask=022
	#
	# Uncomment this to allow the anonymous FTP user to upload files. This only
	# has an effect if the above global write enable is activated. Also, you will
	# obviously need to create a directory writable by the FTP user.
	#anon_upload_enable=YES
	#
	# Uncomment this if you want the anonymous FTP user to be able to create
	# new directories.
	#anon_mkdir_write_enable=YES
	#
	# Activate directory messages - messages given to remote users when they
	# go into a certain directory.
	dirmessage_enable=YES
	#
	# If enabled, vsftpd will display directory listings with the time
	# in  your  local  time  zone.  The default is to display GMT. The
	# times returned by the MDTM FTP command are also affected by this
	# option.
	use_localtime=YES
	#
	# Activate logging of uploads/downloads.
	xferlog_enable=YES
	#
	# Make sure PORT transfer connections originate from port 20 (ftp-data).
	connect_from_port_20=YES
	#
	# If you want, you can arrange for uploaded anonymous files to be owned by
	# a different user. Note! Using "root" for uploaded files is not
	# recommended!
	#chown_uploads=YES
	#chown_username=whoever
	#
	# You may override where the log file goes if you like. The default is shown
	# below.
	#xferlog_file=/var/log/vsftpd.log
	#
	# If you want, you can have your log file in standard ftpd xferlog format.
	# Note that the default log file location is /var/log/xferlog in this case.
	#xferlog_std_format=YES
	#
	# You may change the default value for timing out an idle session.
	#idle_session_timeout=600
	#
	# You may change the default value for timing out a data connection.
	#data_connection_timeout=120
	#
	# It is recommended that you define on your system a unique user which the
	# ftp server can use as a totally isolated and unprivileged user.
	#nopriv_user=ftpsecure
	#
	# Enable this and the server will recognise asynchronous ABOR requests. Not
	# recommended for security (the code is non-trivial). Not enabling it,
	# however, may confuse older FTP clients.
	#async_abor_enable=YES
	#
	# By default the server will pretend to allow ASCII mode but in fact ignore
	# the request. Turn on the below options to have the server actually do ASCII
	# mangling on files when in ASCII mode.
	# Beware that on some FTP servers, ASCII support allows a denial of service
	# attack (DoS) via the command "SIZE /big/file" in ASCII mode. vsftpd
	# predicted this attack and has always been safe, reporting the size of the
	# raw file.
	# ASCII mangling is a horrible feature of the protocol.
	ascii_upload_enable=YES
	ascii_download_enable=YES
	#
	# You may fully customise the login banner string:
	ftpd_banner=Welcome to ASE Laboratory FTP service.
	#
	# You may specify a file of disallowed anonymous e-mail addresses. Apparently
	# useful for combatting certain DoS attacks.
	#deny_email_enable=YES
	# (default follows)
	#banned_email_file=/etc/vsftpd.banned_emails
	#
	# You may restrict local users to their home directories.  See the FAQ for
	# the possible risks in this before using chroot_local_user or
	# chroot_list_enable below.
	#chroot_local_user=YES
	#
	# You may specify an explicit list of local users to chroot() to their home
	# directory. If chroot_local_user is YES, then this list becomes a list of
	# users to NOT chroot().
	# (Warning! chroot'ing can be very dangerous. If using chroot, make sure that
	# the user does not have write access to the top level directory within the
	# chroot)
	#chroot_local_user=YES
	#chroot_list_enable=YES
	# (default follows)
	#chroot_list_file=/etc/vsftpd.chroot_list
	#
	# You may activate the "-R" option to the builtin ls. This is disabled by
	# default to avoid remote users being able to cause excessive I/O on large
	# sites. However, some broken FTP clients such as "ncftp" and "mirror" assume
	# the presence of the "-R" option, so there is a strong case for enabling it.
	#ls_recurse_enable=YES
	#
	# Customization
	#
	# Some of vsftpd's settings don't fit the filesystem layout by
	# default.
	#
	# This option should be the name of a directory which is empty.  Also, the
	# directory should not be writable by the ftp user. This directory is used
	# as a secure chroot() jail at times vsftpd does not require filesystem
	# access.
	secure_chroot_dir=/var/run/vsftpd/empty
	#
	# This string is the name of the PAM service vsftpd will use.
	pam_service_name=vsftpd
	#
	# This option specifies the location of the RSA certificate to use for SSL
	# encrypted connections.
	rsa_cert_file=/etc/ssl/certs/ssl-cert-snakeoil.pem
	# This option specifies the location of the RSA key to use for SSL
	# encrypted connections.
	rsa_private_key_file=/etc/ssl/private/ssl-cert-snakeoil.key

	# Connection limit for each IP
	max_per_ip=2
	# Maximum number of clients:
	max_clients=30

	# PASV port
	pasv_min_port=12000
	pasv_max_port=12100

	# Home directory
	local_root=/var/www/ftp
	anon_root=/var/www/ftp
	```
	Save and close nano.
	
  * Packages had been changed:<br />
	
  * Issue:<br />
		
  * Solution:<br />
	
  * Modify:<br />
	
  * TO-DO:<br />
	Create and config ftp virtual users.
	
  * State:<br />
	Complete!!! :+1:

