<https://www.cyberciti.biz/faq/linux-list-disk-partitions-command/>  
(url not available??) <https://wikka.puppylinux.com/Buildsystems>  
<https://landchad.net/gemini>  
<https://distro.tube/index.html>  
<https://www.learnlinux.tv/test-2/>  
<https://miro.medium.com/max/1836/1*eOnDXJOEREW6Q6MFiTucAw.png>

Best minimal options to research:

------------------------------------

- Puppy cookbook with ubuntu/debian as the base
- TinyCore works
- slitaz

What is the end goal that I want to achieve the most:
1. fast linux command line
2. install and run software on linux
3. run and try GUIs or distros
4. cook-up iso's

# :: Tiny Core Core/Plus ::
- <willhaley.com/blog/simple-portable-linux-qemu-vm-usb>
- extracted vmlinuz and core.gz out of iso with 7zip program
- download qemu version which is portable Eric Lassauge
- create vhd disk for qemu

`qemu-img create -f vpc tc.vhd 1G`
- plug that in with the qemu instruction (see file for command line)
- you need to format the virtual hard drive first time you boot-up

`printf "o\nn\np\n1\n\n\nw\n" | sudo fdisk /dev/sda`  
`sudo mkfs.ext4 /dev/sda1`

- reboot

## Fix clocksource
 - `cat /sys/devices/system/clocksource/clocksource0/current_clocksource`
 - `cat /sys/devices/system/clocksource/clocksource0/available_clocksource`
 - `echo hpet | sudo tee /sys/devices/system/clocksource/clocksource0/current_clocksource`


## booting qemu command
- `qemu-system-x86_64 -boot d -cdrom image.iso -m 512 [-hda mydisk.img]`
- last optional part above is if you created a disk image to read/write to during installs

<https://erikveen.dds.nl/qemupuppy/index.html>    
<https://project-awesome.org/PandaFoss/Awesome-Arch#arch-based-projects>

EasyOS Builds - <https://easyos.org/dev/how-to-compile-a-linux-distribution-from-source.html>  
Puppy Builds - With Woof-CE <https://puppylinux.com/woof-ce.html>  
WeeDog Builds - Details: <https://oldforum.puppylinux.com/viewtopic.php?t=116212&i=1>  
Debian Builds -   
Ubuntu Builds - 

# :: BYO Arch ::
Arco - mixer edition of arch (i've looked at this a lot, but confusing...)  
calam-arch - plain arch with graphical installer  
archinstall - included script  
arch linux GUI min  
archfi  
anarchyinstaller.gitlab.io    
<https://osdn.net/projects/ezarch/>  

arch from scratch??  
arch btw??  
Arch Install Guide(s)  

# :: Lightweight Arch ::
<https://artixlinux.org> - outdated and is a protest distro over systemd init change  
<https://maboxlinux.org> - openbox edition  
<https://axyl-os.github.io/>  
<https://rebornos.org>  
<https://archlabslinux.com>  
<https://archlinux.org/>  
<https://sourceforge.net/projects/snallinux/>  
<https://peux-os.netlify.app/>  
<https://archbang.org/>  

qtile window manager  
openbox

# :: Full Arch Linux ::
<https://manjaro.org>- one of the leading distros overall  
<https://endeavouros.com> - upcoming option in this space/category grouping  
<https://garudalinux.org>- another upcoming option/gaming crowd appeal  
<https://archcraft.io> - stylistic version, making the arch setup look good and run   
<https://instantos.io>  
<https://caesar-rylan.60.nu/lirix/>  
xerolinux  
<https://web.obarun.org/>  
<https://salientos.github.io/>  
hefftor  
<https://endlessos.com/home/>  

creation of reproducible arch build that I can pump out, copy, paste, re-load fresh copy)

# :: Debian/Ubuntu ::
Debian  
Ubuntu  
<https://cutefish-ubuntu.github.io/>  
<https://zephix-linux.sourceforge.io/>  
<https://sourceforge.net/projects/eznixos/>  
modicia os (ubuntu)  
<https://zorinos.com/>  
<https://elementary.io/>  
<https://ubuntu.com/>  
<https://www.debian.org/>  
<https://peppermintos.com/>  
<https://pop.system76.com/> -   

# :: Puppy List ::
- Puppy
- WeeDog
- EasyOS
<https://easyos.org/>  
<http://distro.ibiblio.org/fatdog/web/faqs/uefi-flashdrive2.html>  
<http://murga-linux.com/puppy/viewtopic.php?p=977466>  
<http://helledussen.com/linux/files/UEFI_boot/make_uefi-bootable_usb.html>  
<https://www.bleepingcomputer.com/forums/t/679911/puppy-linux-usb-fail-to-boot/>  
<https://chrisjrob.com/2010/04/30/make-a-linux-usb-key/>  
<https://weedoglinux.rockedge.org/viewtopic.php?f=41&t=28&sid=72e17dac324e4d36bb91874db92786c5>  
<https://www.tinylinux.info/>  
<https://forum.puppylinux.com/viewforum.php?f=33>  
<https://www.techrepublic.com/article/solutionbase-puppy-linux-teaches-an-old-dog-new-tricks/>  
<http://www.murga-linux.com/puppy/viewtopic.php?p=517224#517224>  
<https://docs.google.com/document/d/1bkMJ-2wjAAC8HVZZTZBFxBELbojoGctLMg27KazqvRw/edit?hl=en#>  
<https://www.linuxsecrets.com/puppylinux/Remastering.html>  
<https://distro.ibiblio.org/fatdog/web/#download>  
<http://distro.ibiblio.org/fatdog/web/faqs/harddrive.html>  
<http://wikka.puppylinux.com/USBBootwithoutBIOSSupport>  

# :: Experimental List ::
<https://kisslinux.org/>  
<https://www.exton.net/>  
<https://www.mocaccino.org/>  
<https://rlxos.dev/>  
<https://serpentos.com> (ikey doherty)  
<https://peropesis.org/>  
<https://carbslinux.org/>  
<https://bellard.org/>  
<https://vfsync.org/index.html>  
<https://bellard.org/jslinux/tech.html>  
<https://github.com/arjun024/mkeykernel>  
<https://fossbytes.com/dahliaos-custom-fuchsia-os-a-linux-distro/amp/>  
<https://github.com/ivandavidov/minimal>  
<https://distr1.org/>  
<https://dystroy.org/broot/>  
<https://justine.storage.googleapis.com/ape.html>  
<https://loganljohnson.cygo.network/main/>  
<https://draugeros.org/go/>  
<https://opensource.com/article/21/8/what-busybox>  
<https://superuser.com/questions/307087/linux-distro-with-just-busybox-and-bash>  
<https://re-ws.pl/2020/11/busybox-based-linux-distro-from-scratch/>  
<https://github.com/jaromaz/yosild>  
<https://l3net.wordpress.com/2014/02/15/a-memory-comparison-of-light-linux-desktops-part-3/>  
<https://l3net.wordpress.com/2013/04/30/lightweight-debian-lxde-desktop-from-scratch/>  
<https://linuxconfig.org/how-to-run-x-applications-without-a-desktop-or-a-wm>  
<https://superuser.com/questions/904142/launching-programs-with-gui-without-display-manager>  
<https://wiki.archlinux.org/index.php/Xinit>  
<https://wiki.archlinux.org/index.php/window_manager>  
<https://github.com/skiffos/SkiffOS>  
<https://discourse.nixos.org/t/skiffos-cross-compiled-container-initramfs-wrapping-nixos/9708>  
<https://dev.to/mauro_codes/switching-to-arch-linux-1hm>  
<https://linux.softpedia.com/get/System/Operating-Systems/Other/KolibriOS-23358.shtml>  
<http://www.kolibrios.org/en/>  
<https://github.com/ivandavidov/minimal>  
<http://tinycorelinux.net/book.html>  
<https://www.hirensbootcd.org/>  
<https://www.plop.at/en/bootmanagers.html>  
<https://blissos.org/>

# :: Unknowns or independent ::
<https://osdn.net/projects/hanhlinuxiso/releases/>  
Alpine  
<https://redox-os.org>  
<https://getsol.us/home/>  
<https://nxos.org/>  
<https://voidlinux.org/>  
<https://mxlinux.org/>  
<http://www.pclinuxos.com/>  
<https://www.linuxliteos.com/>  
<https://www.neverware.com/#intro>  
<https://distrowatch.com/ultimate>  
<https://liri.io/>  
<https://distrowatch.com/search.php?ostype=All&category=All&origin=All&basedon=Arch&notbasedon=None&desktop=All&architecture=All&package=All&rolling=All&isosize=All&netinstall=All&language=All&defaultinit=All&status=Active#simple>  
<https://www.ultimatebootcd.com/>  
<http://www.slitaz.org/en/>  

### Review these links to categorize them better:  
<https://www.linuxandubuntu.com/home/make-your-very-own-customized-linux-distro-from-your-current-installation>  
<https://www.linuxandubuntu.com/home/desktop-environments-for-linux>  
<https://ostechnix.com/how-to-create-a-custom-ubuntu-live-iso-image-with-cubic/>  
<https://www.kali.org/docs/development/live-build-a-custom-kali-iso/>  
<https://wiki.puppyrus.org/puppyrus/pra>  
<https://help.ubuntu.com/community/LiveCDCustomizationFromScratch>  
<https://bartsimons.me/ubuntu-linux-chroot-guide/>  
<https://help.ubuntu.com/lts/installation-guide/>  
<https://github.com/laurent85v/archuseriso>  

<https://newbedev.com/creating-bootable-debian-image-with-debootstrap>  
<https://wiki.termux.com/wiki/Main_Page>  
<https://medium.com/@lhennessy/up-and-running-with-arch-linux-on-virtualbox-d233c75df29d>  
<https://askubuntu.com/questions/343268/how-to-use-manual-partitioning-during-installation>  
<https://wiki.debian.org/SourcesList>  
<https://www.linuxfordevices.com/tutorials/ubuntu/fix-permission-denied-error>  
<https://ubuntuhandbook.org/index.php/how-to-install-ubuntu/>  
<https://tldp.org/LDP/sag/html/partitions.html>  
<https://gist.github.com/shinycore/d02f3968e02b7f548c68c039277912aa>  
<https://wiki.debian.org/Debootstrap>  

<https://aguslr.com/blog/2019/03/24/lightweight-debian.html>  
<https://www.debian.org/releases/stretch/amd64/apds03.html.en>  
<https://developer.ibm.com/tutorials/l-lpic1-102-2/>  
<https://docs.hytrust.com/DataControl/4.2/Admin_Guide-4.2/Content/Books/Admin-Guide/Linux-Root-Swap-Drive-Encryption/Creating-Boot-Partition-Ubuntu.htm?TocPath=Administration%20Guide%7CLinux%20Root%20and%20Swap%20Drive%20Encryption%7CPrerequisites%20and%20Restrictions%7C_____1>  
<https://www.gnu.org/software/grub/manual/grub/html_node/Installing-GRUB-using-grub_002dinstall.html>  
<https://forums.debian.net//viewtopic.php?f=17&t=134361>  

# Linux notes:

Ubuntu 20.04 LTS is installed in a VirtualBox
This is supported 5 years but will get out of date
If packages cannot be found to install or update you should first run:
`sudo apt update`

This command will refresh packages indexes and configuration of package installs
It doesn't install or download anything new specifically
If you want the most up to date packages INSTALLED you must run:
`sudo apt upgrade`

I don't know how this affects when there are other, newer ubuntu versions available and whether and when
those are downloaded and installed or not. I'm pretty cautious with this.


windows 10 install wsl2 (what to do with wsl1?)
`wsl --install`

Drop to console: [ctrl+alt+f3]

`dpkg-reconfigure -plow unattended-upgrades`

debootstrap (for ubuntu)  
--arch=amd64  
--variant=minbase [minbase|buildd|fakechroot]  
[name] see https://wiki.ubuntu.com/Releases  
[install folder]  
http://us.archive.ubuntu.com/ubuntu/ [mirror url?]  

debian sid/unstable package  
`wget http://http.us.debian.org/debian/pool/main/d/debootstrap/debootstrap_1.0.123_all.deb`
`sudo dpkg -i <pkg>`

low memory/power version of ubuntu on usb to use with hdmi pc.  
my procedure for developing this drive was to switch from gnome desktop to openbox  
remove the default login manager and install the slim manager:  
`sudo apt-get remove gdm3`
`sudo apt-get install slim`
<https://www.fosslicious.com/2018/05/install-and-change-display-manager.html>  

install the openbox wm
`sudo apt install openbox obconf`

what file(s) did I have to update in order to make it login under openbox instead of gnome??

<https://www.lifewire.com/install-openbox-using-ubuntu-4051832>  
<https://itsfoss.com/material-shell/>  
<https://itsfoss.com/free-boot-partition-ubuntu/>  
<https://opensource.com/article/19/12/favorite-terminal-emulator>  
<https://www.howtogeek.com/353819/how-to-make-ubuntu-look-more-like-windows/amp/>  
<https://fosspost.org/lists/turn-gnome-to-heaven-with-these-23-gnome-extensions>  
<https://itsfoss.com/best-gnome-extensions/>  
<https://askubuntu.com/questions/831216/how-can-i-reinstall-grub-to-the-efi-partition>  
<https://itsfoss.com/gnome-tricks-ubuntu/>  
<https://itsfoss.com/gnome-shell-extensions/>  
<https://itsfoss.com/free-up-space-ubuntu-linux/>  
<https://itsfoss.com/install-deepin-ubuntu/>  
<https://www.ubuntupit.com/best-linux-software-our-editorial-list-of-essential-linux-apps/>  
<https://www.google.com/amp/s/www.b247.eu.org/2019/01/gnome-calendar-and-outlookcom-two-way.html>  

<https://towardsdatascience.com/how-i-learned-to-enjoy-vim-e310e53e8d56>  
<https://opensource.com/article/20/12/jed>  

<https://opensource.com/article/20/6/modern-linux-command-line-tools>  
<https://dev.to/haydenrou/1-4-beginners-bash-basics-becoming-one-with-the-shell-mpk>  
<https://haydenjames.io/linux-commands-frequently-used-by-linux-sysadmins-part-1/>  
<https://haydenjames.io/linux-commands-frequently-used-by-linux-sysadmins-part-2/>  
<https://haydenjames.io/linux-commands-frequently-used-by-linux-sysadmins-part-3/>  
<https://haydenjames.io/linux-commands-frequently-used-by-linux-sysadmins-part-4/>  
<https://haydenjames.io/linux-commands-frequently-used-by-linux-sysadmins-part-5/>  
<https://itsfoss.com/connect-wifi-terminal-ubuntu/>  
<https://www.hndigest.com/m/hFqOFsRMRIlqmxeJn2zVdQ==/s/142741>  
<https://leimao.github.io/blog/Tmux-Tutorial/>  
Memory Use  
<https://www.linuxbabe.com/command-line/ubuntu-server-16-04-wifi-wpa-supplicant>  
<https://www.google.com/search?client=firefox-b-1-d&q=how-configure-wireless-any-linux-desktop>  
<https://itsfoss.com/always-on-top/>  
<https://www.gamingonlinux.com/2020/10/bpytop-might-be-the-freaking-coolest-way-to-monitor-your-linux-system>  

<https://www.linuxlinks.com/lxqt-lightweight-qt-desktop-environment/>  
<https://www.linuxlinks.com/budgie-desktop-flagship-desktop-environment-solus/>  
<https://www.linuxlinks.com/deepin-desktop-environment-desktop-environment-deepin-linux-distro/>  
<https://www.linuxlinks.com/enlightenment/>  
<https://www.linuxlinks.com/xfce/>  
<https://www.linuxlinks.com/cinnamon-desktop-environment-advanced-features/>  
<https://www.linuxlinks.com/mate-desktop-environment-continuation-gnome-2/>  
<https://www.linuxlinks.com/kde-plasma-desktop-environment-kde/>  
<https://www.linuxlinks.com/gnome-finely-crafted-desktop-environment/>  
<https://www.linux.com/tutorials/how-use-super-fast-i3-tiling-window-manager-linux/>  
<https://kde.org/plasma-desktop>  

<https://www.lifewire.com/install-openbox-using-ubuntu-4051832>  
<https://itsfoss.com/material-shell/>  
<https://itsfoss.com/free-boot-partition-ubuntu/>  
<https://opensource.com/article/19/12/favorite-terminal-emulator>  
<https://www.howtogeek.com/353819/how-to-make-ubuntu-look-more-like-windows/amp/>  
<https://fosspost.org/lists/turn-gnome-to-heaven-with-these-23-gnome-extensions>  
<https://itsfoss.com/best-gnome-extensions/>  
<https://askubuntu.com/questions/831216/how-can-i-reinstall-grub-to-the-efi-partition>  
<https://itsfoss.com/gnome-tricks-ubuntu/>  
<https://itsfoss.com/gnome-shell-extensions/>  
<https://itsfoss.com/free-up-space-ubuntu-linux/>  
<https://itsfoss.com/install-deepin-ubuntu/>  
<https://www.ubuntupit.com/best-linux-software-our-editorial-list-of-essential-linux-apps/>  
<https://www.google.com/amp/s/www.b247.eu.org/2019/01/gnome-calendar-and-outlookcom-two-way.html>  